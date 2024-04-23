Muhammad Navis Raditya Riayatsyah
2106717291
Tutorial 7 Game Development

Latihan: Basic 3D Plane Movement
- buat scene `player`
- tambahkan node KinematicBody dan CollisionShape sebagai child dari Player
- tambahkan node Spatial, ganti nama jadi Head dan tambahkan kamera di Head
- putar CollisiionShape dan MeshInstance menjadi 90 derajat
- integrasikan script sesuai dokumen soal dan membuat InputMap sesuai (tapi di project file udah ada dari awal)
- kontrol kamera baru bisa aktif setelah mengaplikasikan script yang ada di soal

Latihan: Object Interaction
- untuk interaksi object, bikin script buat interactable dan script buat objeknya. INGAT script interactble jangan dikaitkan ke node manapun biar bisa berfungsi
- untuk raycast.... sepertinya saya kurang explore soalnya masih gk bisa fungsional

Latihan: Membuat Level 3D Menggunakan CSG
(ini pusing banget)
- Buat sebuah scene 3D baru, namai "ObjLamp".
- Tambahkan child node, pilih CSGCombiner, dan namai "lamp".
- Tambahkan child nodes untuk membentuk bagian lampu:
   1 CSGCylinder dengan sebuah cone untuk dasar lampu.
   2 CSGCylinder lain untuk tiang lampu.
   3 CSGPolygon untuk membentuk trapesium sebagai penutup lampu.
- kalau mau warnain, bisa pilih node yang mau diwarnain, terus bikin SpatialMaterial baru. dan masukkan warna di Albedo sesuai keinginan

Menambahkan obstacle
(oke aku harus jujur... buat readme tentang menambah obstacle ini aku cuma summarize dari soal karena pas coba2 masih gk berhasil dan ini jadi bagian paling pusing selama ngerjain tutorial 7)
- Buka scene "World 1".
-  Tambahkan node CSGCombiner baru dan centang "Use Collision" di tab Inspector.
-  Tambahkan dua node CSGBox ke dalam CSGCombiner untuk membuat ruangan baru dan lubang.
-  Letakkan sebuah CSGBox tambahan di luar CSGCombiner untuk memungkinkan pemain melompati lubang.

Interaksi antar Scene
(sama seperti 2D. pake trigger body)
- buat scene baru, kasih nama area (kalo punyaku, namanya AreaTrigger3D
- tambahkan CollisionShape sebagai child dari node area
- pake script dari soal ke Area
- hubungkan signal ke script dari Area
- Buat bikin level dan integrasi antar scene, tinggal tambahin "get_tree().change_scene(str("res://Scenes/" + sceneName + ".tscn"))"

segini dulu soalnya belom implementasi latihan mandiri ehe
