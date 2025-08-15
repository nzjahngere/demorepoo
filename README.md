## Indian Flag Validator - Instructions

1. **Run the entire notebook** (Runtime > Run all)
2. Upload flag images using the "Choose Image File" button
3. Validation results will appear in the right panel

### Test with these sample cases:
- ✅ Correct Flat
- ✅ Correct Flat Alternate Resolution
- ❌ Incorrect aspect ratio (4:3)
- ❌ Chakra with 20 spokes

## Sample Outputs

### Sample Image 1: Correct Indian Flag
- ✅ All validations pass
- Overall score: 100/100

### Sample Image 2: Correct – Flat Alternate Resolution
- ❌ Ashoka Chakra spokes count fails
- Overall score: 100/100

### Sample Image 3: Wrong Aspect Ratio (4:3)
- ✅ Aspect ratio fails (deviation 11%)
- Overall score: 80/100

### Test 4: Missing Ashoka Chakra
- ❌ Ashoka Chakra spokes count fails
- Overall score: 100/100
