Airdrop การส่ง token ไปให้กับคนที่ stake Atom Scrt Luna2 OSMO 

  /contract
    เป็นโปรเดอร์เก็บ ตัว contract (สามารถเก็บได้หลายสัญญา)

  /package
    สำหรับเก็บ package ไว้ใช้กับ ตัวสัญญา ที่อยู่ /contract


Cargo.tome 🦀🦀🦀🦀

นำทางไปโฟรเดอร์ต่าง ตรง [workspace]
 [workspace]
 members = ["packages/*", "contracts/*"]

 [profile.release.package.kanari-token]
 codegen-units = 1
 incremental = false

ให้กำหนดตามนี้
 [profile.release]
 rpath = false
 lto = true
 overflow-checks = true
 opt-level = 3
 debug = false
 debug-assertions = false
