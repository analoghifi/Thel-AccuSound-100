#### work in progress not finished yet !  

this is not the original Thel PCB but it's very like\* the original with the following exceptions:  
* different board dimensions original: 200mm x 100mm -> this PCB: 200mm x 103mm  
* using a combined 5.0mm/7.5mm pin spacing footprint for the small foil caps C12 and C23  
  
\*(same schematic / same 1-layer\** layout THT / same THT components in the same places on the board)  
\**(strictly speaking, this KiCad PCB is a two-layer PCB with plated-through holes, but you can also (let) produce it as a classic 1-layer PCB with non-plated holes if you wish, since all the tracks are on the bottom side only)  
  
----  

#### remarks:
in the original, mica capacitors from the US company "Cornell Dubilier Electronics" (CDE) are used for C2, C3 and C9  
the [CD15-Series](https://github.com/analoghifi/capacitors/blob/main/audio%20and%20filter%20capacitors/docs/datasheets/mica%20glimmer/CDE_Silver_Mica_series_STD-DIPPED.pdf) or the better [CD17 Series](https://github.com/analoghifi/capacitors/blob/main/audio%20and%20filter%20capacitors/docs/datasheets/mica%20glimmer/CDE_Series_CD17_CD18_high_frequency.pdf) is used:  
* C2, C3 = 47pF / 1% / 500V / 6.9mm pitch / Type-No. CD15ED470FO3 ([stock at Mouser](https://www2.mouser.com/ProductDetail/Cornell-Dubilier-CDE/CD15ED470FO3?qs=9iVfQKk8ifFmXLRqX5bCNQ%3D%3D))  
or better CD17ED470JO3F ([stock at Mouser](https://www2.mouser.com/ProductDetail/Cornell-Dubilier-CDE/CD17ED470JO3F?qs=nnhpPVbCybXjnSWSlsUlRA%3D%3D))
* C9 = 10pF / 5% / 500V / 6.9mm pitch / Type-No. CD15CD100JO3 ([stock at Mouser](https://www2.mouser.com/ProductDetail/Cornell-Dubilier-CDE/CD15CD100JO3?qs=m9iv7GyUMnFXRIC2%252BbnrrQ%3D%3D))  
or better CD17CD100JO3F ([stock at Mouser](https://www2.mouser.com/ProductDetail/Cornell-Dubilier-CDE/CD17CD100JO3F?qs=PXF%252Blbo4VJ7Sv5GDGZWsoQ%3D%3D))  
  
since C2,C3 and C9 are used for controlling the ultrasonic frequencies (>20kHz) here in this circuit you may use instead  
ceramic C0G capacitors (tolerance: 1% to 2,5% / rated DC Voltage: 100V or 205V / pitch 5mm or 7,5mm)  
e.g. KEMET "[goldmax 300](https://github.com/analoghifi/capacitors/blob/main/audio%20and%20filter%20capacitors/docs/datasheets/C0G/KEMET_C1049_GOLDMAX_C0G_THT.pdf)" Series in THT version ([10pF/47pF stock at mouser](https://www2.mouser.com/c/passive-components/capacitors/ceramic-capacitors/mlccs-multilayer-ceramic-capacitors/multilayer-ceramic-capacitors-mlcc-leaded/?q=goldmax&capacitance=10%20pF%7C~47%20pF&dielectric=C0G%20%28NP0%29&lead%20spacing=5.08%20mm&tolerance=1%20%25&voltage%20rating%20dc=250%20VDC))  
They perform very well for high frequencies and are a very good alternative to the expensive Mica caps from CDE.  

----  
  
these are KiCad 6.x projects  
see how to get the proper 3D-Models from here: https://github.com/analoghifi/KiCad-3D-Models  
  
----  
  
use kicanvas.org to see this KiCad-Project in Browser:  
https://kicanvas.org/?github=https://github.com/analoghifi/Thel-AccuSound-100/tree/main/hardware/4.)%20final%20version%202003-2015/4.2)%20version%202006-2011/KiCad/original
