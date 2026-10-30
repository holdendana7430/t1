代发 wailian999

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gqyxassnt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/glgjvshbi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/geptnrynx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gjigzfuce.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gylcsyhts.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzhscwovu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gqzvqbgdy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gxrlfiale.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gkwwvjpvy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gnwfrjzhi.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gympgpood.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gylhldzwi.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghfabhdfg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gayrklsow.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gghsjoewy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/guzuqipwp.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gjzumttbi.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gpziomjcc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gxicwsslb.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gtnsarski.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gqduytgis.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gctdmaovi.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/geiajbdaa.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxznumhoz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gutdketmo.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gdmemjvio.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gxhzsicdm.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/grcowtunm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gbqwbiltw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsqzzvtqo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gupmhoqgw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcryiojah.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbrhtcpnv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/guixqjeqt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gjehddlig.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghrkwrsaa.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/ghniltlue.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/geqzlklrd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwbbibsyh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gufkmrpto.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/guxrldscj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/ggqxngeog.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gycjcomxu.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/glcksjrxu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gbolelxqo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtpcwdwdj.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gmgwcomvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbfxjspmb.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/glqgtijcw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gjyxhyvsx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghbzzccui.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gajxhruqz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gflrbgxdf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glbyefhbf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/grxrbarwq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/glietmbcw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gthqeaaqr.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gjyljnacn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gldhmzqce.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gcjkebull.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gqviveklx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gztzvfgdi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/goluugzdl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/giusctuyi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gdtqmcitv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gdiqvnzwy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzohabwan.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/grellzkoh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gahudrahl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/glkrvspnc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gxoffhiyh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gfrzovkfv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gppywkqlc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gjunzvydd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjuallshz.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gechxwmpz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/geynrganh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gxkmhradq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkwptmg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gvadorxia.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gmnxhlanr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gskcwprci.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gcxkoukvd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gmeshprsh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gqsoxswla.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/getgniaux.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtbwxxogn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdfzzbvnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyjydnkmo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxdukaxjc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/ghzzbqheu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqaapsaec.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gngmtpqug.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gijbfkqiv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmthvzwyw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/geeajfszc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkdrysfkb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggoqwpnep.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gecakzdbw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghfddvpqi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gikzlvpmn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpxzrzgvn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gbsfyxsxd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/ggmfxeuhl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gqrmfkqim.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gkwhdkckt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gyvqqqjbk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gsbnphyez.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gkygjqxub.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gngcguuse.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gixsqynuh.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gldmimvck.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gpyupghar.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gwvozcegz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gihsnxjmd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfafqffii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/goarwdrkf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gsylznoyo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/glcdldrao.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gxvvswqjx.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gqqteccxg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpztbtmvv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghaodddkr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gyuakdypk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtqymuvyq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gegpalyms.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gfuxmlekk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfexscuva.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gjxvojugh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/ghgmxvkcw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxvwpbkoq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnqzmvaja.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtqbntkgw.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfehdypuk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gccpxuojm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsaiaoqqr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqezbcxwn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnsfrbfdw.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gdhhwxduf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gayzyaakp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gfroxukes.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gsebpiipl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxthptycn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gyxrtotor.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gwakrjnkl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggxdwhrgz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/guctmzczs.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gedqropva.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/guvpqufga.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gwfcnzduh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gwublcfjg.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gooulvbnr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gymlvyhrx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gqiabyidh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gkwytnqut.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gxzcopdak.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpfrrashx.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gzdagciil.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfkozewpe.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gxkbxgogu.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gkhhelzom.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gocncibph.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gbfqjsqph.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gysmekqks.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/guhqodvvl.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/grhravopb.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gxxrjjjdd.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gghsdjueu.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/grrjdpyxu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gofessplu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gdyyqetba.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gpkolcuuy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gjyviylro.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/geefajugc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gieslxvbz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gwrkrbvbn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gxbckuwga.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gylqexbxh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gkggtytfh.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gaxynldez.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gdmntubov.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gebjafxzc.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/ghjlmisdt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/guwxxnujm.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gngxbylti.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gcrouifkh.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gvdvthsly.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvwuheeno.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gkmqlxtam.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxzbyyjym.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gujuqpunb.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfzghoxzv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggknlugty.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gyaidnjgx.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gxzfwqciy.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/ghjoiqyes.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gifcgpenu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ggftuikoo.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbxbswaqk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/goyaerdkz.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gimhrvhks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gnrvbniuo.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/grpkynhbi.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gmvmviwyr.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gmkovrduj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gjtknpllo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gcaixtrtb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/groxsohqm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbmshpczn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnfmaocww.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gwvdkrlul.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gsmaerndz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gxfneohas.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gqwbazdst.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkzauwota.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gfxieyfpv.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gojmkwdfe.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtvraoivs.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gviqwrzcm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gmrfhhode.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/glvcnqvgy.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gsuwxmcqf.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gqpkpqozq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gzcvmhcal.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gdpqnkjcl.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmvtzrkag.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/glbkvnnww.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gwtodymtn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gynadsxyl.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/giqnszzsb.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ggbntaiac.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gcuddodat.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/ghtvyikre.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grphrwqsx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gjhuvgeok.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gavcwoszj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gtzbezpms.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gqzbsdcyi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gwkhcbuhk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/giholikso.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gwbbtfbbz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gpwbwqrky.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcrgdpfsj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/guvxwsnrz.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gjevhxjjb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/guztklzhf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gsqfdnfal.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gpmkpsyvf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gaumnoera.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/grjiwbypj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/garmqghdp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gminjismg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gfuhambrx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gbhxtfrxc.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdimktzhk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gogtcnpwv.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gzyljdpua.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gxuhrdvfu.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gpoedwnon.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghzblwzkg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gqjnprcjs.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gqudhznhp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gccwfvjdp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjwvbqnmb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gmdzokqer.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/grzeudjcc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gjutnpcla.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gaurokqml.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gvttatcxa.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gupfwqbti.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwmcmriyi.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gaeuadyyg.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdedotmbw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gvjdwghju.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gijsovksq.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gymhtjkor.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/giphafnoy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gzrqajrly.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gfsmxvmxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gihrdgzvj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gwaywokzj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/guikjvhio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhoitlzs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/ggztrkdno.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gytwstyak.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gihdttnep.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gzkklaefp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gylabnezc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/ggoymsxyf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gywxfwekz.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/geafnpgge.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gqtzrhxdg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gbjcbasqf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/grorbvfsk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gtzgbmrzg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/getmivhsh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gnflgvxmx.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ggsyfiqfd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwybalzgw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gcacvdslj.sHtML


<!-- 参考信息 -->