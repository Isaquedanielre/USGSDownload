# usgs_download

Name                 : USGSDownload
Description          : Landsat Data download from earth explorer
Date                 : April, 2016
copyright            : (C) 2016 by Lucas Lamounier
email                : lucasls.oas@gmail.com

Basic usage
****************************************************************************
if you do not register, access the site https://ers.cr.usgs.gov/register/ and make the register

    scene = SceneInfo('LC82280612016108LGN00')
    usgs = USGSDownload(scene, USER, PASSWORD)
    usgs.download(bands=['BQA', 4, 5, 6], download_dir=/home/user/landsat)

