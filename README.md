# Data for using migrationR

To run Hetero-occurrence Species Distribution Models (HOSDMs), data of environmental variables are needed.

The compressed file Env.zip (295 MB) is a RasterBrick (a .grd file accompanied by a corresponding .gri file, 2.4 GB) with 12 environmental variables. This dataset covers the geographical area within the latitude and longitude range of 28-30° and 115-117°, encompassing the entire Poyang Lake region. The resolution of the dataset is 30 meters. The variables are: (1). Land cover dataset comprising nine distinct land cover categories, such as croplands and water bodies (Gong et al. 2013). (2). DEM, the Terra Advanced Spaceborne Thermal Emission and Reflection Radiometer (ASTER) Global Digital Elevation Model (GDEM) Version 3 (ASTGTM) (Polidori and El Hage 2020). (3-6). Bio_1, Bio_4, Bio_12, and Bio_15 from the set of 19 climate variables (Fick and Hijmans 2017), which represent mean and variance of temperature and precipitation. (7). The Human Footprint Index (Sanderson et al. 2002). (8-10). Solar radiation data for January, wind speed data for January, and water vapor pressure data for January (Hijmans et al. 2005). The original resolution of layers 3-10 was 1 kilometer, which we resampled to 30 meters for consistency using the function projectRaster in the raster package (Hijmans et al. 2015). (11-12). One layer for longitude and one layer for latitude with the same extent and resolution.

# References

Fick, S. E., and R. J. Hijmans. 2017. WorldClim 2: new 1km spatial resolution climate surfaces for global land areas. International Journal of Climatology 37:4302–4315.

Gong, P., J. Wang, L. Yu, Y. Zhao, Y. Zhao, L. Liang, Z. Niu, X. Huang, H. Fu, S. Liu, C. Li, X. Li, W. Fu, C. Liu, Y. Xu, X. Wang, Q. Cheng, L. Hu, W. Yao, H. Zhang, P. Zhu, Z. Zhao, H. Zhang, Y. Zheng, L. Ji, Y. Zhang, H. Chen, A. Yan, J. Guo, L. Yu, L. Wang, X. Liu, T. Shi, M. Zhu, Y. Chen, G. Yang, P. Tang, B. Xu, C. Giri, N. Clinton, Z. Zhu, J. Chen, and J. Chen. 2013. Finer resolution observation and monitoring of global land cover: first mapping results with Landsat TM and ETM+ data. International Journal of Remote Sensing 34:2607-2654.

Hijmans, R. J., S. E. Cameron, J. L. Parra, P. G. Jones, and A. Jarvis. 2005. Very high resolution interpolated climate surfaces for global land areas. International Journal of Climatology 25:1965–1978.

Hijmans, R. J., J. Van Etten, J. Cheng, M. Mattiuzzi, M. Sumner, J. A. Greenberg, O. P. Lamigueiro, A. Bevan, E. B. Racine, and A. Shortridge. 2015. Package ‘raster’. R package 734:473.

Polidori, L., and M. El Hage. 2020. Digital elevation model quality assessment methods: A critical review. Remote sensing 12:3522.

Sanderson, E. W., M. Jaiteh, M. A. Levy, K. H. Redford, A. V. Wannebo, and G. Woolmer. 2002. The Human Footprint and the Last of the Wild. Bioscience 52:891–904.
