For example add  THSarabun.ttf & THSarabunBold.ttf
* Clone/download html2pdf from https://github.com/spipu/html2pdf/
* Update composer (composer.json) download tcpdf from composer
* This case create in folder vender/tecnickcom/tcpdf

![example](https://www.viriyasoft.com/uploads/TCPDF-font.jpg)

```
php tcpdf/tools/tcpdf_addfont.php -b -t TrueTypeUnicode -f 32 -i THSarabun.ttf,THSarabunBold.ttf
```
### If everything works as expected
```
>>> Converting fonts for TCPDF:
...
>>> Process successfully completed!
```

###
* Set for tcpdf
```
pdf->SetFont('THSarabun', '', 9);
or
$pdf->SetFont('THSarabun', '', 14, '', false);
```
* Set for html2pdf
```
$html2pdf->setDefaultFont("THSarabun");
```

