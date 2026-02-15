# siero-coin
Siero Coin is an open-source digital asset designed for the era of Agent AI. Unlike traditional ERC20 tokens, Siero Coin integrates a Trust System and Consequence Mechanism to create a living, reputation-driven economy.
siero-coin/
│
├── core/                        # Rust Core (SieroCoreFinal)
│   ├── Cargo.toml               # konfigurasi Cargo
│   ├── src/
│   │   ├── lib.rs               # library utama
│   │   ├── ledger.rs            # modul ledger transaksi
│   │   ├── trust.rs             # modul trust system
│   │   ├── consequence.rs       # modul consequence (penalti/pajak)
│   │   ├── governance.rs        # delegated governance node
│   │   └── heartbeat.rs         # pulse & resonance protocol
│   └── tests/                   # unit test Rust
│
├── middleware/                  # Python M Core
│   ├── setup.py                 # konfigurasi package PyPI
│   ├── siero_middleware/
│   │   ├── __init__.py
│   │   ├── api.py               # REST API untuk wallet
│   │   ├── validator.py         # compliance filter (trust/consequence)
│   │   ├── agent.py             # integrasi agent AI
│   │   └── utils.py             # helper functions
│   └── tests/                   # unit test Python
│
├── contracts/                   # Smart Contract ERC20
│   ├── SieroCoin.sol            # kontrak utama ERC20
│   ├── TrustSystem.sol          # modul trust
│   ├── Consequence.sol          # modul penalti
│   └── migrations/              # script deploy
│
├── gui/                         # Wallet & Dashboard
│   ├── package.json             # konfigurasi npm
│   ├── src/
│   │   ├── App.js               # entry point React/Vue
│   │   ├── Wallet.js            # saldo, send/receive
│   │   ├── TrustScore.js        # menampilkan trust score
│   │   ├── Consequence.js       # menampilkan penalti
│   │   ├── GovernanceBadge.js   # status Raja/Ratu Komunitas
│   │   └── api.js               # koneksi ke middleware
│   └── public/
│
├── docs/                        # Dokumentasi
│   ├── README.md                # deskripsi proyek
│   ├── INSTALL.md               # cara install & run
│   ├── ARCHITECTURE.md          # diagram sistem
│   ├── GLOSSARY.md              # istilah teknis (trust, consequence, governance)
│   └── CONTRIBUTING.md          # panduan kontribusi
│
├── LICENSE                      # lisensi open source (MIT/GPL/Apache)
└── .gitignore                   # file yang diabaikan Git
