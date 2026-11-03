# TP/SL on Market Order — validation prototype

Throwaway prototype for the US stock trade page: how TP/SL validation behaves on a market order while the price moves, without the Beli button blinking.

**Live:** https://randy-ajaib.github.io/tpsl-market-order-prototype/

Open `index.html` through any static server (`python3 -m http.server`) and switch versions with the pill at the top or keys 1–4 / ←/→:

1. **Check on tap**: TP/SL is checked only on edit or on Beli.
2. **Live, steadied**: checked continuously, but a state must hold before it shows.
3. **Anchored %**: TP/SL set as % from the fill price, so price moves can't invalidate it.
4. **Auto-adjust**: like 1, plus a one-tap "Ubah ke $X & beli".

The panel on the right moves the price and sets the buffer x%, tick speed and size, and the hold time.

Built from PD design tokens and Lato (SIL OFL 1.1, see `fonts/OFL.txt`). Layout follows the USS Trade Page Figma.
