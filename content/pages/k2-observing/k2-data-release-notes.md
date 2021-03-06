Title: K2 Data Release Notes
Save_as: k2-data-release-notes.html

[TOC]

This page details the key features of the K2 data releases,
including a description of technical issues relevant to
the scientific exploitation of the data.


<hr>

# K2 Campaign 5

## At a glance

<div class="col-lg-5">

    <b><i>Pointing</i></b>
    <ul>
        <li>RA: 130.1576478 degrees</li>
        <li>Dec: 16.8296140 degrees</li>
        <li>Roll: 166.0591297 degrees</li>
    </ul>

    <b><i>Targets</i></b>
    <ul>
        <li>25,850 in long cadence (LC)</li>
        <li>204 in short cadence (SC)</li>
        <li>Several custom targets (see below)</li>
    </ul>

    <b><i>Full Frame Images (FFI)</i></b>
    <ul>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2015127093352-c05_ffi-cal.fits">ktwo2015127093352-c05_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2015170131810-c05_ffi-cal.fits">ktwo2015170131810-c05_ffi-cal.fits</a></li>
    </ul>

    <b><i>First cadence</i></b>
    <ul>
        <li>Time: 2015-04-27 02:18:11.949 UTC</li>
        <li>Long Cadence Number: 107552</li>
        <li>Short Cadence Number: 3215020</li>
    </ul>

    <b><i>Last cadence</i></b>
    <ul>
        <li>Time: 2015-07-10 22:39:43.571 UTC</li>
        <li>Long Cadence Number: 111214</li>
        <li>Short Cadence Number: 3324909</li>
    </ul>

</div>

<div class="col-lg-7">

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Schematic of Kepler's C5 field-of-view with observed targets shown with purple dots.</i>
        </div>
        <a href="images/campaign_selected/C5_selected.png">
            <img src="images/campaign_selected/C5_selected.png" class="img-responsive" alt="C5 field-of-view with selected targets">
        </a>
    </div>

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Distribution of the Kepler magnitudes of observed targets in C5. All targets are chosen by Guest Observers. The bimodality is due to how the largest <a href="k2-approved-programs.html#campaign-5">Guest Observer programs</a> were selected.</i>
        </div>
        <a href="images/release-notes/c5/C5LcMagDistribution.png">
            <img src="images/release-notes/c5/C5LcMagDistribution.png" class="img-responsive" alt="Distribution of the Kepler magnitudes of observed targets in C5.">
        </a>
    </div>

</div>

## Features and events

<br>
***M67***

The open cluster M67 was observed by collecting a 400x400 region of sky near the core of the cluster in modules 6.1 and 6.2. See the image below. These data are grouped into 72 custom apertures, each with a 50x50 pixel mask or smaller. Their data are listed by custom aperture number at the MAST in the range 200008644--200008715.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: The tiling of the M67 open cluster is shown in green on mod.outs 6.1 and 6.2 of C5.</i>
    </div>
    <a href="images/release-notes/c5/M67Tiling.png">
        <img src="images/release-notes/c5/M67Tiling.png" class="img-responsive" alt="The tiling of the M67 open cluster is shown in green on mod.outs 6.1 and 6.2 of C5.">
    </a>
</div>

<br>
***Trans-Neptunian Object***

The Trans-Neptunian Object TNO (126154) 2001 YH140 was observed in Campaign 5 by creating 565 1 x n pixel target definitions (where n ranges from 4 to 21) that cover the path of the TNO. The custom aperture numbers range from 200008716 to 200009280.

<br>
***Noted Data Anomalies***

Approximately 55.5 days after the start of C5, we note a small (~4000 electrons per cadence) increase in the median dark level that lasts approximately a day. The event is likely caused by a Coronal Mass Ejection, and its size is small compared to other normal variations seen in the dark level. This change in dark level is part of the normal calibration process that occurs in the CAL module.

One Argabrightening event was seen in the observed background level approximately 38 days into the campaign and affects a majority of the channels. This event is flagged on bit 13 in the QUALITY column of the light curve and target pixel files for those targets on the affected channels.

<br>
***Light Curve Quality***

The dominant systematic present in K2 simple aperture photometry light curves is a sawtooth shape that is due to the roll of the spacecraft approximately every 6 hours. The PDC module of the Kepler Pipeline uses Principle Component Analysis to remove this signal in addition to other systematics. Below, we examine observed noise levels in the PDC light curves for C5, Data Release 7.

<a href="images/release-notes/c5/K2-C05_CDPP_Summary.txt">Table giving 6.5-hr CDPP as a function of magnitude.</a>

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: CDPP measured for all targets as a function of Kepler magnitude. Dim targets have poorer overall photometric precision than bright targets, but can look better because the residual sawtooth falls below the noise floor. The saturated targets tend to have the lowest CDPP, but often show a residual sawtooth. Also, the photometric precision is generally better near the center of the focal plane where the variations in roll angle produce less pixel motion. All cadences coincident with a definite thruster firing are gapped.</i>
    </div>
    <a href="images/release-notes/c5/K2-C05_logg_CDPP_vs_model.png">
        <img src="images/release-notes/c5/K2-C05_logg_CDPP_vs_model.png" class="img-responsive" alt="CDPP measured for all targets as a function of Kepler magnitude.">
    </a>
</div>


## Release History

The following is the data release history for this campaign. Follow the link for information about some of the features of the software used to reduce and export these data. There will be a new entry each time the data is released by the mission.

* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr7">Data Release 7</a>

<hr>



# K2 Campaign 4

## At a glance

<div class="col-lg-5">

    <b><i>Pointing</i></b>
    <ul>
        <li>RA: 59.0759116 degrees</li>
        <li>Dec: 18.6605794 degrees</li>
        <li>Roll: -167.6992793 degrees</li>
    </ul>

    <b><i>Targets</i></b>
    <ul>
        <li>15,853 in long cadence (LC)</li>
        <li>122 in short cadence (SC)</li>
        <li>Several custom targets (see below)</li>
    </ul>

    <b><i>Full Frame Images (FFI)</i></b>
    <ul>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2015051131033-c04_ffi-cal.fits">ktwo2015051131033-c04_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2015092174954-c04_ffi-cal.fits">ktwo2015092174954-c04_ffi-cal.fits</a></li>
    </ul>

    <b><i>First cadence</i></b>
    <ul>
        <li>Time: 2015-02-08 06:50:09.177 UTC</li>
        <li>Long Cadence Number: 103744</li>
        <li>Short Cadence Number: 2976430</li>
    </ul>

    <b><i>Last cadence</i></b>
    <ul>
        <li>Time: 2015-04-20 04:32:47.045 UTC</li>
        <li>Long Cadence Number: 107213</li>
        <li>Short Cadence Number: 3078009</li>
    </ul>

</div>

<div class="col-lg-7">

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: C4 field-of-view with selected targets shown as purple dots.</i>
        </div>
        <a href="images/campaign_selected/C4_selected.png">
            <img src="images/campaign_selected/C4_selected.png" class="img-responsive" alt="C4 field-of-view with selected targets">
        </a>
    </div>

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Distribution of the Kepler magnitudes of observed targets in C4. All targets are chosen by Guest Observers. The bimodality is due to how the largest Guest Observer programs were selected for C4.</i>
        </div>
        <a href="images/release-notes/c4/C4_lcDistribution.png">
            <img src="images/release-notes/c4/C4_lcDistribution.png" class="img-responsive" alt="Distribution of the Kepler magnitudes of observed targets in C4.">
        </a>
    </div>

</div>

## Features and events

<br>
***Pleiades and Hyades***

One Director's Discretionary Target program (GO4901, PI:White) was approved in Campaign 4 which observes the nine 3–5 mag B-stars and red giants in the Pleiades and Hyades open clusters. The targets were observed using circular pixel masks (20 pixels in radius) that cover the wings of the PSF but not the entire saturation bleed.

The two stars in the Hyades are γ Tau and δ1 Tau. The seven stars in the Pleiades are: Alcyone (η Tau), Atlas (27 Tau), Electra (17 Tau), Maia (20 Tau), Merope (23 Tau), Taygeta (19 Tau) and Pleione (28 Tau). These stars are all listed in the EPIC; however, their data are listed by custom aperture number at the MAST in the range 200007765--200007773.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: The Pleiades open cluster as seen on module 15 of the K2 C4 FFI.</i>
    </div>
    <a href="images/release-notes/c4/c4-pleiades-k2-1579.png">
        <img src="images/release-notes/c4/c4-pleiades-k2-1579.png" class="img-responsive" alt="The Pleiades open cluster as seen on module 15 of the K2 C4 FFI.">
    </a>
</div>

<br>
***Trans-Neptunian Object***

The Trans-Neptunian Object 2002 KY14 was observed in Campaign 4 by creating 1340 masks that cover the path of the TNO. The custom aperture numbers range from 200006425 to 200007764. These observations were taken as part of Guest Observer program GO4110 (PI:Schwamb).

<br>
***Background Residuals near Pleiades***

Background removal for channels near the Pleiades has larger than normal residuals. These large residuals occur on mod.outs 10.3 and 15.1 through 15.4 due to the background on these channels being dominated by dust clouds near the Pleiades. The rich spatial structure of the Pleiades' dust clouds is poorly captured by the low order (≤ 4) polynomial model used to fit the background flux, with the best fit for these channels being given by a constant. This fit is done for every cadence, and the result is higher than normal background residuals, with residuals as large as 7 times the standard deviation of the background pixel values. (Normal residuals are typically less than the background standard deviation.)

We recommend caution when using light curves or the background model on these channels. Note that the FLUX column of the target pixel files contains calibrated pixels with the background subtracted. The amount of background that was subtracted per pixel can be found in the <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr5">FLUX_BKG column</a> and restored, if desired.

Local background estimates per star may produce higher-quality results. The change in the constant background level on these channels over time is in family with the median background change on other channels

<br>
***Lightcurves Created with Non-Optimal Apertures***

Due to an incompatibility between K2 roll motion and the determination of photometric optimal apertures, some light curves may be based on apertures that are too small and therefore have more noise than necessary. In particular, there are 887 stellar targets that are particularly suspect; they are listed <a href="http://keplerscience.arc.nasa.gov/K2/K2drn/C4/C4_reduced_ap_targets.txt">here</a>. The brighter targets in this set may have correct optimal apertures, but stars with Kp > 13 have been shown to have lower photometric precision than non-suspect stars of similar brightness.

<br>
***Stars Show Lower Than Expected Flux***

The comparison of the measured flux to the flux based on their Kepler magnitudes in the EPIC catalog shows that ≈3,752 stars (23.8% of all stellar targets) are too bright by about a magnitude. The EPIC catalog field Kepflag gives the provenance of the Kepler magnitude estimate by listing the catalog magnitudes used to estimate the Kepler magnitude. Stars with Kepflag = “JHK” or “J” have Kepler magnitudes that are generally overestimated. These stars appear at all magnitudes, but predominantly have EPIC Kepler magnitudes dimmer than 14. The optimal apertures used to generate light curves for these “JHK” or “J” targets may be larger than optimal, reducing their photometric precision.

<div class="thumbnail" style="width: 100%;">
    <div class="caption">
        <i>Figure: histograms of the relative flux for C4 stellar targets. Left: the relative flux distribution of stellar targets with EPIC Kepflag values of “gri” or “BV”, showing that their measured flux is consistent with the expected flux. Right: the relative flux distribution of stellar targets with EPIC Kepflag values of “JHK” or “J”, showing that the observed flux is less than half the expected flux.</i>
    </div>
    <a href="images/release-notes/c4/lowfluxJband.png">
        <img src="images/release-notes/c4/lowfluxJband.png" class="img-responsive" alt="histograms of the relative flux for C4 stellar targets">
    </a>
</div>

<br>
***Several Stars Show Higher Than Expected Flux***

There is a group of target stars whose measured flux is more than twice that expected from their EPIC Kepler magnitudes. The figure below shows that these stars fall into spatial groups that are aligned with RA and Dec, rather than focal plane coordinates, strongly indicating that the cause of this anomaly is catalog error. The source of this error is presently unknown and is not correlated with Kepflag values. The optimal apertures used to generate light curves for these targets may be smaller than optimal, reducing their photometric precision.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: all C4 target stars plotted in celestial coordinates, colored by their Kepler magnitude inferred from their observed flux minus their Kepler magnitude from the EPIC catalog. There are two square-like regions and a line of blue markers, indicating stars whose inferred Kepler magnitude is about a magnitude smaller than their catalog magnitude, indicating that these stars are about a magnitude brighter than expected. The randomly distributed red markers are consistent with the population of Kepflag = “JHK” or “J” stars whose brightness is overestimated.</i>
    </div>
    <a href="images/release-notes/c4/C4radecKepMag.png">
        <img src="images/release-notes/c4/C4radecKepMag.png" class="img-responsive" alt="all C4 target stars plotted in celestial coordinates, colored by their Kepler magnitude inferred from their observed flux minus their Kepler magnitude from the EPIC catalog">
    </a>
</div>

<br>
***Stellar Targets with Negative Lightcurve Values***

Seventy-six stellar targets show negative flux values in their SAP_FLUX light curves, which is somewhat more than normally seen. Most of these are very dim, near background level targets at the edge of the focal plane where K2 roll has the largest impact, so it is not surprising that the roll causes negative flux values after background removal. The bright targets with negative flux values either have isolated negative flux outliers or are on the Pleiades channels, where there are large background residuals due to the constant background model on these channels, see above.

<br>
***Light Curve Quality***

The dominant systematic present in K2 simple aperture photometry light curves is a sawtooth shape that is due to the roll of the spacecraft approximately every 6 hours. The PDC module of the Kepler Pipeline uses Principle Component Analysis to remove this signal in addition to other systematics. Below, we examine observed trends and noise levels in the PDC light curves for C4, Data Release 6.

<a href="images/release-notes/c4/K2-C04_CDPP_Summary.txt">Table giving 6.5-hr CDPP as a function of magnitude.</a>

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: CDPP measured for all targets as a function of Kepler magnitude. Dim targets have poorer overall photometric precision than bright targets, but can look better because the residual sawtooth falls below the noise floor. The saturated targets tend to have the lowest CDPP, but often show a residual sawtooth. All cadences flagged as having definite thruster firings are gapped.</i>
    </div>
    <a href="images/release-notes/c4/c4-cdpp_kepMag_full_FOV.jpg">
        <img src="images/release-notes/c4/c4-cdpp_kepMag_full_FOV.jpg" class="img-responsive" alt="CDPP measured for all targets as a function of Kepler magnitude">
    </a>
</div>

The photometric precision is generally better near the center of the focal plane where the variations in roll angle produce less pixel motion:

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: 10th percentile CDPP of the 12th magnitude targets across the focal plane. The better performance near the center is evident.</i>
    </div>
    <a href="images/release-notes/c4/c4-10pcdpp_12th_mag.jpg">
        <img src="images/release-notes/c4/c4-10pcdpp_12th_mag.jpg" class="img-responsive" alt="10th percentile CDPP of the 12th magnitude targets across the focal plane">
    </a>
</div>


## Release History

The following is the data release history for this campaign. Follow the link for information about some of the features of the software used to reduce and export these data. There will be a new entry each time the data is released by the mission.

* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr6">Data Release 6</a>

<br>
***Notes Specific to Data Release 6***

These notes are issues specific to how the data was processed and are likely to change when the data are reprocessed.

*SC PDC Quality Flags*

The PDC quality flags were populated for some of the SC targets even though there are no SC PDC light curves. These flags are: manual exclude (bit 9), SPSD detected (bit 11), and impulsive outlier removed (bit 12). Users may simply ignore these flags.

<hr>







# K2 Campaign 3

## At a glance

<div class="col-lg-5">

    <b><i>Pointing</i></b>
    <ul>
        <li>RA: 336.66534641439 degrees</li>
        <li>Dec: -11.096663792177 degrees</li>
        <li>Roll: -158.494818065985 degrees</li>
    </ul>

    <b><i>Targets</i></b>
    <ul>
        <li>16,375 in long cadence (LC)</li>
        <li>55 in short cadence (SC)</li>
        <li>Several custom targets (see below)</li>
    </ul>

    <b><i>Full Frame Images (FFI)</i></b>
    <ul>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014331202630-c03_ffi-cal.fits">ktwo2014331202630-c03_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2015008010551-c03_ffi-cal.fits">ktwo2015008010551-c03_ffi-cal.fits</a></li>
    </ul>

    <b><i>First cadence</i></b>
    <ul>
        <li>Time: 2014-11-15 14:06:05.515 UTC</li>
        <li>Long Cadence Number: 99599</li>
        <li>Short Cadence Number: 2976430</li>
    </ul>

    <b><i>Last cadence</i></b>
    <ul>
        <li>Time: 2015-01-23 18:37:04.488 UTC</li>
        <li>Long Cadence Number: 107213</li>
        <li>Short Cadence Number: 3078009</li>
    </ul>

</div>

<div class="col-lg-7">

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Schematic of Kepler's C3 field-of-view with selected targets shown with purple dots. Note, the use of an incorrect rotation angle in software used by Guest Observers to select targets has resulted in obvious variations in target density across the focal plane.</i>
        </div>
        <a href="images/campaign_selected/C3_selected.png">
            <img src="images/campaign_selected/C3_selected.png" class="img-responsive" alt="C3 field-of-view with selected targets">
        </a>
    </div>

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Distribution of the Kepler magnitudes of observed targets in C3. The bimodality is due to the large Guest Observer programs selected for C3.</i>
        </div>
        <a href="images/release-notes/c3/magnitudeDist.png">
            <img src="images/release-notes/c3/magnitudeDist.png" class="img-responsive" alt="Distribution of the Kepler magnitudes of observed targets in C3.">
        </a>
    </div>

</div>

## Features and events

<br>
***Neptune***

Neptune moved across the field of view during C3 and K2 observed it in both long and short cadence. Short cadence data were obtained approximately 20 days either side of the stationary point of Neptune. See this time lapse <a href="https://www.youtube.com/watch?v=Tw-q3uM_5_0">movie</a> created by Jason Rowe that clearly shows Neptune and its moons, Titan and Nereid. The custom aperture numbers associated with Neptune are 200004468--200004923. These observations were taken as part of Guest Observer Programs GO3060 (PI:Rowe) and GO3057 (PI:Gaulme).

<br>
***Trans-Neptunian Object***

The Trans-Neptunian Object (225088) 2007 OR10 was observed with 2 masks and given custom aperture numbers 200004466 and 200004467. This target was observed as part of Guest Observer Program GO3053 (PI:Szabo).

<br>
***Highlights of Pipeline Improvements***

Campaign 3 (Data Release 5) data were the first K2 data processed with the SOC 9.3 pipeline. With this data release comes the higher-level data products. A detailed list of the pipeline developments that accompany this data release is listed on the <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr5">pipeline release page</a>. A few highlights are listed here:

* Quality flags now indicate which cadences were obtained during thruster firings.
* Background pixels were observerd and used to model the background level across the field of view. The calibrated pixels available in the target pixel files now have this background level removed.
* Simple Aperture Photometry (SAP_FLUX) and cotrended (PDCSAP_FLUX) light curves are available for long cadence data.
* The FFIs now contain a World Coordinate Solution.

<br>
***Light Curve Quality***

The dominant systematic present in K2 simple aperture photometry light curves is a sawtooth shape that is due to the roll of the spacecraft approximately every 6 hours. The PDC module of the Kepler Pipeline uses Principle Component Analysis to remove this signal in addition to other systematics. Below, we examine observed trends and noise levels in the PDC light curves for C3 (as measured using Data Release 5).

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: CDPP measured for all targets as a function of Kepler magnitude. Dim targets have poorer overall photometric precision than bright targets, but can look better because the residual sawtooth falls below the noise floor. The saturated targets tend to have the lowest CDPP but often show a residual sawtooth. All cadences flagged as having definite thruster firings are gapped.</i>
    </div>
    <a href="images/release-notes/c3/cdpp_vs_mag.png">
        <img src="images/release-notes/c3/cdpp_vs_mag.png" class="img-responsive" alt="CDPP measured for all targets as a function of Kepler magnitude">
    </a>
</div>

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: The photometric precision is generally better near the center of the focal plane where the variations in roll angle produce less pixel motion. This figure shows the 10th percentile CDPP of the 12th magnitude targets across the focal plane. The better performance near the center is evident.</i>
    </div>
    <a href="images/release-notes/c3/tenth_prctile_cdpp.png">
        <img src="images/release-notes/c3/tenth_prctile_cdpp.png" class="img-responsive" alt="10th percentile CDPP of the 12th magnitude targets across the focal plane">
    </a>
</div>

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: Tests show that stellar signals are well preserved out to a period of about 20 days. However sometimes the stellar signals are partially masked by residual sawtooth.
</i>
    </div>
    <a href="images/release-notes/c3/amplitude_study_1_6379_amp.png">
        <img src="images/release-notes/c3/amplitude_study_1_6379_amp.png" class="img-responsive" alt="Tests show that stellar signals are well preserved out to a period of about 20 days.">
    </a>
</div>

The short cadence light curves produced by the Kepler pipeline are inadequate for scientific research and are not being released at this time.


<br>
***Reduced Noise from Change in Bandwidth***

The change in bandwidth for pointing control (from 50 to 20 seconds) for C3 resulted in an increase in SNR for short cadence by a factor of roughly 4--9, with the larger improvement seen at the higher frequency end. Note, the bandwidth pointing control parameter was set to 10 seconds for the original Kepler Mission.

<br>
***Premature End***

Campaign 3 had a nominal duration of 80 days, but an actual duration of only 69.2 days. The campaign ended earlier than expected because the on-board storage filled up faster than anticipated due to unusually poor data compression.


## Release History

The following is the data release history for this campaign. Follow the link for information about some of the features of the software used to reduce and export these data. There will be a new entry each time the data is released by the mission.

* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr5">Data Release 5</a>

<hr>




# K2 Campaign 2

## At a glance

<div class="row">
<div class="col-lg-5">

    <b><i>Pointing</i></b>
    <ul>
        <li>RA: 246.1264 degrees</li>
        <li>Dec: -22.4473 degrees</li>
        <li>Roll: 171.2284 degrees</li>
    </ul>

    <b><i>Targets</i></b>
    <ul>
        <li>13401 in long cadence (LC)</li>
        <li>55 in short cadence (SC)</li>
        <li>Several custom targets (see below)</li>
    </ul>

    <b><i>Full Frame Images (FFI)</i></b>
    <ul>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014240042843-c02_ffi-cal.fits">ktwo2014240042843-c02_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014294030900-c02_ffi-cal.fits">ktwo2014294030900-c02_ffi-cal.fits</a></li>
    </ul>

    <b><i>First cadence</i></b>
    <ul>
        <li>Time: 2014-08-23 18:27:16 UTC</li>
        <li>Long Cadence Number: 95497</li>
        <li>Short Cadence Number: 2853370</li>
    </ul>

    <b><i>Last cadence</i></b>
    <ul>
        <li>Time: 2014-11-10 13:27:43 UTC</li>
        <li>Long Cadence Number: 99352</li>
        <li>Short Cadence Number: 2969049</li>
    </ul>

</div>

<div class="col-lg-7">

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Schematic of Kepler's C2 field-of-view with selected targets shown with purple dots.</i>
        </div>
        <a href="images/campaign_selected/C2_selected.png">
            <img src="images/campaign_selected/C2_selected.png" class="img-responsive" alt="C2 field-of-view with selected targets">
        </a>
    </div>

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Distribution of the Kepler magnitudes of observed targets in C2.</i>
        </div>
        <a href="images/release-notes/c2/C2_lc_kp.png">
            <img src="images/release-notes/c2/C2_lc_kp.png" class="img-responsive" alt="Distribution of the Kepler magnitudes of observed targets in C2.">
        </a>
    </div>

</div>

</div>

<div class="thumbnail">
    <div class="caption">
        <i>Figure: Full Frame Image Highlights</i>
    </div>
    <a href="images/release-notes/c2/K2-new-litho_2015.png">
        <img src="images/release-notes/c2/K2-new-litho_2015.png" class="img-responsive" alt="Campaign 2 Full Frame Image Highlights.">
    </a>
</div>


## Features and events

<br>
***Solar Activity***

During C2 Kepler experienced two energetic particle events of note, likely caused by solar activity. Both events affected all channels as can be seen in the dark current metric plot for the first 26 days of C2 (see below). The first was a broad peak lasting approximately from cadence 95924 -- 96335 (01-Sep-2014 11:51:30 Z [MJD: 56901.4941] to 09-Sep-2014 21:24:55 Z [MJD: 56909.8923]). The second was a stronger more-peaked event lasting approximately from cadence 96357 -- 96551 (10-Sep-2014 17:01:54 Z [56910.7096] to 14-Sep-2014 07:20:35 Z [56914.30596]). At the peak of the 10-Sep-2014 event the average dark current increased by a factor of ~7 over the quiescent level. The GOES x-ray flux plot for this time shows an increased x-ray flux at Earth, though we don't have an independent measure of the exact timing and magnitude at the location of Kepler. The impact to the data will be in the form of increased background level, and increased photometric noise. The impact will be largest for faint targets.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: Dark Current Metric plotted against time.</i>
    </div>
    <a href="images/release-notes/c2/c2_dark_current_metric.png">
        <img src="images/release-notes/c2/c2_dark_current_metric.png" class="img-responsive" alt="Dark Current Metric plotted against time.">
    </a>
</div>


<br>
***Mars***

Mars passed across the field of view between October 1 and October 23. See the figure below for a prediction of where Mars is on the focal plane during Campaign 2. Mars is a bright object which will saturate the CCD. Both its image and its reflection will likely contaminate nearby stars.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: Schematic of Kepler's C2 field of view (outlined in blue) with the positions of Mars shown as small red squares.</i>
    </div>
    <a href="images/release-notes/c2/f2-fov.png">
        <img src="images/release-notes/c2/f2-fov.png" class="img-responsive" alt="Schematic of Kepler's C2 field of view.">
    </a>
</div>


<br>
***LDE Flags***

During the latter half of C2 we experienced a large number of parity errors coming from the photometer's local detector electronics (LDE). These LDE parity errors can occur when a very bright star saturates and spills charge into the CCD serial readout register, causing an overflow at the input to the analog-to-digital converter. While these errors were rare in Kepler, the very bright stars, or solar system planets, on the focal plane in K2 can cause frequent parity errors. For example, stars on channels 67 and 75 were the source of many of the parity errors during C2. These errors do not affect the quality of data from pixels on the active focal plane.

The LDE parity error triggers a flag (bit 15, decimal=16384) in the QUALITY column of the target pixel files. This flag is set for the majority of cadences in the second half of the campaign.

<br>
***Attitude Tweak***

The pointing of the spacecraft was adjusted by approximately 10" on 2014-Aug-25, during cadence 95546, in order to ensure that the observed targets were centered in their masks. This event is flagged in the QUALITY column of the target pixel files with bit 1 (decimal=1). The data collected before the tweak may fall close to the edge of the collected mask and some of the object's flux may have been lost. Use these cadences with caution. 
Note, in Data Release 4, because of an operator error, the tweak is marked on the previous cadence, 95545.

<br>
***Two Globular Clusters***

The clusters M4 and M80 were observed in C2 by collecting all the pixels in 50x50 pixel masks. For M4, 16 of these custom apertures were collected and for M80, 4 were collected. The data files for M4 range from 200004370 -- 200004385. The data files for M80 range from 200004386 -- 200004389. The target pixel files may be found by using the Object Type field on the <a href="http://archive.stsci.edu/k2/data_search/search.php">MAST K2 data search</a> page.

<br>
***Two Solar System Objects***

Comet C/2013 A1 (Siding Spring) was observed by obtaining 2583, 25x1 pixel, masks across module.outputs 2.3, 4.2, 4.3 and 4.4. These apertures were given custom aperture numbers ranging from 200001787 -- 200004369. This target was observed as part of the Guest Observer Programs GO2030 (PI:Kelley) and GO2046 (PI:Lisse).

The Trans-Neptunian Object (268361) 2007 JJ43 was observed with 661, 11x1 or 13x1 pixel, masks and given custom aperture numbers ranging from 200001126 -- 200001786. This target was observed as part of Guest Observer Program GO2066 (PI:Schwamb).

These data sets can be found at the <a href="http://archive.stsci.edu/k2/data_search/search.php">MAST</a> by entering the Investigation ID on the search form. The Investigation ID matches the GO Program number that requested the observations.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: The path (shown in blue) of C/2013 A1 (Siding Spring) runs along modules 2 and 4 during C2.</i>
    </div>
    <a href="images/release-notes/c2/comet-path.png">
        <img src="images/release-notes/c2/comet-path.png" class="img-responsive" alt="Path of comet Siding Spring.">
    </a>
</div>

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: The masks selected for mod.out 17.3 are shown in green. Those selected to capture the TNO 2007 JJ43 are shown as a green arc in the lower right-hand corner of this figure.</i>
    </div>
    <a href="images/release-notes/c2/jj43_path.png">
        <img src="images/release-notes/c2/jj43_path.png" class="img-responsive" alt="Masks selected to capture TNO 2007 JJ43.">
    </a>
</div>

<br>
***EPIC Catalog Assignment***

For C2, a number of targets were proposed without <a href="https://archive.stsci.edu/k2/epic.pdf">EPIC</a> ID numbers. If a target was observed, it was either 1) given an EPIC ID number from the regular catalog if that target matched a target in the catalog, or 2) assigned a new EPIC ID. We created EPIC ID numbers for 69 targets, ranging from 210282492 -- 210282560.

## Release History

The following is the data release history for this campaign. Follow the link for information about some of the features of the software used to reduce and export these data. There will be a new entry each time the data is released by the mission.

* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr4">Data Release 4</a>

<hr>




# K2 Campaign 1

Campaign 1 (C1) is the first full length observing campaign for K2 where the targets were selected by peer review.

## At a glance

<div class="row">
<div class="col-lg-5">

    <b><i>Pointing</i></b>
    <ul>
        <li>RA: 173.939610 degrees</li>
        <li>Dec: 1.4172989 degrees</li>
        <li>Roll: 157.641206 degrees</li>
    </ul>

    <b><i>Full Frame Images (FFI)</i></b>
    <ul>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014157010055-c01_ffi-cal.fits">ktwo2014157010055-c01_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014203150825-c01_ffi-cal.fits">ktwo2014203150825-c01_ffi-cal.fits</a></li>
    </ul>

    <b><i>First cadence</i></b>
    <ul>
        <li>Time: 2014-05-30 15:54:44 UTC</li>
        <li>Long Cadence Number: 91332</li>
        <li>Short Cadence Number: 2728420</li>
    </ul>

    <b><i>Last cadence</i></b>
    <ul>
        <li>Time: 2014-08-20 20:19:37 UTC</li>
        <li>Long Cadence Number: 95353</li>
        <li>Short Cadence Number: 2849079</li>
    </ul>

</div>

<div class="col-lg-7">

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Schematic of Kepler's C1 field-of-view with selected targets shown with purple dots.</i>
        </div>
        <a href="images/campaign_selected/C1_selected.png">
            <img src="images/campaign_selected/C1_selected.png" class="img-responsive" alt="C1 field-of-view with selected targets">
        </a>
    </div>

</div>

</div>


## Features and events

<br>
***Attitude Tweak***

The attitude of the spacecraft was changed by a few pixels at cadence 91433 to better position the targets in the center of their apertures. All cadences in C1 prior to this event have the first bit in the QUALITY column set (integer value = 1) to indicate that they were taken prior to the tweak.

<br>
***Trans-Neptunian Object***

A long-cadence custom aperture was constructed in order to collect data on trans-Neptunian Object 2002 GV31. Note, this target is very faint (V=22) and falls in its custom aperture pixels for only about 10 days. This custom aperture can be found by searching the MAST for the K2 ID numbered 200001049.

<br>
***EPIC Catalog Assignment***

For this Campaign, a number of targets were proposed without EPIC ID numbers. If a target was observed, it was either 1) given an EPIC ID number from the regular catalog if that target matched a target in the catalog, or 2) assigned a new EPIC ID. We created EPIC ID numbers for 28 targets, ranging from 210282464 to 210282491. Regular EPIC targets in C1 have catalog ID numbers ranging from 201000001 to 202059065.

## Release History

The following is the data release history for this campaign. Follow the link for information about some of the features of the software used to reduce and export these data. There will be a new entry each time the data is released by the mission.

* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr3">Data Release 3</a>

<hr>




# K2 Campaign 0

Campaign 0 (C0) was implemented as a full-length engineering test to prove that K2 was a viable mission. It observed sources "at risk" from a community-provided target list.

## At a glance

<div class="row">
<div class="col-lg-5">

    <b><i>Pointing</i></b>
    <ul>
        <li>RA: 98.2985439 degrees</li>
        <li>Dec: 21.5904167 degrees</li>
        <li>Roll: 177.4754730 degrees</li>
    </ul>

    <b><i>Full Frame Images (FFI)</i></b>
    <ul>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014070234206-c00_ffi-cal.fits">ktwo2014070234206-c00_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014074233223-c00_ffi-cal.fits">ktwo2014074233223-c00_ffi-cal.fits</a></li>
        <li><a href="https://archive.stsci.edu/pub/k2/ffi/ktwo2014110010101-c00_ffi-cal.fits">ktwo2014110010101-c00_ffi-cal.fits</a></li>
    </ul>

    <b><i>First cadence</i></b>
    <ul>
        <li>Time: 2014-03-12 00:18:30 UTC</li>
        <li>Long Cadence Number: 87434</li>
        <li>Short Cadence Number: 2611480</li>
    </ul>

    <b><i>Last cadence</i></b>
    <ul>
        <li>Time: 2014-05-27 16:48:13 UTC</li>
        <li>Long Cadence Number: 91186</li>
        <li>Short Cadence Number: 2724069</li>
    </ul>

</div>

<div class="col-lg-7">

    <div class="thumbnail">
        <div class="caption">
            <i>Figure: Schematic of Kepler's C0 field-of-view with selected targets shown with purple dots.</i>
        </div>
        <a href="images/campaign_selected/C0_selected.png">
            <img src="images/campaign_selected/C0_selected.png" class="img-responsive" alt="C0 field-of-view">
        </a>
    </div>

</div>

</div>

## Features and events

<br>
***Not In Fine Point Data***

The second half of the C0 data is more indicative of the quality of data users should expect from K2. The Kepler spacecraft was not in fine point for the first part of C0, causing large photometric scatter. The data quality is much improved in the second half of the campaign, beginning on cadence 89347 after the safe mode, when compared to the first half of the campaign. See the QUALITY flag (bit 16) to determine when the spacecraft was in fine point.

<br>
***Safe Mode***

The Kepler Spacecraft was in safe mode between cadences 88198 and 89346. Data is flagged in the QUALITY column with bit 2. The project used this time to fix large attitude errors that were occuring during resaturation events.

<br>
***Photometric Jitter Caused by Lower Bandwidth***

During the development of the K2 Mission, the number of guide stars per fine-guidance sensor (FGS) was changed from ten (for Kepler) to one (for K2). This change was demanded by the need for increased aperture sizes given the uncertainties in the star-tracker to boresight alignment and the need to acquire an entirely new field-of-view every 80 to 90 days. To compensate for the increased sensor noise and assure that fine-point lock could be achieved, the attitude control bandwidth was decreased from 0.1 Hz (for Kepler) to 0.02 Hz (for K2). This change in bandwidth means that the cross-boresight attitude (i.e., RA and Dec) has a time constant of 50 seconds, comparable to the short-cadence duration. Engineering studies have shown that the photometric precision of the long-cadence data is also compromised by the larger pointing jitter associated with the lower bandwidth. The project has approved a change in bandwidth to 0.05 Hz (20 seconds) starting with Campaign 3.

<br>
***Large Pixel Masks***

When planning C0 observations, the pointing performance of K2 was not accurately known. The worst case scenario was that a star at the edge of the focal plane could move as much as 40" from its nominal position. Therefore each star was assigned a large pixel mask by first computing a Kepler-style optimal aperture and then adding 10 rings of pixels to account for a potential 40" pointing offset. During the second half of C0, the pointing performance was excellent and the pointing drifts were no more than 6" for any target star. Care will be needed when performing photometry on C0 data. Simply including all collected pixels for a given target will not create a high signal-to-noise light curve. For tools to help choose your photometric aperture, see for example, <a href="http://keplergo.arc.nasa.gov/PyKE.shtml">PyKE contributed software</a>.

<br>
***Jupiter's Reflection***

Because K2 points along the ecliptic, its field of view will occasionally contain bright solar system objects. Jupiter was in the K2 field of view during C0 from 2014-03-14 through 2014-05-12, but fell on dead module 3. It creates a bright antipodal ghost on module 23, channel 79, and impacts all the targets observed in this region. See the FFI ktwo2014074233223-c00, extension 79, for an image of the reflection.

While Jupiter was on the focal plane, the background level was increased over its nominal value for nearly half the channels, with the largest impact seen in channels 53 -- 84. In addition, as Jupiter moved on and off the focal plane, a specular reflection lasting approximately 6 hours was seen in these channels. The relative background levels as measured in the smear signal from channel 83 are shown below as Jupiter enters the focal plane (near cadence no. 87525) and leaves the focal plane (cadence no. 90375). The specular bump resulted in an increase in background level of 25-30% for the affected channels, while the quasi-static background increase for the time Jupiter was on the focal plane was 3-5%.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: FFI showing the reflection of Jupiter as seen on channel 79.</i>
    </div>
    <a href="images/release-notes/c0/Jupiter-ghost3.png">
        <img src="images/release-notes/c0/Jupiter-ghost3.png" class="img-responsive" alt="FFI showing the reflection of Jupiter as seen on channel 79.">
    </a>
</div>

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: The background level on channel 83 as Jupiter enters (left) and leaves (right) the focal plane.</i>
    </div>
    <a href="images/release-notes/c0/ch83_jupiter_on_smear.png">
        <img src="images/release-notes/c0/ch83_jupiter_on_smear.png" class="img-responsive" alt="The background level on channel 83 as Jupiter enters (left) and leaves (right) the focal plane.">
    </a>
</div>

<br>
***Observations of M35 and NGC 2158***

The open clusters M35 (NGC 2168) and NGC 2158 were observed during this campaign by placing 154 separate 50x50 pixel masks over the densest portion of these two adjacent clusters. Each mask was given a custom aperture number to act as the unique identifier found in the file name. The target pixel files for these clusters have custom aperture numbers ranging from 200,000,811 to 200,000,964.

<div class="thumbnail" style="width: 68%;">
    <div class="caption">
        <i>Figure: Individual masks when tiled together cover the field of view containing M35 and NGC 2158.</i>
    </div>
    <a href="images/release-notes/c0/M35_im1.png">
        <img src="images/release-notes/c0/M35_im1.png" class="img-responsive" alt="Individual masks when tiled together cover the field of view containing M35 and NGC 2158.">
    </a>
</div>

<br>
***Channel 10 Black Correction***

The black correction on Channel 10, mod.out 4.2, has problems because a bright star bleeds into the black region. For data release 1, the affected regions of the black are excluded from the fit of the black, so the fit is poorly constrained and we see chatter in the residuals. This mostly affects stars in the last 200 rows of the channel.

<br>
***Image Artifacts in K2***

The thermal environment is changing more rapidly in K2 than it did for the Kepler Mission. As a result the number of channels with significant rolling band (changes in the black level that are both time and spatial dependent) is larger for K2. The channels observed to be most impacted by rolling band in C0 are 1, 2, 10, 11, 14, 25-28, 36, 44, 58, 62, 74 and 79. Other known image artifacts, such as Moiré patterns and undershoot from bright stars, are also likely to be enhanced in K2 data as compared to Kepler. See the <a href="http://archtest.stsci.edu/kepler/manuals/KSCI-19033-001.pdf">Kepler Instrument Handbook</a>.

<br>
***Module 7 Failure***

Prior to the start of C0, on January 21, 2014, the photometer was autonomously powered off by an under voltage fault in the Local Detector Electronics Power Supply. Since that time, module 7 (i.e., channels 17 to 20) has yielded no star data or charge injection signal. The subsequent behavior of this module is very similar to that of module 3 after it failed on January 19, 2010. K2 continues to operate and collect simultaneous data from sources falling upon the remaining 19 detector modules over 105 square degrees. There is no indication of any accelerated degradation on these other modules.

<br>
***Cropped Calibrated Pixels in Data Release 1***

**The problem described below was corrected in Data Release 2 of the Campaign 0 data. See the DATAREL keyword in the primary header of the target pixel file to determine which data release you have. We recommend that everyone use the latest release of the data.**

In Data Release 1, for cadences after the Safe Mode (cadence no. 89346), the calibrated data (see the FLUX column in the exported target pixel files) is incorrectly reporting a value of zero for pixels collected near the edge of the aperture. The raw pixels (see the RAW_CNTS column) do not have this issue, so the collected data is properly reported in the target pixel files. An example of the issue is shown in the figure below. The left image is the mask (white indicates a collected pixel), the central image shows the calibrated pixels and the right image contains the raw pixels for one cadence. Those columns and rows that are black in the central image incorrectly have a value of zero, but there is clearly data in the original raw data on the right.

This issue occurs for both the long and short cadence data. It does not appear in the custom apertures, so the calibrated pixels are being exported as expected for these files.

<div class="thumbnail" style="width: 100%;">
    <div class="caption">
        <i>Figure: Image of mask (left), calibrated pixels (center) and raw pixels (right) for one cadence of one target.</i>
    </div>
    <a href="images/release-notes/c0/mask-issues.png">
        <img src="images/release-notes/c0/mask-issues.png" class="img-responsive" alt="Image of mask (left), calibrated pixels (center) and raw pixels (right) for one cadence of one target.">
    </a>
</div>

## Release History

The following is the data release history for this campaign. Follow the link for information about some of the features of the software used to reduce and export these data. There will be a new entry each time the data is released by the mission.

* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr2">Data Release 2</a>
* <a href="http://keplerscience.arc.nasa.gov/K2/pipelineReleaseNotes.shtml#dr1">Data Release 1</a>
