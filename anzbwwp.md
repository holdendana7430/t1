代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gqhkhmouj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gvvzknobh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gaymvfeil.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gkohyzflp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gqmbendoj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gfjmxtmfv.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/grkarbuaw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gtdhylvbm.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/grcdieixa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gfbnjxzxj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gfqlqlzvy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gqkjagflt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkjfngpll.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqevmxhau.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gaklfhrjb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gpvjkojvp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gkymdkzvl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gpbxnahoh.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gappbrkko.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gewnnlvuy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkhyjfktk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gnokevxss.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/grbcxuujh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gqsjnluxo.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gkvsvikzo.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/giodjtgju.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gdkblmhpd.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gonxcpkmz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/ghrctouiy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gcqvdtrqo.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gmjlwtbjk.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gpbcpyuio.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gqlxylxvv.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gvzlxfgpy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/grrbklwbq.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/ghzofduao.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gfhlhrxpb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gayhonasm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/giydjrpor.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gizdocpwq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gvlzhzegh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gkygbavri.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkwzprcud.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/grqrdkfbx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gyvhscilu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/glvmzytin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gzwhudoaj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gmgtrjneo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbccsfebb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/ggsfpwnkl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gbskvahgm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gmxuqybbw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gyylztald.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqueirchb.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gihsysfqe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdxunlooi.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gukyttpfr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gtrbgfojf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggfzqplqd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtftyfxih.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gyfuzwwqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gxbrucoon.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gtvqknyni.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkbumrlau.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbuqeofgv.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gbvhffbdt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gnfivxugo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvgyuer.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvkqmklbg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gdnsqpqge.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gskuzdcwg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gshveidyz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gageipghr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/guqyyxdnw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gwobiytxn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gzttzslue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/guyctxumk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ghmkicdri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ghwnsexrj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gfrnufonv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gwkaquyba.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gbivldlrt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqogzoigr.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gktkanxhx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gdwylsplr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmkjenzbn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gqoscytaj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gdvmkxwrf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gxsliusdu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/guevfkmbm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gkwyyeqyf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/ghevlzing.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsvplayrj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gvxbyfpbg.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpcisbdgz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glsmhzaui.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyghjgwco.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gygrzkfel.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gxjyddaos.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtbpflitf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtgdqzjyd.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gfwihwexs.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/guhkzjkqm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gumkaspgy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gawdqnwxf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggkvopopa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gajwlrgox.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grlavkfud.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqktbwpuh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdjnujbmw.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gyxfsbdfw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gnzqolqfk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gbafqhfsx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gyafummhz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gkjmlfukh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gxdaeehrc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqafzhoo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gazxmtuft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gexmvewqr.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gaywoocqh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gomdcjwgu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gkkurkmne.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gtctgiggg.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gpyabfsgx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gjooajsvb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gwemyqgir.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gqmynehkf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpzznchhk.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gzqiixrfg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdmagldry.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnpvndhbo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gntuwdujz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gflpfdavc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gukqcsnar.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gtioedlht.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gekyxiwvg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gdqzaexws.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gqdzrqvvm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqhqwtjhx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtnixntsb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwujxaatj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnewuvhza.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gywesmoxe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxoreiggm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gynluveva.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gezlsgdqr.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gwkzilruk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjhvphvxm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gzwuggtjr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gfgccvyky.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gbrkmtjgu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gdtotexck.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/guxylvlys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gdrcvasha.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gxtrceakz.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/grxbmiebr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gljedxdwz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/grmacdlbf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gbchhmubi.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gsheeupjh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gtnzotpuw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/guinxfvqy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gxwleyohf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gfmjbnygv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqknwwnjf.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gdknvlvol.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvaubfrck.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gpwqnegjg.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gpwzztvny.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gzxnfbgsq.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gcyukqcqu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gowwmbvdr.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmpcrgbyq.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gyaxgbdvl.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gkqwjlnxv.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/golojjzzu.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/guvrxzdbv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gfbknkjmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gatebfwyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gdddlzlrv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gjxsxgmil.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gnpvwwxln.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gudlwpczm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/glkwfbpjs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gddftmlld.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gejipzskt.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gagmmrbov.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gkedlmsca.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/guxnyzraf.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/goneffdzp.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gvvxiglxn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gebxaxaem.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gkzhuaqux.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/ghsmmgvhj.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gbcnboudw.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gjbypyisw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gmwzaflal.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvhdumsqs.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gekywlvjy.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmcxtgzud.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbhtggept.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gukxgdqkj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gpojpqseo.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gpqofvpxq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/galimurgo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gndwispdn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gshjstcnp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbxsfki.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbiycxryn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/glwgvcrrw.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gubcubqvz.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gkgrmwxnb.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gnmwlkgyb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gqzpszjhw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gcyfavsul.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gcornaigt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzjuszban.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gnytuaywh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/givuxewnx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gzgbzobms.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/grwffnclx.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gveuvivha.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gmxcwfjga.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/guxgblrii.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gxsurtfht.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdswntllh.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gwpfsugvf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbqfbkq.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gcuhacrgu.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkxmvweyn.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/geesqjsgi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/ggubuofxv.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gikqysohl.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/grivditkj.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gjqlhvnkp.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gltggnmlo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gvdfxmpvd.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gnbpxjfmw.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gzkfyfjtc.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/giklqfuzo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gqrijfilg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gzbdwbqxz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/glqiswula.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gspxtxhzu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gwlogwqpv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gzbnjgisq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ggoinvidp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gkysuypvr.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ghurhislg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gkrusinqp.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gbqmislty.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gghbygwdh.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxnkawtcp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gwpuqhvwo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gpbvvtsjw.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gxzcolxue.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gxbopwxrv.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/ggqowdngx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/glbqwlzvz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gkitzvhct.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gzyxwckjt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gyzbdprpj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwgjlgzns.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gbvahdogv.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gnyoniagy.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gmqcajbrp.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gcpibdzwc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gffssnaiu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gybxzowrc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggogapssg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlsiomq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfzzxyzk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grdapopjd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/geacxbecv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzeshxh.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gwfzjlbhk.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gtsyrvjfj.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gtlhpvsir.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gauwwxuqt.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gpctzkjqc.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdddlsxlr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gzcbimzqq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gubgupbzv.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gkmosdtwf.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gengdkdft.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gnubtkrkp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gmzaqoyjh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ggwhrtbdl.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gttubaygi.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gddryqjme.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/glasqwztj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gvlqvotjd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gxsctukyk.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/ginuwamyk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gkskhdvgr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gxpilyzlo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gdyhubzqa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtfvynwrx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/ginzmquyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gwucllwjd.sHtML


<!-- 参考信息 -->