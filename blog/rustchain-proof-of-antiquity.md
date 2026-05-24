## RustChain: Mining on Vintage Hardware with Proof-of-Antiquity

*Published: 2026-05-25*

---

### What is RustChain?

RustChain is a Proof-of-Antiquity (PoA) blockchain that rewards miners based on hardware age rather than computational power. Unlike Proof-of-Work where faster hardware wins, RustChain gives higher multipliers to older, vintage machines.

### How Proof-of-Antiquity Works

Every unique hardware device gets exactly 1 vote per epoch. Rewards are split equally among active miners, then multiplied by the hardware's antiquity multiplier.

**Hardware Multipliers:**
- DEC VAX-11/780 (1977) — 3.5x
- Motorola 68000 (1979) — 3.0x
- PowerPC G4 (2003) — 2.5x
- Apple Silicon M1-M4 — 1.2x
- Modern x86_64 — 0.8x

### Hardware Fingerprinting

Each miner must prove it's running on real hardware through 6 checks: clock-skew, cache timing, SIMD identity, thermal drift, instruction path jitter, and anti-emulation detection. Virtual machines get 1/1,000,000,000th of rewards.

### Getting Started
```bash
git clone https://github.com/Scottcjn/Rustchain.git
cd Rustchain && python3 -m venv venv
source venv/bin/activate && pip install -r requirements.txt
python3 setup_miner.py
python3 miners/linux/rustchain_linux_miner.py
```

### Resources
- [rustchain.org](https://rustchain.org)
- [GitHub](https://github.com/Scottcjn/Rustchain)
- [BoTTube](https://bottube.ai)
