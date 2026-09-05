+++
title = "Data Release 4"
draft = false
type = "datarelease_ms_uncover_color"
URL = "/DR4.html"

+++

<h1 class="othersurvey">The <img src="../images/UNCOVER_logo_white.png" alt="MegaScience"/> & <img src="../images/megascience_white.png" alt="MegaScience"/> Surveys: </h1>



<h2 id="DR4">Data Release 4</h2>

<div class="subnav">
    <ul>
        <li><a href="#Spectra">Reduced spectra + catalogs</a></li>
        <li><a href="#LensingMaps">Lensing maps</a></li>
        <li><a href="#UpdatedLensMag">Lensing Magnifications</a></li>
        <li><a href="#SPSCatalogs">Stellar population catalogs</a></li>
        <!-- <li><a href="#PhotometricCatalogs">Photometric catalogs</a></li> -->
        <!-- <li><a href="#Mosaics">Mosaics</a></li> -->
    </ul>
</div>



<hr>
<!-- Spectra+Catalogs-->
<h3 class="minor" id="Spectra">First reduced spectra + redshift catalog release</h3>


<h4 class="minor date">December 5, 2024</h4>

<p style="margin-bottom: 1rem">
    <b><i>UPDATE:</i></b> The release has been improved to include additional 
    information that may be beneficial to users in this version (DR4.1). 
    The redshift catalog now includes 
    an advisory flag regarding potential issues with the 
    local background subtraction scheme adopted in this release. 
    <!--  -->
    <i>(<b>Note:</b> this is only an advisory flag to alert users to inspect the 
    2D spectrum and evaluate if this background issue could impact their planned analysis.
    The robustness of measured redshifts is not impacted by this flag.)</i>
    <!--  -->
    Additionally, a new catalog containing coordinates (in RA/Dec) for 
    the slit shutters of each target, for all masks, has been added. 
    <!--  -->
    Please refer to the 
    <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
    for further details. 
    The links for the updated catalogs now point to the DR4.1 files. 
</p>


<h4 class="minor date">August 7, 2024</h4>

<p style="margin-bottom: 1rem">
    The initial release of the UNCOVER reduced spectra and redshift catalogs 
    are now available as part of DR4! 
    The DR4 Spectra release includes all successfully reduced observations 
    taken in July/Aug 2023, with PRISM spectra from 0.6-5µm of 553 objects.  
    For this initial release, the redshift catalog includes only 
    objects with secure or solid (<code>flag_zspec_qual=3</code> or 
    <code>=2</code>) redshift fits (409 objects). 
</p>

<p style="margin-bottom: 1rem">
    All catalogs are based on F444W PSF-matched imaging, 
    where the bright cluster galaxies and ICL have been modeled and subtracted. 
    Detection was performed on a noise-equalized long-wavelength image 
    (F277W+F356W+F444W). 
    <!--  -->
</p>
<p style="margin-bottom: 1rem">
    In addition to the spectroscopic redshift catalog, 
    we release a catalog of line fluxes that are estimated from 
    each object's <a href="https://github.com/gbrammer/msaexp"><code>msaexp</code></a> 
    redshift best-fit, and 
    magnifications calculated from the updated <a href="#LensingMaps">v2.0</a> lensing 
    model using the new spec-zs. 
</p>
<p style="margin-bottom: 1rem">
    For full details, please see the 
    <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a> 
    and the <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">UNCOVER first spectra release paper</a>.
</p>
<p style="margin-bottom: 1.5rem">
    Please cite <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">Price et al. 2025</a>
    when using any of the following data products, 
    and <a href="https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.4568F/abstract">Furtak et al. 2023</a>  
    when using the MSA target magnification catalog. 
</p>
<table style="margin-bottom:0; width:100%;">
    <tr class='mainhead'>
        <th style="width:25%">Catalog</th>
        <th style="width:50%">Description</th>
        <th style="width:25%">Files</th>
    </tr>
    <tr>
        <td>Redshifts</td>
        <td>
            Spectroscopic redshift catalog of all 
            targeted objects, with quality flags
        </td>
        <td>         
            <!-- Catalog: -->
            <a href="https://drive.google.com/file/d/10E5tGzATWGz-3y7G0g9LfUPBHGxgqSjJ/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10BQOEvwzcazLkJFmH4EzNWlwY70xejYi/view?usp=drive_link">ASCII</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>
    <tr>
        <td>Line fluxes</td>
        <td>
            Line fluxes derived from <code>msaexp</code> redshift fits for 
            all targeted objects
        </td>
        <td>         
            <!-- Catalog: -->
            <a href="https://drive.google.com/file/d/1ojbDYoEWxrshzcTnyFS9VmdtKRGykXuJ/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1ojZExqQlJ_BjkoxNKSr6KFZxR0VspIyE/view?usp=drive_link">ASCII</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>    
    <tr>
        <td>MSA target magnifications</td>
        <td>
            <a href="#LensingMaps">v2.0</a> lensing magnifications for all MSA targets 
        </td>
        <td>         
            <!-- Catalog: -->
            <a href="https://drive.google.com/file/d/1o7BBgi4WEIbwgc2FO4QVMGfVv-XplLKI/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1mq4RDH5qewnEvLegZNnyKR5T8tT5GYb1/view?usp=drive_link">ASCII</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>     
    <tr style="border-bottom: 0;">
        <td>Slit coordinate catalog</td>
        <td>Coordinates of all targets' shutter corners (in RA/Dec) for each mask </td>
        <td>
            <!-- Catalog: -->
            <a href="https://drive.google.com/file/d/10Kr00rnBWQJTMW-yXSyUdi5nFu0c3jw4/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10MUcEHRB9Y5CVpsaJ4LSJ0NkMvHmdtV1/view?usp=drive_link">ASCII</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>
</table>

<table style="margin-bottom:0; width:100%;">
    <tr class='mainhead'>
        <th style="width:25%">Reduced spectra</th>
        <th style="width:50%">Description</th>
        <th style="width:25%">Files</th>
    </tr>
    <tr>
        <td><b>Default (recommended)</b></td>
        <td>Extracted 1D+2D spectra, & other extensions</td>
        <td>         
            <a href="https://drive.google.com/drive/folders/1OiGBRv7Vi9CXMyx_QqGexVvu6NEY1l5D?usp=drive_link">Folder</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>
    <tr style="border-bottom: 0;">
        <td>Phot cal</td>
        <td>Spectra calibrated to 0.32" diameter aperture 
            photometry using polynomial fit; 
            see README for recommended use cases
        </td>
        <td>         
            <a href="https://drive.google.com/drive/folders/1SpnDhzhxIZY3UB-UFsqeL16L-X8sxABp?usp=drive_link">Folder</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>
</table>
<table>
    <tr class='mainhead'>
        <th style="width:25%">Ancillary products</th>
        <th style="width:50%">Description</th>
        <th style="width:25%">Files</th>        
    </tr>
    <tr>
        <td>Redshift fits</td>
        <td><code>msaexp</code> redshift fitting files for best-fit</td>
        <td>        
            <a href="https://drive.google.com/drive/folders/1imJobDIPA4eEjy_87eDBFHr1IoMVC6fR?usp=drive_link">Folder</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a> 
        </td>
    </tr>   
    <tr>
        <td>Mask metadata</td>
        <td>Details regarding observed masks and targets</td>
        <td>        
            <a href="https://drive.google.com/drive/folders/15MVdWMh-8OHNcXAY3Nnii2n_d5EINb4I?usp=drive_link">Folder</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a> 
        </td>
    </tr>
</table>




<hr>
<!-- Lensing map release -->
<h3 class="minor" id="LensingMaps">Lens model updated release: v2.0</h3>
<h4 class="date">August 7, 2024</h4>
<h5>Authors: Lukas J. Furtak and Adi Zitrin</h5>

<p style="margin-bottom: 1rem">
    The UNCOVER strong lensing (SL) model 
    is a parametric SL model constructed 
    with the UNCOVER JWST data using a new (grid-free) analytic method by A. Zitrin.
</p>

<p style="margin-bottom: 1rem">
    In this model release (v2.0), we supply WCS-registered FITS maps 
    of the deflection field (in pixels), convergence, shear, 
    and the lensing potential normalized to Dds/Ds=1. 
    We also supply magnification maps for various source redshifts: 
    1, 2, 4, 6, 8, 10, 15 and 20. The lensing maps have a FoV of 7.6' x 7.6', 
    which covers the entire central UNCOVER field. 
    We provide maps for the best-fit model in two resolutions, 
    a high-resolution version in 0.04"/pix (JWST NIRCam resolution) 
    and a low-resolution version with 0.1"/pix.
</p>
<p style="margin-bottom: 1rem">
    Compared to the <a href="/DR1.html#LensingMaps">v1.1 models</a>, 
    we added 13 spectroscopic redshifts from JWST/NIRSpec MSA and JWST/NIRCam 
    grism observations, and 132 additional cluster members selected from 
    JWST/NIRCam imaging. The additional spectroscopic redshifts in particular 
    constrain the northern and north-western sub-structures that were 
    previously mostly constrained with photometric redshifts.
</p>


<p style="margin-bottom: 1rem">
    Please cite 
    <a href="https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.4568F/abstract">Furtak et al. 2023</a> 
    and <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">Price et al. 2025</a>
    when using any of the lensing maps provided here.
</p>

<p style="margin-bottom: 1.5rem">
    For any questions, please contact us at: <i>furtak [at] post.bgu.ac.il</i>
</p>

<table>
    <tr class='mainhead'>
        <th>UNCOVER lensing maps</th>
        <th>Files</th>
    </tr>
    <tr>
        <td>v2.0</td>
        <td>
            <a href="https://drive.google.com/drive/folders/1Y3CGDH9EfqrjCHZSwwx4SLFDvCV8pqlV?usp=drive_link">Folder</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10IGwetPxd06EFDTIzYXJIy8yip6iLdYa/view?usp=drive_link">README</a>
        </td>
    </tr>
    <tr>
        <td>All versions</td>
        <td>
            <a href="https://drive.google.com/drive/folders/1Lc7uveJr_ZNIcvAQYVfAeRF8Qr68D_5p?usp=drive_link">Top folder</a> 
        </td>
    </tr>
</table>



<hr>
<!-- Updated lensing magnifications for full UNCOVER catalog -->
<h3 class="minor" id="UpdatedLensMag">Updated Lensing Magnifications</h3>
<h4 class="minor date">August 7, 2024</h4>



<p style="margin-bottom: 1rem">
    We also release updated lensing magnifications the full UNCOVER photometric sample!  
    The lensing values are computed for each source 
    (from the <a href="DR3.html/#PhotometricCatalogs">SUPER photometric catalog</a>) 
    using the best-available redshift 
    (highest to lowest priority: UNCOVER MSA spec-z, literature spec-z, 
    and MegaScience+UNCOVER <code>eazy</code> phot-z). 
</p>
<p style="margin-bottom: 1rem">
    <b>Note that the IDs in this full-sample catalog are identical to the DR3 IDs.</b>
</p>
<p style="margin-bottom: 1rem">
    For full details, please see the 
    <a href="https://drive.google.com/file/d/1o6uidRd0G4lkrO6WrxPK7hkvp-ZbBnjI/view?usp=drive_link">README</a>. 
</p>
<p style="margin-bottom: 1.5rem">
    Please cite 
    <a href="https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.4568F/abstract">Furtak et al. 2023</a> (lens modeling), 
    <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">Price et al. 2025</a> (updated lens model & UNCOVER spec-zs), and 
    <a href="https://ui.adsabs.harvard.edu/abs/2024ApJ...976..101S/abstract">Suess et al. 2024</a> 
    & <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270....7W/abstract">Weaver et al. 2024</a> 
    (MegaScience+UNCOVER <code>eazy</code> phot-zs)
    when using the full-sample magnification catalog.
</p>
<table style="margin-bottom:0; width:100%;">
    <tr class='mainhead'>
        <th style="width:25%">Catalog</th>
        <th style="width:50%">Description</th>
        <th style="width:25%" >Files</th>        
    </tr>
    <tr>
        <td>SUPER magnifications</td>
        <td>
            <a href="#LensingMaps">v2.0</a> lensing magnifications for 
            all objects in the<br><a href="DR3.html#PhotometricCatalogs">DR3 MegaScience+UNCOVER SUPER catalog</a> 
            <br>(row matched, using the same IDs)
        </td>
        <td>         
            <a href="https://drive.google.com/file/d/1o7nnk6c1Gu3-x5vkQoolk8S6y22vVIiE/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1o7JqX2RYb-Dx1ewxNigfgoOn-u5moyq2/view?usp=drive_link">ASCII</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1o6uidRd0G4lkrO6WrxPK7hkvp-ZbBnjI/view?usp=drive_link">README</a>
        </td>
    </tr>
    <tr>
        <td>MSA target magnifications</td>
        <td>
            <a href="#LensingMaps">v2.0</a> lensing magnifications for all MSA targets (by <code>id_msa</code>); 
            see the <a href="#Spectra">spectroscopic release</a> description. 
        </td>
        <td>         
            <!-- Catalog: -->
            <a href="https://drive.google.com/file/d/1o7BBgi4WEIbwgc2FO4QVMGfVv-XplLKI/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1mq4RDH5qewnEvLegZNnyKR5T8tT5GYb1/view?usp=drive_link">ASCII</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/10Vu1M7p7LPr9Ol146EYE6Qk2fSlHKk7-/view?usp=drive_link">README</a>
        </td>
    </tr>
</table> 



<hr>
<!-- Stellar populations catalogs release -->
<h3 class="minor" id="SPSCatalogs">Updated stellar population catalogs release</h3>


<h4 class="minor date">February 13, 2025</h4>



<p style="margin-bottom: 1rem">
    The updated DR4 stellar population synthesis (SPS) catalog is based on the 
    "SUPER" DR3 photometric catalog, with optimally determined aperture sizes 
    per object. 
    The methodologies follow 
    <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270...12W/abstract">Wang et al. 2024</a>: 
    Modeling is performed with the Prospector inference framework 
    (<a href="https://ui.adsabs.harvard.edu/abs/2021ApJS..254...22J/abstract">Johnson et al. 2021</a>). 
    The modeling assumes a non-parametric, logarithmically-spaced SFH, as well 
    as a mass function prior, a Gaussian mass-metallicity prior, and a dynamic 
    SFH(M, z) prior from Prospector-β to optimize the photometric inference 
    over the wide parameter space covered by deep JWST surveys 
    (<a href="https://ui.adsabs.harvard.edu/abs/2023ApJ...944L..58W/abstract">Wang et al. 2023</a>). 
    A second catalog with fixed redshifts to spec-zs 
    (including the UNCOVER MSA spec-zs) is also available.
</p>
<!-- <p style="margin-bottom: 1rem"> -->
<p style="margin-bottom: 0.2rem">
    In summary, this date release incorporates the following updates:
</p>
<ul>
    <li>SED fitting is performed on the complete set of photometric data, which 
    includes broad-band data obtained from UNCOVER and medium-band data 
    obtained from MegaScience.</li>
    <li>Lens model v2.0 is used.</li>
    <li>An additional catalog, where the SEDs are fit with redshifts fixed to 
    the spectroscopic redshifts released in DR4 
    (<a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">Price et al. 2025</a>) 
    is included.</li>
</ul>
<p style="margin-bottom: 1rem">
    <b>Note that the IDs in the full-sample catalog are identical to the DR3 IDs.</b> 
    <br>The primary IDs in the spec-z catalog are the MSA IDs (please see the 
    <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a>). 
</p>
<p style="margin-bottom: 1rem">
    For full details, please see the 
    <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
    and the <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270...12W/abstract">catalog paper</a>.
</p>
<p style="margin-bottom: 1.5rem">
    Please cite <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270...12W/abstract">Wang et al. 2024</a>, 
    <!-- (SPS modeling methodology),  -->
    <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270....7W/abstract">Weaver et al. 2024</a>, 
    <a href="https://ui.adsabs.harvard.edu/abs/2024ApJ...976..101S/abstract">Suess et al. 2024</a>, 
    <!-- (UNCOVER & MegaScience photometry) -->
    and <a href="https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.4568F/abstract">Furtak et al. 2023</a> 
    <!-- (lens modeling methodology) -->
    when using any of the following data products, 
    and also 
    <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">Price et al. 2025</a> 
    <!-- (spec-z release) -->
    when using the catalogs adopting spec-zs. 
</p>
<!-- <table> -->
<table style="margin-bottom:0; ">
    <tr class="mainhead">
        <th style="width:22%">Product</th>
        <th style="width:50%">Description</th>
        <th style="width:20%">Files</th>        
    </tr>
    <tr class="double-row-border">
        <td>SPS catalog</td>
        <td>Stellar population catalog based on the DR3 SUPER photometric catalog 
            with optimally determined aperture sizes per object, 
            with the redshift inferred <u>simultaneously</u> from the photometric fit</td>
        <td>         
            <a href="https://drive.google.com/file/d/1AE1g_5m9PYnu2LtDEAgXOgxkguImy7jv/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a>
        </td>
    </tr> 
    <tr>
        <td>Quicklook notebook</td>
        <td>Jupyter notebook for plotting the maximum-likelihood SEDs, SFH percentiles, and posteriors</td>
        <td>        
            <a href="https://drive.google.com/file/d/1BatnxQfFvffe1sVtwmY7VOi4xkRIlPrz/view?usp=drive_link">Notebook</a> 
        </td>
    </tr>
    <tr>
        <td>Chains</td>
        <td>Posteriors (subset of 500) for the default SPS catalog</td>
        <td>        
            <a href="https://drive.google.com/file/d/1j0-QfKx26ZLZT0eeCGpRyCRcUWgBXMv_/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
    <tr>
        <td>SEDs</td>
        <td>Best-fit models for the default SPS catalog, for visualization purposes</td>
        <td>        
            <a href="https://drive.google.com/file/d/1JL0e3VM4NZRcJrcQ4aoyOR1AORO_-ng6/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
    <tr>
        <td>SFHs</td>
        <td>SFH percentiles for the default SPS catalog (in lookback time, Gyr)</td>
        <td>        
            <a href="https://drive.google.com/file/d/18gK5JFK0A-WCJ7T3r0h1amXPRCrfmorw/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
    <tr>
        <td>Chains, log SFR ratios</td>
        <td>SFH posteriors, quantified as temporal array of logSFR ratios (subset of 500)</td>
        <td>        
            <a href="https://drive.google.com/file/d/1f7aR8Wptqgjzvd-6bUPERGyDBllE6jTI/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
</table>
<table>
    <tr class="mainhead">
        <th style="width:22%">Product</th>
        <th style="width:50%">Description</th>
        <th style="width:20%">Files</th>          
    </tr>
    <tr class="double-row-border">
        <td>SPS catalog, spec-zs</td>
        <td>Stellar population catalog based on the DR3 SUPER photometric catalog 
            with optimally determined aperture sizes per object, redshifts fixed to 
            DR4 UNCOVER/MSA spec-zs</td>
        <td>         
            <a href="https://drive.google.com/file/d/1j32n3e7hX0iw5ZyGlVAbyIf4MmjM4RfS/view?usp=drive_link">FITS</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a>
        </td>
    </tr> 
    <tr>
        <td>Chains, zspec</td>
        <td>Posteriors (subset of 500) for the SPS catalog with fixed spec-z</td>
        <td>        
            <a href="https://drive.google.com/file/d/1amAhNd_LRbb8H0a-aMMvOpGJ4Fktemds/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
    <tr>
        <td>SEDs, zspec</td>
        <td>Best-fit models for the SPS catalog with fixed zspec, for visualization purposes</td>
        <td>        
            <a href="https://drive.google.com/file/d/1Aki1UYdVFbLGqPJMRVTxHG65yY8CQdzp/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
    <tr>
        <td>SFHs, zspec</td>
        <td>SFH percentiles for the SPS catalog with fixed zspec (in lookback time, Gyr)</td>
        <td>        
            <a href="https://drive.google.com/file/d/1o2nlVZClkAicJGNgJnA7aL5atLs_45sb/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
    <tr>
        <td>Chains, log SFR ratios, zspec</td>
        <td>SFH posteriors, quantified as temporal array of logSFR ratios (subset of 500), with fixed spec-z</td>
        <td>        
            <a href="https://drive.google.com/file/d/1amAhNd_LRbb8H0a-aMMvOpGJ4Fktemds/view?usp=drive_link">npz</a> &nbsp; &nbsp; 
            <a href="https://drive.google.com/file/d/1kkCsTJJ8tu2_IFW3a7gTHwpqXt_RJH6G/view?usp=drive_link">README</a> 
        </td>
    </tr>
</table>




<!-- <hr> -->
<!-- Photometric catalogs release -->
<!-- <h3 class="minor" id="PhotometricCatalogs">Photometric catalog release</h3>
<h4 class="minor date">August 7, 2024</h4>

<p style="margin-bottom: 1rem">
    This release includes updated DR4 photometric catalogs, 
    [FINAL DETAILS]. 
</p>
<p style="margin-bottom: 1rem">
    The DR4 Photometric catalog includes photometry from 
    the combined MegaScience+UNCOVER set of mosaics. 
    Included in the release are a "SUPER" catalog with photometry determined 
    from optimally-selected color apertures, identification of 
    stars and artifacts, and complete coverage of 
    all available JWST imaging over Abell 2744.
</p>
<p style="margin-bottom: 1rem">
    All catalogs are based on F444W PSF-matched imaging, 
    where the bright cluster galaxies and ICL have been modeled and subtracted. 
    Detection was performed on a noise-equalized long-wavelength image 
    (F277W+F356W+F444W). 
</p>
<p style="margin-bottom: 1rem">
    In addition to photometry, the catalogs contain basic photometric
    redshifts and rest-frame fluxes derived using EAZY, 
    ALMA fluxes from DUALZ (<a href="https://ui.adsabs.harvard.edu/abs/2025ApJS..278...45F/abstract">Fujimoto et al. 2025</a>) 
    where available, and lensing magnifications for each object based on the  
    <a href=#LensingMaps>v2.0 lensing maps</a>  
    (<a href="https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.4568F/abstract">Furtak et al. 2023</a>, 
    <a href="https://ui.adsabs.harvard.edu/abs/2025ApJ...982...51P/abstract">Price et al. 2025</a>). 
    <b>Note UNCOVER MSA spec-zs are not included in these catalogs,
    and the lensing magnifications in this catalog are based only 
    on phot-zs or previous literature spec-zs.</b> 
</p>
<p style="margin-bottom: 1rem">
    Also included in the release is a catalog of photometric redshifts derived using 
    Prospector-β 
    (<a href="https://ui.adsabs.harvard.edu/abs/2023ApJ...944L..58W/abstract">Wang et al 2023</a>).
</p>
<p style="margin-bottom: 1rem">
    For full details, please see the 
    <a href="URL">README</a> 
    and the <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270....7W/abstract">UNCOVER catalog paper</a>.
</p>
<p style="margin-bottom: 1.5rem">
    Please cite <a href="https://ui.adsabs.harvard.edu/abs/2024ApJ...976..101S/abstract">Suess et al. 2024</a> 
    and <a href="https://ui.adsabs.harvard.edu/abs/2024ApJS..270....7W/abstract">Weaver et al. 2024</a> 
    when using any of the following data products.
</p>
<table style="margin-bottom:0; width:100%;">
    <tr class='mainhead'>
        <th colspan="2">Photometric catalogs (including EAZY redshifts & restframe fluxes):</th>
        <th></th>
    </tr>
    <tr>
        <th style="width:25%">Flux aperture</th>
        <th style="width:45%">Intended use</th>
        <th style="width:30%">Files</th>
    </tr>
    <tr>
        <td>SUPER</td>
        <td>Recommended catalog with optimally determined aperture sizes per object</td>
        <td>         
            <a href="URL">Catalog</a> &nbsp; &nbsp; 
            <a href="URL">README</a>&nbsp; &nbsp; 
            <a href="URL">Regions</a>
        </td>
    </tr>
    <tr style="border-bottom: 0;">
        <td>0.32", 0.48", 0.70", 1.00", and 1.40"</td>
        <td>Single aperture catalogs for specific science applications 
            (e.g., small radius for compact, faint, high-z, or crowded sources; ...)
        </td>
        <td>
            <a href="URL">Catalogs</a> &nbsp; &nbsp; 
            <a href="URL">README</a> 
        </td>
    </tr>
</table>
<table style="margin-bottom:0; ">
    <tr class='mainhead'>
        <th style="width:70%">Prospector-β photometric redshifts:</th>
        <th style="width:30%"></th>
    </tr>
    <tr style="border-bottom: 0;">
        <td style="width:70%">Prospector-β photometric redshift catalog, 
            derived using the DR4 SUPER photometry catalog (and updated 
            magnifications).
        </td>
        <td style="width:30%">        
            <span style="color: rgba(229, 160, 90, 1);">Catalog [coming soon!]</span> &nbsp; &nbsp; 
            <span style="color: rgba(229, 160, 90, 1);">README [coming soon!]</span>
        </td>
    </tr>
</table>
<table>
    <tr class='mainhead'>
        <th style="width:25%">Ancillary products</th>
        <th style="width:45%">Description</th>
        <th style="width:30%">Files</th>        
    </tr>
    <tr>
        <td>LW detection</td>
        <td>Noise-equalized F277W+F356W+F444W detection image</td>
        <td>        
            <a href="URL">Image</a> &nbsp; &nbsp; 
            <a href="URL">Segmap</a> &nbsp; &nbsp; 
            <a href="URL">Regions</a> 
        </td>
    </tr>
    <tr>
        <td>Bright cluster galaxy (bCG) modeling</td>
        <td>bCG-subtracted mosaics (non-PSF-matched) 
            and bCG models</td>      
        <td>        
            <a href="URL">Images</a> &nbsp; &nbsp; 
            <a href="URL">README</a> &nbsp; &nbsp; 
            <a href="URL">Models</a> 
        </td>
    </tr>
    <tr>
        <td>PSFs</td>
        <td>Empirical PSFs for all filters</td>       
        <td>
            <a href="URL">FITS files</a>
        </td>
    </tr>
    <tr>
        <td>Kernels</td>  
        <td>Convolution kernels for PSF matching all filters to F444W</td>
        <td>
            <a href="URL">FITS files</a> 
        </td>
    </tr>
    <tr>
        <td>Filter translation</td>
        <td>EAZY zphot filter translation</td>
        <td>
            <a href="URL">zphot.translate</a>
        </td>
    </tr>
</table> -->




<!-- <hr> -->

<!-- Mosaic release -->

<!-- <h3 class="minor" id="Mosaics">NIRCam primary / NIRISS parallel mosaic release</h3>
<h4 class="minor date">April 22, 2024</h4>


<p style="margin-bottom: 1rem">
    <b style="color: rgba(229, 160, 90, 1);">DR4 does not update the UNCOVER mosaics, 
        but the links to the DR3 
    images are included here for ease of use.</b>

<p style="margin-bottom: 0.5rem">
    The reduced mosaics from the MegaScience observations are now available! 
    These include the remainder of the NIRCam broad- and medium-band filters 
    not yet observed over the extended Abell 2744 cluster: 
    the shortest two broad-band filters (F070W, F090W) and 
    11 medium-band filters (F140M, F162M, F182M, F210M, F250M, F300M, 
    F335M, F360M, F430M, F460M, F480M). 
    The parallel NIRISS imaging, overlapping the previous UNCOVER 
    imaging over the Hubble Frontier Fields parallel pointing, 
    includes two broad-band (F090W, F277W) and four medium band filters 
    (F140M, F158M, F430M, F480M). 
</p>

<p style="margin-bottom: 0.5rem">
    Updated UNCOVER mosaics, with the same WCS, are also available. 
    The short- (shorter than F250M) 
    and long-wavelength bands (F250M and longer) 
    use pixel scales of 0.02" and 0.04", respectively. 

    All filters have the same WCS, which is defined so that 
    the short-wavelength pixels 
    can be binned 2x2 to directly match the long-wavelength images. 
    Note that the primary footprint has been expanded from the UNCOVER DR2 
    mosaics to fully all available NIRCam imaging in Abell 2744. 

</p>
<p style="margin-bottom: 1rem">
    Additionally, mosaics of all existing <i>HST</i> data are provided, 
    produced with the same WCS and footprint and a 0.04" pixel scale. 
</p>

These mosaics include data from the following programs:
<ul style="margin-bottom: 1rem">
    <li><i>JWST</i>/NIRCAM: GO-4111 (MegaScience), 
        MAGNIF (GO-2883, PI: Sun), 
        ALT (GO-3516; PI: Naidu & Matthee), 
        GO-3538 (PI: Iani), 
        GO-2561 (UNCOVER), ERS-1324 (GLASS), DD-2767 </li>
    <li><i>JWST</i>/NIRISS: GO-4111 (MegaScience), 
        MAGNIF (GO-2883, PI: Sun), 
        ALT (GO-3516; PI: Naidu & Matthee), 
        GO-2561 (UNCOVER), ERS-1324 (GLASS)</li>
    <li><i>HST</i>/ACS: #11689 (PI: Dupke), #13386 (PI: Rodney), 
                #13495 (PI: Lotz / HFF), #13389 (PI: Siana), #15117 (PI: Steinhardt / BUFFALO),
                #17231 (PI: Treu) </li>
    <li><i>HST</i>/WFC3: #13495 (PI: Lotz / HFF), #15117 (PI: Steinhardt / BUFFALO)</li>
</ul>


<p style="margin-bottom: 1.5rem">
    Please cite <a href="https://ui.adsabs.harvard.edu/abs/2024ApJ...976..101S/abstract">Suess et al. 2024</a> 
    and <a href="https://ui.adsabs.harvard.edu/abs/2024ApJ...974...92B/abstract">Bezanson et al. 2024</a>
    if using these mosaics in any publication.
</p>


<p style="margin-bottom: 0;">
    <i>The following scripts can be used for batch downloads:
    <table class="plainlayouttable">
        <tr>
            <td class="minor">Linux/Unix:</td>
            <td class="minor">
                <a href="scripts/all_unix_DR3.sh">All files</a>,
                <a href="scripts/nircam_unix_DR3.sh">NIRCAM/Primary</a>,
                <a href="scripts/niriss_unix_DR3.sh">NIRISS/Parallel</a>,
                and the ancillary 
                <a href="scripts/hstacs_unix_DR3.sh">HST/ACS</a>, 
                <a href="scripts/hstwfc3_unix_DR3.sh">HST/WFC3</a> 
                mosaics
            </td>
        </tr>
        <tr>
            <td class="minor">MacOS:</td>
            <td class="minor">
                <a href="scripts/all_macos_DR3.sh">All files</a>,
                <a href="scripts/nircam_macos_DR3.sh">NIRCAM/Primary</a>,
                <a href="scripts/niriss_macos_DR3.sh">NIRISS/Parallel</a>,
                and the ancillary 
                <a href="scripts/hstacs_macos_DR3.sh">HST/ACS</a>, 
                <a href="scripts/hstwfc3_macos_DR3.sh">HST/WFC3</a> 
                mosaics
            </td>
        </tr>
    </table>
    </i>                    
</p>


<table>
    <tr>
        <th>NIRCAM Primary</th>
        <th>Files</th>
    </tr>
    <tr>
        <td>F070W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f070w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f070w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f070w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1Aljm8e9ONx5AYU_jtd_uGFglAubM_fD5/view?usp=sharing">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F090W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f090w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f090w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f090w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1tMJr6cSRDRSRpP2xCDqxjhwCmHMfpSoa/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F115W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f115w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f115w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f115w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1zwzFmLba26xmy804qRdUgu5USjg-2IMf/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F140M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f140m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f140m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f140m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/11gnGoCALCnauJ7cfBpWMcDKPTfiByBGs/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F150W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1KsxjCSGpxwgweK5ATn9vqgY_X36Xan8J/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F162M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150w2-f162m_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150w2-f162m_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150w2-f162m_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1aJTA6seONfg0ZBgsh_n-amQUNJgtpv3m/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F182M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f182m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f182m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f182m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/148sAR5uCKB1467hzk-WrYMkHSgaSIw6k/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F200W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f200w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f200w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f200w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1CPjv4mJUj-4Qn8nwWS0FEPEdBfhDxzV_/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F210M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f210m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f210m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f210m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1CheOW5TEb5DzaykSpru33dPhDXovknZ7/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F250M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f250m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f250m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f250m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1uusyUFvTlw0q3HcqqbkUoCapbhJB-Uj8/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F277W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f277w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f277w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f277w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1BYXUpGm84dVlcQ38AP-dDgcGySRxV29N/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F300M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f300m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f300m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f300m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/13Q-TMD-pRQlmFINBk-vE8xtNfiNk09KJ/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F335M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f335m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f335m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f335m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1uzwm-4BGAETwAnEsP1rSKUKoUymo6krf/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F356W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f356w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f356w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f356w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1oSl7LP_-XLCQ2F81-qto03IOZ_x7FJzf/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F360M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f360m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f360m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f360m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1y1a952L-P1vNU_e2rJj6uCnmjI8f4trW/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F410M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f410m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f410m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f410m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1U1_2p32k4KlQ8qkIM7N9RJ-vrcS4XXvz/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F430M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f430m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f430m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f430m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1qsx_td5Zi0g9iwJbYRxZRJOI4fi1VZex/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F444W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f444w-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f444w-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f444w-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1TyZGsMbzjYkT_3iVPiB666NHuDzKkuTX/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F460M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f460m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f460m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f460m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1qRGd7P4gl5DUUwYoxJAQxDc4fHPYJg68/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <td>F480M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f480m-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f480m-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f480m-clear_wcs.csv">Frame WCSs</a> &nbsp; &nbsp;
            <a href="https://drive.google.com/file/d/1Rq8Bqi6RSTRA-MdCNFbWmogQ0hh9DzVQ/view?usp=drive_link">bCG-subtracted</a>
        </td>
    </tr>
    <tr>
        <th>NIRISS Parallel</th>
        <th>Files</th>
    </tr>
    <tr>
        <td>F090W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f090wn-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f090wn-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f090wn-clear_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F115W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f115wn-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f115wn-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f115wn-clear_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>    
    <tr>
        <td>F140M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f140mn-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f140mn-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f140mn-clear_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F150W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150wn-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150wn-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f150wn-clear_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F158M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f158mn-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f158mn-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f158mn-clear_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F200W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f200wn-clear_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f200wn-clear_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-f200wn-clear_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>    
    <tr>
        <td>F277W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f277w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f277w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f277w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F356W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f356w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f356w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f356w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F430M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f430m_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f430m_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f430m_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F444W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f444w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f444w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f444w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F480M</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f480m_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f480m_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.2-clearp-f480m_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <th>Ancillary HST: ACS/UV, Optical</th>
        <th>Files</th>
    </tr>
    <tr>
        <td>F225W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f225wu_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f225wu_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f225wu_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F275W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f275wu_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f275wu_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f275wu_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F336W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f336wu_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f336wu_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f336wu_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F435W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f435w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f435w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f435w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F475W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f475w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f475w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f475w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F606W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f606w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f606w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f606w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F775W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f775w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f775w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f775w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F814W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f814w_drc_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f814w_drc_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.1-f814w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <th>Ancillary HST: WFC3/IR</th>
        <th>Files</th>
    </tr>
    <tr>
        <td>F105W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f105w_drz_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f105w_drz_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f105w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F125W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f125w_drz_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f125w_drz_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f125w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F140W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f140w_drz_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f140w_drz_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f140w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
    <tr>
        <td>F160W</td>
        <td>
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f160w_drz_sci.fits.gz">Mosaic</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f160w_drz_wht.fits.gz">Weight map</a> &nbsp; &nbsp; 
            <a href="https://s3.amazonaws.com/grizli-v2/JwstMosaics/v7/abell2744clu-grizli-v7.0-f160w_wcs.csv">Frame WCSs</a> 
        </td>
    </tr>
</table>
 -->
