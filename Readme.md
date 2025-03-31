# Curvilinear Structure Dataset (CSD-8)

## Dataset Description
A collection of 8-class natural curvilinear structures with paired annotations.  
**Two versions available**:  
- 🖼️ **Full-resolution**: Original high-quality images (max dimension 5000px+)  
- ⚡ **1k-version**: Resized to 1000px  in length (aspect-ratio preserved) using nearest-neighbor interpolation. 

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
[Google Drive](https://drive.google.com/file/d/1oHZHODyz3XA_hSuVmNnEYTk5-ALRCf7A/view?usp=sharing)

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

