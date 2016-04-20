# USGSDownload

Name                 : USGSDownload
Description          : Landsat Data download from earth explorer
Date                 : April, 2016
copyright            : (C) 2016 by Lucas Lamounier
email                : lucasls.oas@gmail.com

Instalation
****************************************************************************
pip install USGSDownload


Basic usage
****************************************************************************
if you do not register, access the site https://ers.cr.usgs.gov/register/ and make the register
    
    from usgsdownload.usgs import SceneInfo, USGSDownload
    
    scene = SceneInfo('LC82280612016108LGN00')
    usgs = USGSDownload(scene, user='your user', password='secret password')
    usgs.download(download_dir='/home/user/landsat')
    
    # Note: if not specified download_dir the files are sent to the user's home folder in landsat

