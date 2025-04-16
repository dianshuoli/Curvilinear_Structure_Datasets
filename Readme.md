
# Curvilinear Structure Dataset (CSD-8)

## Dataset Description
A collection of 8-class natural curvilinear structures with paired annotations.
**Two versions available**:
- 🖼️ **Full-resolution**: Original high-quality images (max dimension 5000px+)
- ⚡ **1k-version**: Resized to 1000px in length (aspect-ratio preserved) using nearest-neighbor interpolation.

**Recommended usage**:
✅ Use **1k-version** for all training/testing workflows
✅ Reserve full-resolution only for visual inspection

> **Note**: All annotations (segmentation/centerline) are pre-scaled to match their respective image versions.

**Total Images**: 800+ (≥100 per category)
**Data Types**:
- Original Images (`.jpg`or `.JPG`)
- Pixel-level Masks (`.png`)
- Centerline Masks (`.png`)

## Class Categories
1. `branch`
2. `crack`
3. `floor`
4. `leaf`
5. `scratch`
6. `soil`
7. `wire`
8. `tyre`

## U-Net Segmentation Performance
| Category   | F1 Score | Precision | Recall | Quality | Correctness | Completeness |
|------------|----------|-----------|--------|---------|-------------|--------------|
| branch     | 72.35    | 72.37     | 76.02  | 24.21   | 38.90       | 39.08        |
| crack      | 57.39    | 59.54     | 67.53  | 18.97   | 30.60       | 33.81        |
| floor      | 52.11    | 63.42     | 50.65  | 23.77   | 43.13       | 34.29        |
| leaf       | 47.90    | 56.49     | 43.50  | 9.82    | 22.63       | 14.87        |
| scratch    | 33.10    | 57.75     | 28.19  | 9.72    | 27.30       | 13.62        |
| soil       | 71.48    | 71.19     | 73.11  | 18.56   | 32.28       | 30.55        |
| tyre       | 47.10    | 72.10     | 38.46  | 17.70   | 36.90       | 25.75        |
| wire       | 51.94    | 51.32     | 58.04  | 19.82   | 30.77       | 32.00        |

**Average F1 Score across all categories**: 54.17

## Data Splits
| Split     | Percentage | Selection Method                 |
| --------- | ---------- | -------------------------------- |
| **Train** | 70%        | First 70% per class (rounded up) |
| **Test**  | 30%        | Remaining images                 |

## Annotation Details
- **Segmentation Masks**: Binary PNG (0=background, 255=foreground)
- **Centerline Masks**: 1-pixel wide skeletons (0=background, 255=centerline)

## Download
**Cloud Storage**:
[Google Drive](https://drive.google.com/file/d/1_5hR0yypZDDXgjg23OXcFze6KSbQWJlL/view?usp=sharing)

**Compressed Size**: ~3.5GB

## Usage License
- **Citation**:
```bibtex
@dataset{csd8-2025,
  title={CSD-8: Curvilinear Structure Dataset with Multi-level Annotations},
  author={Dianshuo Li},
  year={2025},
  version={1.0}
}
```
