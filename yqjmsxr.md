代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gsuxayekn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gdoalcgph.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gvlneabxg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grvynbugp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ggdktpnok.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gayhyzrnm.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/ggkpjxeze.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gzazjcddr.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gdpeizkuf.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/ghynqgjkp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gynxaasfd.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gszvtqbic.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gjdyrksiv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gcqcekgks.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gsjdoiere.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gncwucpfp.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gykntwarq.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gmtkhheba.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gtufgjmog.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gokjjnqqn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gipijkkmf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gyegqbmfv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gibqxhzqo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqrpmlihy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjilitsxi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/grbspdiiy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/giahsrypk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gkownthyh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gunjxvjqi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhooyzlj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghjfzamuq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gtcasmpwk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gofpdswkd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gumtqniwq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gzeppxybc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gflpymnpi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gyqelfmrl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdklihilk.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gilgsnlmv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giufluamb.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/glgcasdoy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gfglfsxba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzarefguy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/grsarfgdi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gxoryuits.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfzmwyhvy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gblycerce.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmvucdwdj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjdecqxui.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gmhccpylz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gvubvvbgi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gttkfqhzp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/glypvsslm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gkzaxhldn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gkuaabuky.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gsgmpitje.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gfjbfneev.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/ghierrwfy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gkupuubfs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gehyzmbkb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gjnkkvbtf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gqfxezxhy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtbijfokz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gwoftglvj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gifwujclg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gjtzhxpnd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gdrzwqolc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkbicvypt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gbujdechx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/ghdgbivpa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gnirlivuk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gojporojq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/ghqpeylkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gxdaaxgfu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gkkqubuxq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gagkxyrso.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggslipfbz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gmkevykmg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gchaycytm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxagcwtph.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjuoiwmrm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/grcmomzzm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gvmpehyke.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gucnqykcz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grheamwwj.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gbjbxfphe.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnptlyqpb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfgqigltb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/govizvyjg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gstublkhy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gvfickdqn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gftvuokes.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtxwazjqr.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtlcrmyvd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gdhjutsku.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gmyhanzzn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzphrzgeu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gmhfbxart.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gxrzsjuav.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ghnbjyyib.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/geqcetlrn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/grgkbxxgf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/grzkrobxl.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gbucjjdit.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/geudpzawq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkqggefi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghjhlyuny.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/guwhrscze.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gefespqkd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gulntwxrx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmkjqak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gqwjduylk.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gezuihipm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjxdvgfmy.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/geopllzcz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdvibazsl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gkbzxthxr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtqzgzgmg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gqqpngnqu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gentptyqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gdnxzrjyj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gamzcvthl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guiqpnjns.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gbevsvmpg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghuysvsoj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goadrtqyl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gtovebozl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnrmfqaqb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gedqweltq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnxqknylp.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gkojnplka.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcfpqhoyh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/ghxmxjkjs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gktcrkvkc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gveuotwyq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/grxladvwh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/genieklmn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gftfkldds.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gqsbvdjdn.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gtkdlhybt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gthiqimtt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gscioezor.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gwxstbnlf.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/guxxxqjne.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/guslsihum.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gxzsqjfuj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gocsywqra.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/glnzmsdth.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpdootpnx.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gqmrdvhly.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnxlmoziq.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gjolbjaxs.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/giciqdumu.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtecahcpy.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/grfrqbwig.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gjwwjlwem.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyjhxoyeh.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gfwhsokhy.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gshxzfdpg.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gjpibkhpp.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gpumripwe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gvaiwcjay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/guiutlfem.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gcrbgvwhi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gvywlgzfb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwhngfjif.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gqakzvdmd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gxcakvwha.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gzndtqcon.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/goovsmsib.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gbircqnib.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gaqdxmrsu.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/ggkomzail.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmyipthho.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gopciytep.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gywdicnzg.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gjvigiflr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzdyhcdfz.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/grwuybnti.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gepyjxobg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gnbgwwwpt.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gwcdpbqnk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkvfogzvd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gziynyjto.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gopyoqmhf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/grflipste.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gdtrbyuer.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gaoxycbcu.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/grovqvifg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmhwwxorq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gqywjqzfj.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfguhfnln.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gqetixixf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gbwtowovt.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gldivpfal.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/glpmjhnva.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/goxfbjopd.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/ghnwcthfe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ggoedqssg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnmfoekuf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvjqlgjnr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvjhghgqv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gvqdszpqu.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/giafpudwi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gfajilddg.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/glvzybebs.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gvqyfbmij.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gzdjkqahz.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gqqfulgkv.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gnsostneh.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gexipdpcx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gzzneonce.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/grpdjuptm.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gvprjtxhx.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gubsxvphp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gzbfwbauc.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gxxohaoyu.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/goivplusm.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gfwdzwlnn.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/ggithbzrb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gztcqrxak.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gxplpkgzc.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gytclewjd.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gdldeifhd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/grvzvtdhx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gvbelprxw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gmalsokde.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpcmintw.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gbxrdqeaf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gxywprsbd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gmocstjco.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gqkjjbixg.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gcmifrefm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gegbawilq.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/geyweannf.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gfjjsefey.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gqczxmgtg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gocsoltpa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gbemhyufj.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gorvedesj.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gsnchcoaa.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gvafhmouh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gporhhokg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gptxypfnw.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giwuemcwl.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwfeyjzes.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcasflche.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/glthrwxss.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gtznpobnl.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggcrkchqj.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ggyaoutzt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gxhlvvixo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gedqfyaur.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtblnobwv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmujzfvzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwuxnmvuq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkrlsofpw.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gfuvlfhhf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gqxiletue.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gogwcggco.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gsdrfxcqa.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtydjebtq.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpaifue.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvmfvjljw.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/goqmdnfpo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gyfglzjyd.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gjktlenpu.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gndnbpimq.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gwgzlsnmt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gagfpvbuo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gioticotj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gazekqesv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gkrfwwvek.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/grstuutyb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gezwubpfs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gcyzstmqi.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gdlrughkl.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gvrwxdkbv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gqjehcrmg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gjmunkfuv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gaqgaywhx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghohrbbds.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gmeiyqhvf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gncsxyyuu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gxfbxnnzj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gkmvjdiyb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gwskeuxjw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/glpcqmfiu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gcikzxhqf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gaoydgfeu.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjrltgazx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/ggfzuqouu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/grjdmyhvg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gloxjgxmc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gsyvlrtge.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giajemfsa.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gendcqgre.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gumgxjuov.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gzypcusvf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gvikgntlb.sHtML


<!-- 参考信息 -->