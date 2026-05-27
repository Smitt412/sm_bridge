# sm_bridge

Bridge dependency for SM resources.

## Supports
- Frameworks: `es_extended`, `qb-core`, `qbx_core`, or standalone identifiers.
- Inventory: `ox_inventory`, `qs-inventory`, `qb-inventory`, `lj-inventory`, `ps-inventory`, `core_inventory`, `codem-inventory`, `ak47_inventory`, `ak47_qb_inventory`, `tgiann-inventory`, `origen_inventory`, framework inventory functions, or `SMBridgeConfig.CustomInventory` hooks.
- Notifications: `ox_lib`, QBCore, Qbox, ESX, okokNotify, mythic_notify, t-notify, `qs-notify`, `nass_notifications`, `drc_notify`, `frvgs_notify`, `vms_notify`, `rtx_notify`, `brutal_notify`, `wasabi_notify`, `stNotify`, `zm_notify`/`zm_notify_escrowed`, chat fallback, or custom hook.
- Progress bars: `ox_lib`, progressbar/qb-progressbar, mythic_progbar, progressBars, rprogress, `drc_notify`, wait fallback, or custom hook.
- Dispatch: cd_dispatch, ps-dispatch, qs-dispatch, core_dispatch, job notify fallback, or custom hook.
- Target: ox_target, qb-target, qtarget, or custom hook.

## Install Order
Ensure `sm_bridge` before any script that uses it:

```cfg
ensure sm_bridge
ensure sm_trap_selling
ensure sm_legal_selling
ensure sm_playtime_rank
ensure sm_combat_stats
```

Edit `config.lua` to force a specific adapter or leave values as `auto`.
