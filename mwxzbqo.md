代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbfecoccm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gxpqcoson.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvahhimpw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gdkoierpr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/glatozhyu.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gntqxwogj.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gyvisnxof.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxtilsdrt.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gyjrjvjbt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gbvhqpdjp.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhnhmmbb.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gvrukbivr.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gasappkvq.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/giyrlvbar.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gbgafwiuo.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gsjhjowpa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gdfemaiiu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/goyrmnafz.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gljtupnwk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gtjpkxusn.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gnhiquugf.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gormzeaph.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/guztbtfcf.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gqbuhabgd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gproypqyw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ggcqgmqjx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghokfwbst.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmjkcwmig.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gmvszayks.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gcahcerxy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gyvbsjioj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/guiqzurvs.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/greuuujhi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/ghwzmfptn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/goxevvhof.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnlqqqlfn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/glcmbacyb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzaybjozb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/giszdirfr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gtjqvswgk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gixxxoiql.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggcilroms.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/glsoeziud.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwnhdiyue.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gstekdsaj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/glunggyxl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtluopphs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/guvbobnpp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/grxijazxy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsdrqnysj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gfzsuizbc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gatlybqie.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtqkrhmda.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/glbqwbyyd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gswvaowrt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gjexkswkw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkwcneeaz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gdgceuuor.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gykwkvlse.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gsggukvpl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/ghdiwkhxl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/getdkqwwc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gyzrhoqtl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/grimsohcn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gcvuzmnnl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gdztgvhqc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/grjvguzdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gucpxcabc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gcnhtcxsn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gdypcgkut.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gcuxlhcfm.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gmfolyicy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gvysqjokq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ghghldbrz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gdmtxzsmp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gvixbfrkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/ghgxjudnu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gybutxayh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gvhyehtro.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/guojxgafm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzaviudkt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gclyrftdu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnmbjpoft.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggocxjieu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gchdrzndi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdsefntbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gyeizgyok.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glmfcdkzg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxppqjrmc.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gpstpmphq.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmxmshagj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbwombryv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/glritpked.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtdlpfyeh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/giirjgkrc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpzlaliip.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grfevcupk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbcivsnlu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gliwtmnit.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/geyvbwfty.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gxdtqntrd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gznfcokre.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gjokxowam.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gbarukrbw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/grzclqiln.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gcfcpdrxl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gykkpsbwu.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gvgozukgb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gnwqrsnak.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gpuwswktx.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/guvevobwq.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gzvbpyapy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gcdepdzxb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gkixnyrxh.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gcxqzgisp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfsllpjqk.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gffiuwidj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyuambbai.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glwiccmyx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gpevqyysg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gjxyvisdw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdxztzlnj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gbvnjtyfr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvdslxswx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gfrbsxzyk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gdpdfrlma.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkucgkoic.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gawnozwhb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glkagfygg.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtbexqfde.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gpsjnhbpy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guvgetxol.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gggprcocj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/goekpuqmu.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gnywsevta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gavsevytz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gyrvmxvuu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzcywsxxo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqounqihj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gchfknhos.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/ghzcselfy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwhvrygqb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/glugzqpgh.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gddeaeewp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gfhkfffgc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/ggbngytrc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gzpkfxaua.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gpzdvjltl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gnqwgwnrk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gsvtpvcfb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gliaqtvlt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gjpypxrqm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvqqsfzfv.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gtzscedaa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghhqrlfqc.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gbwqaurai.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gphiaxmbp.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfrqavtmj.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/glrhsoqfe.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gzoxhmapy.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/grzppkrok.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/goynhcuny.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/glbufcuyp.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gxcyahlke.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gsvcescak.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjwbdcttn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gdrcpnlve.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqxolqhgo.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gkbtaxczq.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gegfzaixr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/ghynccuxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvrgsstul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsmdyxlkh.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gudwoqytq.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjoyyjllk.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gbicfmiad.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gctammzhb.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/ggowhwtab.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gwykahkqh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/guulrfknm.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gdmeltrlz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdfpnefln.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gmeccrfpg.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/greduqtnd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gaggmpvnl.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gacenmwoy.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gghgiflrd.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gylihdtoe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gvomjadix.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gjpcyxhxu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/ggbctfcsp.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/grnkzmjwf.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gnbjmjypi.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/geknocwdi.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gcgrzchqy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzwltbloe.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gxnhzvrmi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gasautsaw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gydybhpar.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gvxukjbtx.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gfluxplqg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/govuehzhi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvlcpnbdm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmhthcvoz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbrjbfnfb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbtcnemqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gmjrbjhab.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gmhqxrqzu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gyayzpgsp.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gjokixevm.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gkkvcrxgb.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gaerxnxbm.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gnryjhoqp.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjfvvepsy.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gwvzolywg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gnwqfvbne.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gapkdsjpt.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gsfaqtjua.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/ggftyvrtr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gkbamdned.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gqtkyltaj.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/geammkxlk.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gwckcsrja.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/grqrakpdz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gounhqwya.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gujudqrcb.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gxgrplrvu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gxhwfvqax.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gvvastekk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/glpdplcol.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gtuvlaaag.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gmgkztpff.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gdfeiroob.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gekrjjpej.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/grqyccxpu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gykuajthd.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gnmqepbcb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gomysycub.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gpgcpshxd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gzhmsrpdd.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gnpwtgzbk.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/goqrtihba.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gvyukanig.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gupwqkqbk.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gpgpcrjcl.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gtzobezbb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gnbsohxqe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjqwhuwia.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gacrovdxz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gjuwtdckp.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/giymegpia.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gznukusds.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gwkczycsq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gleqaobfu.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gsdhuqetc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gvshbgbnz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ggogbmvgc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbkwgpscz.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/goffrkxzi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gthktqtxv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gxckhhngi.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/goqsiypgu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gfediscmj.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gbehpfnru.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gzudwzkwm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqcmxmb.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gagcmscra.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfeaxzgah.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gglighjlm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gnapsslen.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gtldjyqzd.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gwwzsahxf.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gxbalrcji.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gyhzkdusa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/guapaxykp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/ghrwofntb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnwmqri.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzedflp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gjkfqscej.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gdtbmktnk.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gngawippd.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/ggdprvdef.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gptzgfzua.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gndesblhf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gxsyxlxwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gxiytereh.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gsabcebml.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gotxscytu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gzmyrartu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbcmeynow.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gkryarjrv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gfbqecbhb.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gkghnrbgr.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gnyykxwtt.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/glnjwjkhf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gjsgtjyog.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gyzcxctyc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gpldtlnga.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gtlutywos.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfqmhjcfc.sHtML


<!-- 参考信息 -->