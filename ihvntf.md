代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vwmrvkdh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dnsmcwhl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3aiilopuc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bxvjsbei.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ddjldemi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtbwaqak.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnnxguh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3belbxzug.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvkupebx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ocnplvbo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xyksfyfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dfdvkwtw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ftacumge.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rinyzlkx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jsnsexbp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wjbpaipu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3isiavpzd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hqshvwtj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3stnlquei.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebwvfeym.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3datbakwk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3sycyntvf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3sasnmerf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gatyiwuy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ybwzommw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yscpbxfd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ermqwivb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qomgwost.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qfkymlwn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fbqayzkm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3piscixbg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bcadjfyf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3csfvjcqm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebkobvmv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvpulboe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afegkvoj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pmwelzac.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ljpbqznt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xxwfjkur.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mepnohba.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yhtupuyd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gltxkqyq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3utxvsios.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sltzsrot.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3diffzkiz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xkanjfva.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnzymain.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3emtavnjc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bakaroml.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3feeolqgu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qrneucod.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yhobskik.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vgdrhhvx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3euxrdraa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3nafdceik.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cnygfcvs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3prqummoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtcmeefw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fxxyfjxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwatfsdf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3syxgyhjg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vtcnjpar.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nycjxkwc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nwdvmiam.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3icsomuzb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iwhelaog.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xdprsiow.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plfomlpq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dnxdrrmf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgqbsyfy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ckfndisd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bnjjkdrn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pfcyqbgl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljzvqmxc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pexijpaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wvurynjs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ihznhopo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxdqjtbd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3itdvgkhn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3njpcjyjh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3edjpehba.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3usdnkcer.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3adhwcxlu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yrwscqao.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3albdevpl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cijwpxhb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wstrisah.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcucigaz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qxgjzxxx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3selnhgmy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ylzbyrje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gbaxfckt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ukkrnjoi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eodgytzo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fyuokcfm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hopogvtp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kaczesto.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qojtdjvz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3engdhtym.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxlzdugq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfpdtopg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3adccxmfx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iudjsdoy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swozeptp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orgasgog.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3berpbink.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bribwwwo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kuevytoq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fopxcbxr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iippxqdl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oyretmtm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsokuyzt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aumiqqzj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdfjfdyc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3smomanjz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mxebzfkj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3udismqta.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dpyiqhbd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gyvtohmt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wndfgamb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3iqhbtuul.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zwrnmfdd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xxixucms.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3iuftvomp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ilpgqyzh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkrdawp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xntoseyk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xfmetopq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3onuibvrn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pslwhshd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbsdksoe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3suwgglks.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fiiysfsi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohjbhyyb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uynswtqd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xjntqgri.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wlbzfpwe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3accrjrjq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3cxlfofwc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgyoobqi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fvftkfte.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pbfdnnzl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snkmorin.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ghmryisd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okyvqglo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkgiboxy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3itsrajsz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otcoexwv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evkmbbju.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvqmptru.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bgoxdiuy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3daxtmknj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxmyyfqx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfszzmri.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcizcivv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gohnravs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rzbwtbba.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbgxtmza.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cyktuzzw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3byjuzgba.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qjmgcdfc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rvmkfvap.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dshvvcjc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kdvngmqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ejowkusn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rlgkcufq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ydtmcumn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lxqbbmrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kutqhlly.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wurunqis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiszdbon.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mhyiikjh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hbjdlpzm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkoptlgb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlgismdo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qngqkmel.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qtopiwoo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yphgzucd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmwvnk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3laykcolv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mhuioexs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qvcrqvnu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfbatsvz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjtjgwd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjlqyldy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvsomjzt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qlwgskwt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ltcnquxr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lktnnzrs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bdqopikq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3alwjndqi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dxnzhrmw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3happgbdb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nmfhwqwq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rtormaxs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3cqfcikyq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jleowjoa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ylcerxrk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3iyqypaoo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vxtrrvhd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tpeselgv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyzriplw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrtleljp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yzcjdxxt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fegaxrpm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vwlzxcyz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uxvdmdmb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dmovaqtd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iozgbcfg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwtkjvyy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dowmuzoj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3swrkvmtk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3amycmvll.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pgjqvixh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3azxkfeum.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fcdgsipl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3drgsbchq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3yrwzffgu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdaufpty.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khmcaygj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qrinzodr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvksgxxd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3arictdcc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tqyllfip.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ailiqbdy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rrtkkswt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cywstigu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vniznfqf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qafongzz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dslcddus.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mzbxrxoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3iyotnzvv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nddscjvc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mvzjywlj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zoftylzg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kqgwxxnc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3apbekenh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jvlqgnqq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fmmpvlfs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3sqrwqddw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xemncdpc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tmsuudsf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yiwdfmnm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fsqczfzv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3sotlpefg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3twfjfecr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yuvnbhsc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ippsvlil.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgsimoan.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3clmuoksu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3frfhojwj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khvoelku.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mfzsywbm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nzdjxcej.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3omymmqmw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kdtxqgau.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3woqeikeh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yxkzbkjd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3swaexclc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lrihdwiy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vswuuxgk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3lutvkhsu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xnqsoxzy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bpomkkqy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhrvqmty.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsbxkfyj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cxxnenmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vloibvik.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xjhztrhe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmvfqien.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hfuhxlie.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tzdmmfow.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rtyymmlg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjjrgpoz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onvmrnmz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eowbnwsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pabhstaj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ksnjepop.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3octgzrdm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhuyhp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtlllwo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ycnymyms.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cgllifzn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3juzlifwl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cemwkbsv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3dqvegpmy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bbbdidrh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fhxgglnc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qbffnfyr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mhhpvguz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqwcml.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3veyilfna.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tudwikwj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jsoakmgi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uexldyku.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vsnalpwy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mxmzuvzp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tsjdfeyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkjuspdj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uxkzzfgw.html


<!-- 参考信息 -->