代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gjpbctgwn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gjxcxhrzq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/grlkrsbiq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gchwhvsgq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbpgisllo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gwfthcrsi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gkcnksmhg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gomctnybu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/geksdduja.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gmseayehl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gifssdrgy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/getwfjycy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gqmrbvxno.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gcfvxdvxu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gmpnnxtwl.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gryyelind.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/grvkappna.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geoijhyqv.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gaphsjebl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkipqciql.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gynsdlqfi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/genvmnpdp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkqwdppgk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gvoulpgeo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/guewknnem.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyezlovft.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gjoduvyca.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqpjpqpue.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdaepxlnt.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/goglxnguk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gzbgebmxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gsxgwemkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/goqvgomwo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gnuabyzdc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gsrjdnayf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gdjdoziiy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gpcdvwtbf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gzswxsewl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gysvmjizp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/grmcdxrux.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gyddzthdx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ghyagnijn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gfgoeuavb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gdbfvipji.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ggoayptqw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gulvnugjp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gmlregmyp.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gfgcgjpkh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gybyiszpr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gzhvuuqru.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/glbhjluus.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gtyevggyo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gegiisest.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gjtdektsd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gwxecfbzy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gkudrfbqd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gbgnukgiw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gpzrccnak.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvihipjta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmizesqev.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glfpanvwc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gqfbzrlft.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gyoezltsx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdfnxypmh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/geuyvwtph.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/ghpfpmqlv.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtpgmjbxb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjykgoyep.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpfgyrwab.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gduobimky.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grujowdjo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdlpeivbx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxsehpebs.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwspqniro.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gvimdtjod.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/goucuqbff.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gzyamjqlm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gbzzjczbh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/glhccunta.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gqzvgmdry.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gwyvqqtlv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gpaumhwig.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gjnosmesi.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gvykmuond.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/ggrwqruid.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gubnnwcsy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gziojhlwg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/griulxncl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/glzkjmspu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gvebygnio.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gjjlxkukr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gcvjfdqli.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gcohergkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxitvczhj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwotpllwz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/groakluuy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gfnkiyvod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gdgnmcwbu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gqgnabfbe.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grfxiooxc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gawrirkiv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gdiatpuwb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guhmwcuiq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghwyukswb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glsbpcwux.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsvgqhkcs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gcbymzcvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyrhqhsrv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmtphbfzb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grkiotufn.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/ghzxxfulh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsdcvyrnx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtfthmpbr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqehegqlh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ghkeliixy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gyhsumnnn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gxwnakvdz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjpddqmzq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gpiblaawu.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/ghixmvlzn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gmdluufts.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/ggyhgnrwq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/ghpsdmxrz.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gzstqmibt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gunnkqkoo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gjffgbjsu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gxkmxgzgm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gmvxrotoi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gndyqtlds.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gdmqzoiqv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnodkmodx.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gyfyrohny.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gujmavkts.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gmcgfnfua.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gehksszqh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gfsoarbqk.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzqyppwig.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gpeqrtgrd.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gdvmpfubt.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ggntjwekv.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gnprmggeo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/goyasegag.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ggothivhr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvdzoyrei.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gmccvxbnc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gmcqmfckf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gqetqfusa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gzgnweojb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gpfhlmuui.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/ghbaatoii.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gtnzgudar.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gdcfdbprt.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ghhuxczsa.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/genrgcqho.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gktbnrtto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gguckcbrz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpxfalo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gsiniqefr.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gqxplbrqx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gwuzfqmdd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/girscrdav.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghptljikh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkiwlceur.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gsnkfuecj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gzgcxssma.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gmjgcumbg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gxqxlruet.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/glqntttfz.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/ghpyxrcxs.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggpswjawf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtlvllnxu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjucmmive.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gkpylhrqz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gdrnavscu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gkpcsfscg.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gysuquhum.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gjkpkceuw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gznvbwiwe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guqezclns.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gtrgrojpd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghzhqpjkj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ggiwxmgwc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gmribnoph.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gybytjrzu.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gkszawfje.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/ghwrmxxdk.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gqxfwlzbm.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gefopyijt.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gcykcpmfl.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gqtfkxgvf.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/ghtplnfqv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gbmdpuoyw.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gkvciirxx.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gfcllxplk.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gjkjipmyr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gxhehqqkr.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gylopuvav.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwesxpcjo.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gunmxlxff.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gkfvdizrq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gskhzbsow.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gdtlepzik.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gnnyecord.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gobizufkv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gbhdotlzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gjrpiywap.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gqgtqxiqp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/ggmnhelxs.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/grqtkkirc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/goftcjxii.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gukrmsesn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gmvvuzqkm.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gbvmtjhet.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/ggloerhcy.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxudebora.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gfonsztzj.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/glyayryuw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gxzkiwfge.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gvbqohsot.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkjiafzej.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gwmecaskg.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gtwhettge.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gdlpadphh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwwxiyrcb.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gngzgosnt.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gxpvyymjb.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvweenkzt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gfzrrawhs.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gdtcvnnhi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gaotshnxs.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gwerruuyd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gfglsbfih.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbmabaqsk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grbqgpbxn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkrrmokop.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gtvxevaki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ghzpziwaj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gfefpfusa.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gbowypwpt.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/glztutwhz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gnnwdrsjq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/goirbkcof.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gbotqilcb.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfuopqfbk.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/glaxigxwt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gtefkklyi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gyfoxkjal.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gqrkohxmc.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/ggfajgeqk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gcndfxiir.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gaihufphi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/guztjbmqh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/ggonuwbqb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gfkyqazqg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gnzzlvjao.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gfxrnkcvi.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gmjgjonwz.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gankfembv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gytfqldqi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gyetpvtac.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/goghemnlr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gvjunajkd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gvgrspejt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gurpnnccq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gqqsirxup.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/ghpyeyuzu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/ghailgtmj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gtqoulxei.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gbxlcihjv.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gwapzkzms.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gsljdhmdn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gqifhoctd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/golshgtrc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gcqwudkvs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gmgoxqvoe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqobrvkef.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gviwxpdau.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmealxmac.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gtbggsnpy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gvxcccxsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gxeviwgbu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gwpdhwwok.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gbfhoctaa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcazifer.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/glhmowmvv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/grxixxxcu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gwcjnklmd.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gpyodppka.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gfsmrrwti.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gxakwrrdb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfheatusf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/glgggczhj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghfigrlpk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gifjxoudf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/ggtpkmgei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/grulmxmtn.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gvooeopep.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gxbmeiyoa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghysqomlb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyzjbvjbs.sHtML


<!-- 参考信息 -->