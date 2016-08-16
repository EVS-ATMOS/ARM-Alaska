============================================
Design for Clutter Analysis for the OLI KaZR
============================================

Introduction and Aims
=====================
The Ka-Band Zenith Pointing Radar (KaZR) was deployed as part of an ARM Mobile
Facility three (AMF3) deployment to Oliktok Point on the North Slope of Alaska.
Figure 1 shows a time height plot of reflectivity factor from the KaZR.

.. figure:: ./refl.png
   :scale: 200 %
   :alt: Ka Band reflectivity
   
   Figure 1: Time height plot of reflectivity. Note the clutter at 1,500 meters. 

Clutter can be seen as a constant signal at around 1,500 meters above the radar. 
The aim of this task is to produce a map of affected gates and to study the
temporal variability and impact on overlaid meteorological signals. There will
be two deliverables: A CF-Radial file describing the clutter field and a Jupyter
notebook showing the analysis of the clutter field. 

Methodology
===========
Analysis will be performed using the Python programming language and will make
extensive use of Py-ART. We will use the Sky Cover VAP from the total sky imager
and the cloud base heights from the ceilometer to identify clear air days. We
will then look at the average returned power to identify affected gates. We will
look within our data set to see if there is any discernible diurnal or other
cycle in the clutter data and also look at the variability to see if there were
any external events that changed the power returns. 

In addition we will identify several cases where there is a meteorological
signal in a clutter impacted gate and look at the radar Doppler spectrum to see
just how severely impacted weather returns are and if we may be able subtract
the clutter signal from meteorological return and recalculate the moments.

Effort, Staff and Impact
========================
This task will be carried out by Scott Collis at Argonne National Laboratory. We
expect it to take 60 hours of effort and be delivered by October 1st 2016. There
is no impact on operations, however the work will delay other products work
being carried out by Translator team at Argonne. 

