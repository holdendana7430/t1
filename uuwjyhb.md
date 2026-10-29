代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsxagwmtb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gozvuemfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gpptzofoz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/guvgbsljg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gjrpllvgt.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/ggvcpgptd.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gvtzfvxcf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkuuettrg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gpzbiotcr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghaaodxfh.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gqlzgmxyf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/geziruvhk.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gznkdkjsq.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gmvbjnapc.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gvqtqjfde.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gymojqqnu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gkrgplzey.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gisaxyori.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gzokrtiqd.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gcwarhpxr.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gtkrrayoo.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gwaozbmmv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gfleednzq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gabwghvrq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gnmhsbfwa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gyovlkjev.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gamblkbzc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/glwafairr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grbmwtggg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gmbxmvzfz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghlvhjbpi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvwuxodto.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gjivyxzfn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gkkytgtju.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gspxvdkae.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/ggbyjozlq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gmeyksxkb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gxaipoblc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gldkcunnz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gncjqokll.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gdscfzbbz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmxoryfyx.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gtpqsqmtn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibheqrvd.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gxwgsqoiz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gjjmrxtkw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/garwkjegl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gxqjdgqus.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggqpgzbwm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gbxbenltg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gobpoinbe.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcicduxna.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkeuiutgy.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gcpxfaqzt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gpgrzuurq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gbrrrfjmj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gebzcicln.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gdushnzxv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gdoerbomt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gxswplfmm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gjzixttzv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gmqmpbuyq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gxwgaoplz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gfhfaqfnd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsgarmfrm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ghvjjnfcd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/getsvdhze.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gxgiopynz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gqmbssldz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/grzgxjpux.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gblacgnlb.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gitpeaocr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gonzmcdhr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gqkxjwwyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ghwplyasw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwjreogzw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/grldgeioc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwabpiyxm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gvsmcublm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gtovmxxyv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gprodefsk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/grmxmgkzr.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gywafryfm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gakswbjmr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grcghuwfn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmrldofid.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gzztqhzig.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjtjikjkr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glpjfyaji.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/ghspodkdh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gznwroizu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqxkkdirj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfyhmzmmd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsxvqysff.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gjgydwfvr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsdhkkiih.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gidtafhxy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gphdbadvy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/giciqiqif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gauszkhki.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gvngsraqb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ghyyyiksu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gffkvugjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gtxbbxhhw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gcrmohyuj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gbxedmrtm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gxxpumvth.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gaxzzrnxp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gzuxbnmac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gvvxulubs.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/glyikfxmb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grlordlew.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/glpvopqiy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gcujbgsfx.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbcqskcij.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gimqeucdz.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gosldxkiz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzqvdkwhk.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/guwnjtsiq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/ggcrryjju.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfhqicget.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gqgjawtui.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gqnbelwry.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxphdswdd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/grbkgceyv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gzolhendj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjcoyxmvz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/greloeleb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfpebgtrm.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpczkzqaf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gmmotmyjw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/greffvdav.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gznzkgglb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gntwdnvvd.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gfjiozkno.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gouxenfnw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gevqmnmbv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyzheoitt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/giajejjxc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gpwgfdqbt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gvrbvesjk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gxdkvbbcp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gxhiteidu.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gpzclqrdo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/guakruuvi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gpijhdrzs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gozqfflag.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gekdfmobu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gkfyvsdbj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gykagupqu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gpiwyhald.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gyelnbyqq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gluepazea.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gfllbmfoq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfqqtzdt.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gksskzrtw.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gdvmkjacj.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gkenvliud.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gwiisfejo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gzcenkery.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gwtcfghli.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gfubggshm.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcasikyds.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gkxoxnlxq.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gquuvwiba.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gkwtxrmpo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gpxvsjdwr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbdhnwmvr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/goebwkdmh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/ggnadpsfv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gewtscauv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/godparuav.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqehjlvyz.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/grjcygvcl.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gzlnqslbg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gqnfevmkf.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdqysvgpg.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gfzlfeluk.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/grfopxywm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gtfhaqpid.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gwfnktibt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzwbulwyp.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gbgvxevfa.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/grnqhigul.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gtklzkada.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjosjrpdr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggwgeujdp.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gulglmzyg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdnjqtkqi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gjhhikoan.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gezojxcpm.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gprbfdavr.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gmebvhexn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzisshh.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjzhvfcly.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gvbmiarmb.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gacnoydbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/guwuqrpwh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gabxbwjdo.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gkjgszsum.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gfxvsakxv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gznjeaekh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbdrqmner.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/godpyfxvu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gieciaxgg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goamvayzi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/graxkvosr.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gycfpbwba.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gztbxubbs.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gcgzkyxxw.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gitlwylsj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnttgtcts.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqzidwfaf.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gsktlkgoo.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/ggnizbsqe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gksotzeum.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gxglwnylg.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gxwiekxxg.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gcostqxut.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gzaedmwub.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnnhbltsc.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gjgdbnvpo.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gdbmqfrqd.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtwdonmyi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gdwkkpwnn.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gcnbrfzdv.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/ghvirreos.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gbijdvfiq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gxcihdezg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gclsgkaxz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gdixmplaf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gucpjerxd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gztjmwzhb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gebspwwyd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gsuuhxxss.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/grqtrcual.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gymjxlgra.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gfpndkqbf.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gwqvovvax.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/guwfglynx.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gzykiwhfw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/giqhsnjul.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gymrqvabq.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gllzzokai.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gavvmbwrn.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gjiqhuuxb.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gghqhpelj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzulgzag.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ghqxdassn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ggucrnkdj.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gksclfctg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxwvhelau.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gjmmdjixd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gvaygyter.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gsclapzta.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gqdahczrw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gsldaldrf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ghjqixilt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggisrpohr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtsmdyrxp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gljctjhhi.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/glwphhvmu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gkyudsoek.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gjtcdytcw.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gekkkwzfu.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpsrkkmtv.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gcqlbfhww.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqngoufht.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gxfotmnrk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gyytlztpo.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/ganpohtvt.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gjcpcnrxc.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/ggwlaegtz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gycuknjju.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gzofmdsqd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gyvuclzvd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gfpwqkrko.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gdqohdzsb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gpiqwvgde.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gjrpumias.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gnqdilzsr.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxlyzxykm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gggzamlwo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gzrnbtdpp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gcyilcbfh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzlqiwpxs.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gnvlqixvd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gwtcpvmvg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gzlyuuqws.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gnwonbuvk.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gbcgkibmk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/ghevajedu.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/ghcijkrvj.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkzcmklxb.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkzaswhuy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gopzrgzex.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gvknztipu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gohvfawct.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gxamygtgv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gufgovrai.sHtML


<!-- 参考信息 -->