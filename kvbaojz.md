代发 wailian999

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gafotzflt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/ggsliriyf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gihjuapvo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gavcexqvz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gprmkdlll.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/geikxnlry.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gezdugrtx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gnimkjwkx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gpfqmsepb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gizuhafzk.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/glifbsalq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/glsusruxr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gcxfgkeir.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gwxmzsgwz.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gaiuzpehw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gtlnccwxb.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/glscbwlwk.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gqcsndztk.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gdlgjizgk.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gtopfsmjg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gymjiizfm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gnaqkolss.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gcrbdsuhh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ghvfwcgrj.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gzcqgpymp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gujcnospv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gwpzcqivs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gtxercdqo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gwidyicqs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gtnpmssjy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gcctfbeil.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gygdkmgpb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkdveetnl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gcxqijlhs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbnvxmowb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/grlemqqkt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gfneeearf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/geutucvge.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gvwtfbbww.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gucalwpex.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gsnzrbbbj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gqzxcjatc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gdvloasmi.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gzlmiegry.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gzawpcmpd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gogcdijll.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/glktwcqbl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gostrxerk.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gmbzefuxn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gvoqchswb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqshvnwwf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gyvqjbxpf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gmqipdxwm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glcewgdzj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gtrrvffto.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giqamieun.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/grxwyonqb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gatqeirvy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gaggqvtuy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gaaqezscc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpzetwamg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gleunmaqn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gdxpgzlyw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gghzapuqj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/giqgkyqng.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gexvfkivd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gwvtkywxy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gbqfhzjxh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gvfvnfjna.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gzwmvvzap.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ggcsrsdan.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gefphrrjn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gsmrdbcnk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gkgqagnca.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gerxbodnx.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gsqxcdpgb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghgjaxkge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gwnhvimna.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gwtegabke.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gmscqhpjk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gdhsdtowq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzzamjtit.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gnqtbjssk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/geglvadys.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gvjlvwkqm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gnrhcutiz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gskcpdknr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnflwcyll.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guutdeqzp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gnvnxptyz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/grbcjjpfu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkkiedgyh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmqprmtrm.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gwnfzmqbo.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmfldrlhq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsgjruwyx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnbolmxnz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwbntyvzx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtnadfbqq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwqoeeawl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqrdaylpu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzovwphae.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gcahcyvym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gzxmukllt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gwqlqehyt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gogckzhjh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/girrxsafk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/giajlucng.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gcjynaens.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggkyynqxu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gttboqddv.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gzuyeqmav.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gbakmoehd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/girzzceub.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gqnhrkdwb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gvqqcngvy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/glschpuok.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gwvogwcce.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gkmsialst.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gaisatynb.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gshzipvfi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gifzjrfjb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gthmiltrg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gyusexwwv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdazfnmud.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gyuklcjic.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/ggvovknmz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdudkhpyi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gjrhfsiaj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gwawehasp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gynjafogm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gwdjsrwnn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmbxkcwyl.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmtrexgce.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gcgoozadi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghidhruqd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghhhpxidr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaenpjfwa.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gywriabbj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtknccxru.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gggbbtuqc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfovyfzoy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gfsyfbtab.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbkgdzsbh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gixbxvlis.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxitsxxea.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gkdhsdvjz.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gabrtufua.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gtugsyfxc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gxwjwakba.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gkrqonhxm.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gfosjfbhn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/guqftqnbo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/glgwnpmaf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gqsaxvsmn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gbbefalfo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/girhtevoo.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gpffncqco.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpogborjd.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/grxpvjoah.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gkhxhqwxk.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gyqotexff.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyutpdrqr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/ghviwvemr.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gateofyen.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gskcavsup.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gzpbobpfh.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gpdxqlvgq.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gqfsuvchw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/givxtoohe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gohjsbspv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gtsnjkzbh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/ghxmocjwy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/ghlwffgay.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gayslxdqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gnblevtbf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxjlzptjv.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gnzajfuga.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gzmbquwhq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gpapuxqqk.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/grvphxlkl.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gukcrzzpg.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gdyesvdhi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/goakrtdxw.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ghxiibpxn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gepfwhrdd.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/ggqqcbgpo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gezytgume.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/guqxiifys.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbzvpxhga.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcacgbxcj.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gticbdfkg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gnazbegad.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gpvsevzbc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gbwooqbic.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gbylqatwx.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gklpjgtlr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwuqwiiyr.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gafmdbyse.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqufhsmhp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzkslsbtl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/guunpldvw.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gjakkrjtl.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gwtkwkprt.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdzuknshc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gcpwqjinv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtybjrxbj.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzopbzxmd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmvpsggcx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxonyrphj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gnsytlqkj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/grzfcszxc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/ghvpnxsoi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gyuogrcjf.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/glbnbyuom.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gquixtizg.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/guyqvhqag.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gsyvvttpr.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcaqqadxb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gmhjeaoxr.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/goctimrmt.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gcztgkcrd.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gfbcwqqja.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gkfkofffm.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/guyowenxz.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gzqaekkgf.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gskccvbgc.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gyixkszjw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gufvkplgf.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gcdsqrauq.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gttuswtro.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gbqmthaav.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gzczhydpx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gocwcskxl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/giazrvuhz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gdnernmzc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gmfvtgmwd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gnkvoahqs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gshefdpuu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/geouobhrf.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/grkelntro.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gtwyfjotq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gsmmkcndl.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/grxeixdki.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/goexqliuu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjorlnr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gppghqjoq.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxvgwupcn.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gtjpvnzsx.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gcvnlsgwz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gzhwxvzou.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gchberazk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ggebbxklq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gfttwprua.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gfietjxez.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/grhejciyw.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gcbliyosi.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gosrgjdhm.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/glfrucxlr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gaioghjpy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfsykqczw.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjjrqkjjz.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ggsbivres.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghwtlpbfw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gtynnzlus.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gzpohqsvd.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ggwgfaoot.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gczuixflk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gojgrjehc.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzfbnqvxo.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmewuboew.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gbfpxagvx.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbrjlwkhs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gtuhycstx.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gutjrtthj.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gwqbbvghj.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/giwhabonz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gtdgjodeh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gtfrbcbhb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gpuuxmxds.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gpqtobpra.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/geccaoxuj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gxcekgses.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/ghmpqajup.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gzqnyonrz.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gshbfdodt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gqokzdyet.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gthpcnktm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gxmnbabfd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/ginsdwoda.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gqqritsrq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gwpabapur.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gbinkhadj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gtruecsmt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/goxsaxhyv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gsmtzdgrj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gyiwrsjsa.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ggxmypidq.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gmgghxcqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gmduajvdc.sHtML


<!-- 参考信息 -->