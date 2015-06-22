# CPU Memory Map #

<table border='1' cellspacing='0'>
<tr>
<th>Address Range (Hexadecimal)</th>
<th>Size</th>
<th>Notes (Page size is 256 bytes)</th>

</tr>
<tr>
<td>$0000 - $00FF</td>
<td>256 bytes</td>
<td>Zero Page - Special Zero Page addressing modes give faster memory read/write access</td>
</tr>
<tr>
<td>$0100 - $01FF</td>
<td>256 bytes</td>
<td>Stack memory</td>
</tr>

<tr>
<td>$0200 - $07FF</td>
<td>1536 bytes</td>
<td>RAM</td>
</tr>
<tr>
<td>$0800 - $0FFF</td>
<td>2048 bytes</td>
<td>Mirror of $0000-$07FF</td>
<td>$0800-$08FF Zero Page<br />
$0900-$09FF Stack<br />
$0A00-$0FFF RAM</td>
</tr>
<tr>
<td>$1000 - $17FF</td>
<td>2048 bytes</td>
<td>Mirror of $0000-$07FF</td>
<td>$1000-$10FF Zero Page<br />
$1100-$11FF Stack<br />
$1200-$17FF RAM</td>

</tr>
<tr>
<td>$1800 - $1FFF</td>
<td>2048 bytes</td>
<td>Mirror of $0000-$07FF</td>
<td>$1800-$18FF Zero Page<br />
$1900-$19FF Stack<br />
$1A00-$1FFF RAM</td>
</tr>
<tr>
<td>$2000 - $2007</td>

<td>8 bytes</td>
<td>Input/Output registers</td>
</tr>
<tr>
<td>$2008 - $3FFF</td>
<td>8184 bytes</td>
<td>Mirror of $2000-$2007 (multiple times)</td>
</tr>
<tr>
<td>$4000 - $401F</td>
<td>32 bytes</td>

<td>Input/Output registers</td>
</tr>
<tr>
<td>$4020 - $5FFF</td>
<td>8160 bytes</td>
<td>Expansion ROM - Used with Nintendo's MMC5 to expand the capabilities of VRAM.</td>
</tr>
<tr>
<td>$6000 - $7FFF</td>
<td>8192 bytes</td>
<td>SRAM - Save Ram used to save data between game plays.</td>

</tr>
<tr>
<td>$8000 - $BFFF</td>
<td>16384 bytes</td>
<td>PRG-ROM lower bank - executable code</td>
</tr>
<tr>
<td>$C000 - $FFFF</td>
<td>16384 bytes</td>
<td>PRG-ROM upper bank - executable code</td>
</tr>

<tr>
<td>$FFFA - $FFFB</td>
<td>2 bytes</td>
<td>Address of Non Maskable Interrupt (NMI) handler routine</td>
</tr>
<tr>
<td>$FFFC - $FFFD</td>
<td>2 bytes</td>
<td>Address of Power on reset handler routine</td>
</tr>
<tr>

<td>$FFFE - $FFFF</td>
<td>2 bytes</td>
<td>Address of Break (BRK instruction) handler routine</td>
</tr>
</table>