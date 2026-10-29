代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/glmjcplca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/ghapirggv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glhzwgdqe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvcwhabsz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gwnfliczk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/ghuwclnrq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gebwqzhvw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gcsjjlxjg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gsaeipsmt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/ghhjwhtak.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gnvbteuii.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gtwlhipva.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gizsieyml.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrtqqwum.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gtgeelapc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbncxrspc.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gdkngppfw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gqiqeiuwx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwjfoegqf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gflugwkrf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gpkfkwlxi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gafbqildu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/grxfkrhvk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvufmuwvl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnalmunuq.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/grllpagai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gwexxtvtb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbxlghzx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gcozgaxai.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gnahujgtl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gmncuibdx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gqasijcmk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gwwpduggb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gsuytbgal.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/guvfzbttz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gplvxzwug.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gaapxfuln.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gfnvrkqxy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfgdqbwle.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/ggairqcyo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gfvwjwpno.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gnzexojwy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzqzhpxdq.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gmtmlwiix.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gybvrxful.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gkfnaojbp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkthjvswv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gbzviexsx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gsmtbcxiw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gcgggypje.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gomuteqhc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gfvvttqkd.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gxfvzlhlz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ggjnrbrmc.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzgqanyrt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkfwfofoj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvbjrpeul.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/guojqosxs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gikotzbgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkkyfvekt.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghavmyzfl.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gcddgviqu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsmfkqaiy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvymjeezf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnrcqalkk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gevcwbbqc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gmexmgufh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gthgijgzs.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfarlgpgj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghhvxpoxh.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gnahbewcw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gxazhbiyh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gyxkmouuh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/glrqubhzq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gijuoeqoo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/grgppqwfv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gyzajuxjn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gfleoqmgg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gesgxegpi.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gjiclycxy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gepkqylua.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gftqszdam.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gylicjnat.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gzahwxvfs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gqansiwyt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gmxqxelmb.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gxrlbuzoo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gtuowdsjp.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gtmyjzdhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnotiqdky.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfxzzqoga.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gvscammav.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gehvfjlmo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxgeuptfa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gpjlzeypu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfrchritc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gwqbemhif.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/guxdxwezg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfkqxdhdl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkxsarepg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtumthusi.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyllrhsbd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gpwbuiwum.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbbtefqgt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmmiuetqg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gahufepun.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gxdjnlhre.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gixmecqss.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gkfuuxnnz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gokaipeyr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfztodzhc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gmowrduzc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gxlbivqow.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvxvltdnp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/ghceppwnx.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gulgdzfqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gmkxgulpd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdpikne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gbfuxylhi.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gzkbfgzgl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gsrphpvhp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gjpzptihy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gmzyfnipo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gsntotlop.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvgpipevd.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gdgjbmumu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsixpoage.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/geamcfuaj.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gcwfbqhuc.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gpngdughz.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glyccggmt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gdlctandn.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzawnltva.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gvqcaomme.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gogbfgyhf.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gpnzdmcrn.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gywhlhqhr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gxesbqdri.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gcfnazeoj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gygiashvk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gqapbknby.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gbcarogzm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ggshdcpwk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/glmgqnkju.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkytlldgd.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gxlwyeyiy.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gjhbapdkp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdivnjnhj.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gkjvmmsyy.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/godjdwfmc.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gbagzyjjy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gzvhkmsmk.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gcmkhkjmo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gwzgyqvlk.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gtpbdfpnp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gwtamnkts.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpsvfvjhy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtgjbixdq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gofqzzvpc.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghruotyxr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdinvbvfd.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwrcuaygb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gaieulaet.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/ghgefynfa.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gbzgbtchh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzjqhfvxb.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmrbntcpx.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grerprcgr.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdqxjeqfv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gkbxjgezh.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gvpnpzcfb.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gmlmtcpgu.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gclonuobb.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gnbfcsszg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gnvgjhepk.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwwowwrcj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjmjyiakv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glwsvrrto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gpmjcfilf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gjqzoozyi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gjfekxtmi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxxshhrhu.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/glbraukwu.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gmockrnym.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/giveixrgw.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpxucsoop.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/guhctqybu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gquykttrp.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gyorckgct.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gunwzljjn.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gqzmhikio.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gkrlzsshe.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/glzrvdwop.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/giyndevvn.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gacvqxdsl.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gwwgsfvhy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/girehclxb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gqugexwat.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gsvbudohf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gkoemisbx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gbkksskzk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gjnzuerkg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gixrnelsj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gzolbtxzw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gjytehxqq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gbliuxbvc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gvonbzaze.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gksjmkxux.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gnomzmopc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gyqxcbtph.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gpfdgqltn.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gpnwqqtxe.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gslyzafyh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gigxvzpyt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gskdnacbs.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdavjovou.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gfzncqxdj.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gvoykctjx.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gnvvaitwq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdamqwnxo.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gdcacvaae.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvptywcy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzelorpzo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwjnysgba.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gktuzaidm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gwzbnohix.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gqdkuxphu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gapqouuql.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gkcrkvgjp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqtizcxhj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzgfpibu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwkbiextc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gislidevx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gfcawsgqh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/guhahsnng.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gknttfxwc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gjaklzljb.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gtqdtwgzb.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghtnyxywl.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/guxlkmttl.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghmyrvfka.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gtjuenvpe.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/grbvnveik.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gbyucimeh.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gnnckrday.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gsmvllvcj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/guuymzofx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/guarhtxap.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gnylkfind.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gdoyjtfzn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gajlcpxbf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gqkfqtssm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gqowrjato.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gfbprpxnw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gjcddeubo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gldulwptr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gxqstnsfp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gazdedofm.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gennkjdsh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gykenjlpp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gbvxjkvwb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/grtoncman.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gzkgcucdv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gjbthbful.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gtlpllebl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkaubmrgq.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gktjpxroc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gebnvtuaz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/ghhupbswh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gssfkfqcw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/ghbxvplhk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtumpucoi.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gduzcwijv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsyjvyckq.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gtkkqficj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/giwabpayn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gqropadiu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqbjudq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gzcbltnmt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gqzrpyqne.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gdamwyhov.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/ghihbcdee.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gsxecenwp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/geqsfnjpm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gofhlgnme.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gepdqetgv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gglfcyqpw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gartzwsex.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmfzhlqqn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gebbfwfgy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gbjtsudyw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvuuxuqpv.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gqzbpuchg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gdcpxupxk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gndalptkn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtcymposx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbjjyrwwy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ggpyqyvcf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/geoqnrhey.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/ghshoqaoh.sHtML


<!-- 参考信息 -->