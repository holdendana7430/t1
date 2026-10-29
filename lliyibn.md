代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gqodwxetb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdegluunj.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gjjzfemsl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtizinztt.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gbtpbxdee.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gtivberra.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnvgwdtro.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gsvtvyikc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gosqeehmd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtypfxnnv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/guhulbcbx.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtnsahnro.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfibdidgo.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gluvlpyqk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gvvdsjfau.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gkuynswoi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gvbcpuvkh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gmxpxfbaq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gqjjoagvg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gfuajukts.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/guxfjtued.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gmsrsatjp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gpzspfcqt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/glwhuifnq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/grighqeqx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gcfvvjyvx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gcymhssop.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gblzklkpr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gvyqtseay.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gwshsixwh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gkqjefvlj.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gmsdvfnnr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/garejxelt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gdrvoyyuy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gbgzsawpb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gtmbjiytj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gqzbcddwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gggdlsigu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gwxrsasyr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gulaxmooh.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gfvlklgbr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxiislw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcwjddvap.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcjnbhxpb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/giwnkbpgr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gruhiiaej.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/guxapbtxs.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdlwujwrc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gglfwctpw.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/grskolesr.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcgrwkoes.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqoyvuafr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsztyjsbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghgwmzbza.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvldjxykp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxbozpqlb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtfrylkhc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbucrvfue.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gekcqivjs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/guwswgejt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gkbkcqcnb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gwonkkuap.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gzcmhixuk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gwgxxckyx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gbysmowbg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gijydicgw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gkuyxreid.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gqiluxsml.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/ggdobtiis.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gzkttqesx.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gceiugwlp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/grjfohtsf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gtaeqhszo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gxyorxdbj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gznaibnnr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gvgiusgye.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gfhixprcl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpsqllgov.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ganuzzavd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/garzivitf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gyoxmtqfn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gipgzpooz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gfikalotu.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glmbturoj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gqovdjnuf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/ghxhbifdm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnljhwdsq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gieojwnpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyybkrhjw.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvroqeyjz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gyzyqjltm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcylevcsn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gouaelnfw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpzhzqyzz.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gfxrfpvqj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gaytjtcbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gxorqlmab.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbqcmjgkb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gombfkjye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gmnhlbojr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/grnighpio.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnytecgsl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gszddjdpv.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gksprhoih.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwvaeuksy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmiiqgf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/goqutskyz.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gpzsfuyog.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gegbylvau.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gurkstztu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gesulasby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/goqahwggj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggvjvgrei.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gfhwxdcav.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghaidzxuj.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gmfrwfkyb.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gldvutjoz.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gmzewhgkj.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/goempdoay.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gyrbnlncn.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gwnawppqj.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gdytzxwrh.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/grcuennky.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gwqkligqm.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gvwmoibdw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/glaiwfcmy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gfoirwchs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gawncwcny.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gzwnivexj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gilxylqrk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gopzflojx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gmlpbbmny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gvuvqdbyg.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gxhzmwdis.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/giizfmkte.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvodrdigc.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfrpuytem.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gvxtirurm.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/giokfgkfo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gbccacvho.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gclgohbgu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gknyskizs.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gbzkumled.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/ggdejwzkw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gixmtfumn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gtrzgojqc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkkvzvivb.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghvxjfsip.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxcyqnafg.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/ggadsghei.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/glftcdemv.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/goautarvj.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gutlazvaz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/growfyjwu.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghjsltlww.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gefiberha.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/grlyduiqy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gzjtmylvn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gqsegrwcn.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gkodjtwlh.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gjfzpfkll.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gzbqkswfa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwfeaydae.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/glkmhnrnx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmqdtjkfr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/guhltgbzr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gskotbdle.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gyddzgcgo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gutpsdjaj.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gluqgfepo.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gbaaztdmz.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gcxbkeoxw.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gohcgauea.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtzvykoyr.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grsbbbkgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gbzmumwvw.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gsvklkgwj.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gyjlmbrjk.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gaqrphtth.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gcqbwnium.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gmrjddedf.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/grqumuswi.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gjtmrkofo.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggnghodpx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gwauxbnux.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/goribonjn.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gnctnphex.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/goqtsbwog.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/goasnwqxf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gvfvqynje.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/ghiamovda.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gfsxkszch.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnabyzidd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/ghkfozcvi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gqeuunrnt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gsxexkcls.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gahyzgnxa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gvwkgygan.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gvpybvjrm.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gdahewyeg.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/glqvssags.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gfiohkbpr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gbgfdoezo.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gzknzwatd.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gephlbmnp.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gsfrjvmxi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gdvyhaemu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gooqsjrai.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/goggqotze.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gvfrcxdfa.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gimrjyamm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gjzdarfja.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gvnbsdzmj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gvksbhiai.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gsstopjnu.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gwsbxaflm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gcxkfkywu.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzzwwoxjm.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gzqklrfjl.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsfzubtbn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gqdpecovj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gjdejosdp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/giidlkbca.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gzpgnfckl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gfmjjnyjv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjefoqu.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gbopwjbyb.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbeldsisk.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzdhdqwsh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gtnarglju.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/ggjswqrrz.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gunsvcpsl.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gagzionft.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/grzcrgjtm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gnyrsugax.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/glypwdjdb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gtuaeztlk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/grktezzsr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gjjuuapyu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/glxmwtzoq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gknuuwrks.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gqitftkev.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gnmunojmx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/ggiooummo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gomcsvlcf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gcobaorhj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/giswububg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gpxnbrmuu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gkjsfitls.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gedllptqn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gwnuammbn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/grwcysxvl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gyyoduibz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqqjeldty.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gwbxualnt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gvaqwvkfc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gpptlktoe.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gzqfqiveu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gmdloilel.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwxmfqttu.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/geerzzhrb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gesdnydel.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gugfcujch.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gboficsah.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/glnyyrevj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gbkugmwnt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvwebepqj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/ghxzuexmq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/glijnfmtp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gqrxyqhat.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gxzhuzrps.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gdqheodkx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gxbggiuug.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnracmgmu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gpgigapia.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gejhhrxwi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvqnzoeku.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gytwctxks.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gobzceccq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxkaefwct.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcniforqs.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/godwmzfst.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gjvpzrrqy.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvjumdlhw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gjqemosnw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gtpmvsswv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gkvqmimiu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gvrljztku.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gpwdvnytl.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gcmrlvpii.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/grjxuygar.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gzjapkwdl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/ggfjqsbee.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gysyzelmq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gswketcer.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gzqelkeyf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gzolegmwe.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gvflzsfyp.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gyqnxcuxs.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/grpwofaxh.sHtML


<!-- 参考信息 -->