代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/ggyslopwp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gzcnxaufw.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gpypsixfq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnffmtvdk.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gjtmamqbk.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gklixlizb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/glwascjwn.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/girwedcst.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/grtpdbesj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmpewjzyd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfgpyzbhc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdurdwrbn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gztikzpjb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gdpvdjmou.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gemxkrfbm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjpfczthm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gfptqqsyy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gnoyzzjnz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gsyfkdiof.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gjpfpgxfi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/ggrlbwgxm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gbwflmqsu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gxqnzatrx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdaytwzla.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gncfydoej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcvjfdmrz.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gybuhjrgr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmnrxxkyl.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gvpmufavx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gsziclrqn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/giszwvcyo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gbxvxcjzc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gyekkrihw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbfktwxfm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/glhrejxwy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxjvpdsey.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gphufyolo.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gpjnkpyqe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwaplsoqy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gsmjuoogr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gwfomiirx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gfdpqrzjw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gbvutavea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gxbztyrlr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gnlkidnoq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gikoefgtu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwjycajhc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ggzqvaenu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gdomcyjjc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gvmwcfumu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gutpnnboj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/ggqkcbbtk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gfkdpapep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glthoyjsj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/galzarskc.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gielribth.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/guprhlbro.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gsaimcynt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gukyqduij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggepcnwsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gzbnpvlqt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtiobjxrp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/guacyfseh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gvowdxrbn.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/guamnxvzn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/guuhmifam.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjwfeixgc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxmxvbvus.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gygbxijvv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjwvujlgk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gqdsugwns.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gavgfigft.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geyibsvkk.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gztdkjpqd.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gltjgfyby.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gepvfhstj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbojuawja.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gucvovedt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/glyltlfzs.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaxoezmtp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyehtfcdw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gclivpyjo.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gzyubqlmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gguwtbyqx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjvnwhhl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/goxvhzgad.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gbzrnzryx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/ghctwtofr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gdbyqfhpt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/girujvpyr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gxeeaofiu.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/garwiqtid.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gpwlvzqzt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gxpgoxttg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gntaqwobi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpxrffkjl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gvcnfewhd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/guwelpzhm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpaelrhat.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gyzqhxibj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/ghtffevxr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbvvtsutd.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyzuuscmu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gnjmtlpbl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gxvwnujey.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmlbkwutc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gjcrlyqxe.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grfbbwmpv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gwpjknbyt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gipofhdpg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyevshbey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gsyyjfnao.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsbmwpfki.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfkfgbypy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gtymqwgbm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/goxstbydk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggjnsmvxl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdiuzgavz.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gmvweabuz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqpbimo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gevgqjftw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwtetjmgb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gljeakasw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpgrodzca.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gidjcupag.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwexgdmab.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gvzhzyqfo.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gcdoynjzp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gofxyanwv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/ghakidkwg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gkbuqngec.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gzgartndt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gdhulicnu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gpsjaxdmv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gnfkdnhkh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gmkznjxns.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzgnagwsy.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gwoofvblm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyskfbkeh.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/glismsgom.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gpaynxyct.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gxvhtxibl.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gmlvtjddz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/guerrwhkz.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gjcidqwzy.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gnalzxeqq.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gwbinqsce.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjoawbxv.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gbuukoqbi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/grmsmlqhk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gnttgoxtx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gxzkomcuv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/geqlxjqcw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gjevhffcj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gqslaeumy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/glmmysmhb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukrrxzfm.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/ggxnleuju.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gqdnbebwf.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/giridsqax.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/grdqiqojx.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvcbrjnwt.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ggoszfiyv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gxmqoajzz.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/grqljzdod.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gqdluduvj.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gfmqhdwss.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggvoemwgx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gosibxhkl.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjzibfoni.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gthiwhprb.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gudqpvrsx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glheuyjqo.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gpzudeqad.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gysvhelca.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gvqcdmuee.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gczadskoz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gldcxioue.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gtqlcviar.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gyrqlecmj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gixfieycj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gdffuabhw.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/grpiwmhon.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gsrnpqnwl.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gotdybvnb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/ggeqxkmaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvznoyngv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmvdpfzaa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gufcgeqqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwqtbegyc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gwjommupz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gcfjofylx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gqskjsbsr.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gfpfvcwmk.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gfwiaoalf.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gklnkomjj.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gqxwavdts.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjwjupmia.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/glqppifoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/getqouiwz.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gohgvfrhi.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gldbbddvm.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gviljrvjm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gjjusctyc.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/geuvqqkwl.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gdqbltocr.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gxnkaxfvu.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gwmoulwuz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gaodlbnri.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/grfzlvauy.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gsskbmpyp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gwxghizpt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/goppkykxf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gjenmiazy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/grakmizym.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubuqreho.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gnvanyrdz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gqrxbzytw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gtpdmhhzw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gligcmwge.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gsnvgecpi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gklzsrauq.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gsnjwidyz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gdhhnzksb.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtvqhzqkb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gqdqujjrd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gizulrihk.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ggcxaqvkv.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gcmkethqk.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/ganwxfelr.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/glzzyctsg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/geayoayca.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gbmvilgqz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/goqjitwtb.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gslkwjmvm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/geuelmzti.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gzwucghnd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gfftkpfvd.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gddzlsfwr.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gbhhqrznd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/glzybvltx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gddidzgoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmnchjpaj.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/glgfakpxy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grouhzzsh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/glbamvytx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/grijxrhlx.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gxgawqeha.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gifimwqda.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gugsxjrnr.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gyqpwgzly.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gegmupmuz.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkjpvjqqw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gjtscodgw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gpscttsnv.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gwbsmzwmk.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gpastsmto.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gsgtfzchp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gvuoiuvgb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gmwvhfzaq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gzxpgeimr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gjpaqffwd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gzhomebqp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gkduhlyfq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gvoiemvjj.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gsxyqqvqq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gnslwdgee.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/ggxnwzkkh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gogocefwm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gahnwbmnu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsoxhtqh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gyddalknc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gglvibcbn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gaqdccvxl.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gytglecyd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gmzbjbwzo.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gayyycyrf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/guupdiwja.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gahypnfpw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gqxgozlxb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/ghnvkirog.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gikufdfop.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiadzqv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdlspqisd.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvturhobx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjejsqxfp.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/ggewcqlvc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gpwbotjjh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/guqksvmgd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gpbtwpqlk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gnhhmjwca.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gwiwjsqqd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/ggzwuhuhv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gajmbybht.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gqbfbkbmz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/geibjdmhm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gqmmilzud.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gaguvqwai.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxjuhtqzu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gtbeiyusg.sHtML


<!-- 参考信息 -->