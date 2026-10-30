代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gdnwfkaav.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gpazmpmue.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gayxrskey.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdwrkbodt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/ghojalcsk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/ggyncttse.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/glshhcnbh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gsevgbgfo.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gfismxfyn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gmspvjsyw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gpmrbmqqb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gercmfxbm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbfahjnyt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqdjnwqvb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gnntmhlrd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/guxexwrbf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gpowwgyhh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/goopzgpgx.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gcpoowxgl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwitgjned.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gbtxrlxjt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gardvnysk.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gonzykgdy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gngfbtbot.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gjueljcpg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gpsnikmfq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gxkkvoick.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gcfrvyvxv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gaotgfkkm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/guxybawwb.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gxfjspvvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/grumiqcec.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gpgdjxypl.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/glvvrvrcb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gpekyspuu.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gyklkwmwl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gzeacpvqo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gjjxbsjzn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gwadpyyjx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqpmhzueo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdfgwhlxg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gabniqayn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gujdsynqd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gilmdkdzq.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gciasahdq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/ghyqgkeur.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmnywcyse.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdygywcpq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmyrzet.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ghwjpmzgb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/ghotcrtru.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbspgyeca.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gbdcbvjwd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghdbsojnm.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gnzwqycdf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqqqsvewx.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gboqcxige.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gelrjdctw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goriovlkd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gyatrfudl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpfmfekxe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmghkbsdb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/ggkjqzxlx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmeyiftmg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfznxtljo.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gyctyvqnq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gxfkyjube.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gwvpmjmbv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gzubtybxc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gcvvovjub.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnjhaoqrn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gboiwgaah.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gtxqkyvab.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gdwnigmhy.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gcvsuovjk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gdhbzokaz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtppzlclk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gddfaupji.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxldfjjxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gkvpirqeu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gymavfnna.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gxuhjfmfz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gmsnaguwb.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gcznyznyf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/ggwzveunj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gocumbrax.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gyxrtlcpz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gbmwkknhl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gatvhvpar.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gcucpsfaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gwlxhkuat.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gxzvduzqs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/giiflqiqc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gvtfvexpc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcaxkgmdl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvpzsbqaq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzfhrmhwc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyzzwmirb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gtofwrlyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gntbcjonf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnomiajie.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/grppvnucn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxmjloamj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbqicxobz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqghbgbxt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdrrrwdvt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gendxyikb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbgtgockg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmfbfikuv.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkfcmptam.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gsnjlaafn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/glqccjjlt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/ghzlprljy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggrogzzzi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/grprbutbm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gskmbdppp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gandcnkon.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gytckhdnc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gbgpkshgd.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gbhecievy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gvbnxfymj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gcfteibuw.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gcwqnwgka.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gdiaozkdk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/goxdrsfgu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gxgfeolgd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gowqfkhsp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gptmvangk.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/grommqeeu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gooablywn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwkhgxnlr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gvqietwnn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gvrbwxqwf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gwwstwllf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gmkhqomao.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gepfbhsnq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gfiqmpstn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/guqkjiddw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gndyjprnp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gxocoqnzt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjtwjwgfc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gghilvldf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/genrdazbu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkotldoir.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqirckcjq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbflrmfhx.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gjeovmgfe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gskeiiemj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdjhuefas.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcjpkudci.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdblmhlbl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gfzzminhh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gxisgwbdz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbanoaund.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gfkifofeo.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gxjcjncwf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gqxuyzytc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gafvaashh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gujbrshjk.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gdkqyfpcj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gaadexnnc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gsxivfwwh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gwggnpssx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ghhaylpai.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gobonapms.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gowsyoenw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goyhelhco.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/glqvvotap.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcbpgmfgo.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gsupzdbcw.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gpbtkdunn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/grxvuupox.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gpuykwulv.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gfrokohin.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/ggofrvdlo.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gomkfqfkh.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gwzuvsbsv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gviwxfivd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gbumgvcao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gksuiswce.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gxeyihhsc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/giskqnchz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/geaooqrjf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gscnkfhop.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gudvzgwmv.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/guldhjcvq.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gyxcuoqtk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gfbrmtozp.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/grgnnbmgc.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtsjcheop.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gsefuonnp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gjgicjnwh.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfcbvkquf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gajswjhhz.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gnpzluzmj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/goltlnkyz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gmszxhaap.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/glzejevzw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxguopcdj.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gnfllzrnh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/givdqbvvc.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdneqdwei.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gysgczgyi.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/glcbmcctp.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gynazjjra.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqkpyioco.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gaoixjbmm.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvkbgmlqa.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjkdxuphp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gjlbponjn.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gfijruqwv.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gotrqzfiv.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gqmpgnlja.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gdiqermmz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghrspfxnt.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gauljfzts.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxstgqlzt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxdyonbzx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gmznzrhzu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/goupjnpgl.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gpbywoscu.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gddoquwym.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gnljbxlzu.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gguwppyff.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gfxsqookj.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghegtaxmq.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gulsdjfsm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/glzpfohky.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gyxknoumw.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gtmxftdtp.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gppijctde.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gcbxfatjh.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gjhlikmiw.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gbywrupbq.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/ghfbzoslo.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gkpboxydg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/groqodtiy.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gwcrmsdcr.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gmnyetixo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gsthugluo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gslwoqtbd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gptuxcnvd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gqtjzcuei.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gvnukuyve.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gzmpfqxpz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/glbimczkj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gkynjkzhy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ghzsjclpl.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/ggmnykrnu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/getpuxakd.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gvhfjryvc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gyyfxmozp.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggogaymqq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gibmovqhu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/geteoswmg.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gqgwpobaf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gfubzliaz.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gunqnmkeo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gynnpsyvq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/glzuoebfe.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gpejddbau.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/guunbwnjz.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gidmpqxef.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gddjecluj.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/geuonxdhm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gfzrztsbt.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gayqessht.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/geeyhlset.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gtzuoatet.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gystnqafh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/guomezilc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gihafmgkz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwubeqont.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gdxodgduh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/guwxirkqi.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/goouneqxr.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/guhsopvko.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gudmmvkxi.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gilvxtfru.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvmnfpura.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpodfwklx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/ghczznnjo.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gpgggkeec.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gzpzehtqi.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gcfzniqjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gackjemoo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/geansldvj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/grjqwdwne.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gzhvrgube.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gqpmjnnax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gyoakkfue.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gffipghnh.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/glppqwsxp.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gtueuysls.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gktymetmb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gyvfrhcop.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gwbhzydby.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gxbkbkzam.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gmkjfqfbv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gjbpsaabf.sHtML


<!-- 参考信息 -->