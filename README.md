# Project-1
基于像元的多时相遥感影像植被变化检测方法研究

#include"gdal_priv.h"
#include<"cpl_conv.h" // for CPLMalloc()

int main()
{
    GDALDataset  *poDataset;

    GDALAllRegister();

    poDataset = (GDALDataset *) GDALOpen( pszFilename, GA_ReadOnly );
    if( poDataset == NULL )
    {
        ...;
    }
