# Priceglade: Grocery Price Book

<img src="assets/icon.png" width="96" alt="Priceglade paired-tag icon">

**A personal price book. Different packs, on one clear basis.**

[Product and guide](https://sepidehdalir.github.io/priceglade/) · [Privacy](https://sepidehdalir.github.io/priceglade/privacy.html) · [iOS portfolio](https://github.com/sepidehdalir/ios-app-portfolio)

**Production in progress, October26,2026. Version1.0(1) is not submitted, approved or released.** Final physical-device, genuine Sandbox, Apple privacy/submission and remaining QA gates are still pending. TestFlight is skipped by publisher instruction.

## The job

Remember what you actually paid. Record a product, store, date, currency, quantity per pack, identical-pack count and total paid for all packs. Compare compatible quantities and see your own recorded latest, lowest, median and highest prices with dates and sample counts. There is no live retailer feed, market-lowest claim or currency conversion.

## Product decisions

Free includes ten active products, manual entries, equivalent-unit comparison, personal history, stores/categories, corrections, Undo, archives, recoverable Trash and full JSON backup/recovery. Lifetime Pro is a one-time non-consumable for additional active products within device limits, new on-device text recognition, advanced filters and confirmed-purchase CSV. Apple supplies the localized purchase price. Existing records remain accessible if access changes.

OCR creates an unconfirmed text draft. Users select lines, correct every field and explicitly review before saving a purchase. Images are transient and are not retained with the book or backups. Full recovery imports fresh archived copies without replacing current work or preferences.

## Engineering

Universal iPhone/iPad, deployment15.0 with currentSDK26.5. SwiftUI, checked Foundation Decimal calculations, explicitly labeled metric/US/Imperial units, currency minor-unit rules, immutable purchase snapshots, bounded graph validation and coordinated atomic protected JSON writes. The model publishes only after successful persistence and rejects stale revisions. Vision recognition runs on device; StoreKit2 grants verified entitlements only. No developer account, backend, tracking, advertising or analytics SDK.

## Verification so far

Fifty native iOS17 cases passed, including real Vision recognition, persistence/recovery and local StoreKit states. Forty-six selected domain/native/model cases passed on the current iPad simulator. Actual screen checks cover reviewed pack totals, history/relaunch, comparisons, saved scan drafts, the ten-product gate followed by a local Pro purchase, and completed local Restore Purchases. Current phone/iPad campaign flows also passed. Native Files JSON save/open/fresh archived-copy import and CSV save/output inspection passed. Signed Archive/AppStore export and package resource/privacy/signature audits passed. These are dated checkpoints, not a claim of completed physical or genuine Sandbox testing. Actual iOS15 runtime and spoken VoiceOver remain unverified.

## Original campaign

The first three frames communicate the value, equivalent-quantity workflow and personal result. The iPad campaign uses dedicated layouts. All screens are authentic native UI with original fictional examples; text recognition examples do not establish OCR accuracy. Commercial Swift source, tests, signing material and private QA artifacts are excluded from this repository.

<img src="assets/campaign/iphone-01.png" width="210" alt="Remember what you paid"> <img src="assets/campaign/iphone-02.png" width="210" alt="Different packs, equal footing"> <img src="assets/campaign/iphone-03.png" width="210" alt="Your personal price history">

Publisher: **Sepideh Javanbakht Dalir** · [arvinify.com](https://www.arvinify.com) · [hello@arvinify.com](mailto:hello@arvinify.com)
