### Core Principles

1. **Problem-Specific Analysis**
   - Thoroughly analyze the existing source.html code structure before proposing solutions
   - Identify specific bottlenecks causing negative cell over-segmentation
   - Consider the interplay between different processing stages

2. **Diverse Solution Generation**
   - Generate genuinely different approaches, not just parameter variations
   - Each solution must have a clear hypothesis about why it addresses the over-segmentation issue
   - Avoid copy-paste solutions; tailor each approach to the specific problem context

3. **Technical Rigor**
   - Base parameter choices on image analysis principles, not arbitrary values
   - Consider typical Ki67 staining characteristics (cell size: 10-20μm, staining patterns)
   - Ensure mathematical correctness in all implementations

4. **Implementation Standards**
   - Maintain clean, readable code with meaningful variable names
   - Include detailed comments explaining the rationale behind each modification
   - Preserve the original UI/UX flow while improving the core algorithm

5. **Category-Specific Guidelines**

   **For Preprocessing approaches:**
   - Consider how noise reduction affects subsequent segmentation
   - Balance between noise removal and detail preservation

   **For Segmentation approaches:**
   - Focus on methods that naturally handle touching/overlapping objects
   - Consider multi-scale or hierarchical approaches

   **For Morphology approaches:**
   - Carefully design kernel shapes to match typical cell geometry
   - Test different operation sequences for optimal defragmentation

   **For Contour processing:**
   - Implement smart merging criteria based on spatial and shape features
   - Consider watershed-like approaches for splitting merged cells

   **For Classification improvements:**
   - Expand feature space beyond simple color means
   - Implement adaptive thresholds based on image statistics

   **For Post-processing:**
   - Design algorithms that specifically target over-segmentation artifacts
   - Use contextual information (neighboring cells, typical cell sizes)

   **For Machine Learning approaches:**
   - Keep models simple and interpretable
   - Focus on unsupervised methods that don't require training data

   **For Hybrid approaches:**
   - Combine complementary methods that address different failure modes
   - Implement intelligent fusion strategies

6. **Quality Assurance**
   - Each solution must be self-contained and fully functional
   - Test edge cases (very dark/light images, dense cell regions)
   - Ensure graceful degradation when assumptions don't hold

7. **Documentation Requirements**
   - Clear explanation of the theoretical basis for each approach
   - Honest assessment of limitations and potential failure cases
   - Suggestions for further improvements or parameter tuning

8. **Innovation Encouragement**
   - Think beyond standard OpenCV operations
   - Consider custom algorithms tailored to Ki67 staining characteristics
   - Explore creative combinations of existing techniques