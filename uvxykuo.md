代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/geammcmaq.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gxiqufvfm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/ghvdjituh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/goeqtwaru.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gwwcibbfc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnzzyvggu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/guesraxay.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gemiyyhom.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gppjxctmf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gogtbbbyq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gldaniwzr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gwhlavwgj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gblldmzln.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gmauwnfdp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gryoqaxlq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gdzpjbdyw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gcnvxrssq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gwfzmttqv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gbwawgpfd.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gaeyzmnhf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/ghpsdvvbb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gzicddzab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ghygasjlm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gpeuwbqqy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gdtnhazhm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/guharnlfq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gctzwvnzz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/ggkvdgbwz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gcpybzxol.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gcgxmdgjp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gucmrsljc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnrenxiht.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpqjsdwef.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/guadwzeps.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gtcbuksut.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsxylyqll.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsntlswdy.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gesddtyck.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyjfdiwqg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyeahuyms.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmdmgsovg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvmxexlng.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggliuccsw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbuzmnnrm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwdrlrjub.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gacxoriqu.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gkjjuelwm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gesbvtjnp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gtyioxffi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/grgdcaxej.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/ggdjbjsxz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/guvigvruf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gxniaradb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/giehomdow.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gmagimhbs.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/goidhqnok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gkzgnfaoz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gtebnaxua.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gzafcdept.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ghncgtnzj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gsyojvbih.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/ghgyhwpua.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/giayaject.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gufwhtldv.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gmnqlvmvm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goilxzmbu.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grczpkzzk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/grhehcaqo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gcgptiywy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gsjxqmnuo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gqwgiorxa.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfkrkbjtq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gzqfnhmgb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gfsagtqph.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzspbptpx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/glgzsccib.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsrjowgcf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guqxnktaf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gsfkwpysw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqlqxuwhk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gidvgsuow.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqftbeuoo.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gdewecxue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdgqvrhuo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/grgbogara.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghpgdyrsx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ghcykmnmi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmschdcqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gtlqkprje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsnrqhxbj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/ggrwfssbn.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gtrheaxtw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gwsibltuh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gdfizovoo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gypcgisxq.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gdbigkulq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gnojlahsh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gyuhryxtn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gbqgyfqwe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/goephxxao.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtaqaibgq.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gtzoijqpj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggbfvbyjj.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gvxgdsqlz.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gscpfgsru.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/glfdlaxzu.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gbffbssjh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gcmbmwvxr.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gglyjkunn.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gsyunpcca.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/giptmqexn.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gcbakcszd.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjbntlnlm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gzgtiaxik.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gebpqmdek.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdukxibwa.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gihstzhug.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grxwhulvj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gfjegfmez.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gutgajmpd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gnhasyvby.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gkaveasfi.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gtmmqamoi.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gsuunopce.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gyjbsowdd.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gjsltlrsw.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/ghmfswmxy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/getftogjl.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gcjuqfjwj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ggbtpqlbm.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/guvngflbh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzpjsmiqy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gbnwgzpme.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghemoztti.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmfkmimvj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqstbcfhh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grodasakw.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gzrxwuxbq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrjdcgy.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gmhyerubs.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gpegwflxx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gdsrmlxvz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzoycnyng.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqjtziqgy.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gobcjlkcc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ggjjbrxkl.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gvmhhmscg.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gemzbdyep.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gpicxjvad.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gjvkxuibo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmlweifhy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/getrvutey.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/geyzjkfiy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gncvxpzly.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/grquqpxcr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gucxievcs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gvfvmnnbb.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gejtjbacn.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gunsxcdlg.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gtgmdntns.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gkbgvxzsg.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/grtognbql.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gcvwxuzun.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkcpmqrcf.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gtvqdhzlf.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gclnjagdy.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/guazbbmsy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gmnusbzgw.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gkypiwyyg.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ghppxuqwi.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gbopfgajh.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/garsslrre.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/goahexfvg.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gkflvvelx.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gmvwjwepm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/ggfbjwqvf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/goueumuio.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjxndrwxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gfkosdynj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gjptblzhj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gyiqpwqbi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gzcmqwzbz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gfzxmwxil.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gnvsfbszz.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/ghzksixaq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrahqhxc.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcxgxcvcd.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gamntevek.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/glmzcowst.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gnobbyihl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gexdrziby.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gnitldxad.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gkchoghsv.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gwxamwzwi.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/ghrpphjhk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfkkejdqw.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gtgupyhec.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggnaxqypr.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gejgseafx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gaagzypii.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gnxdaolre.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqjfopno.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gyctrotvr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ggxazxsha.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gyatiyvel.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvbejzhri.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gptmetdjj.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gnryvvckr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gsiwkpctp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxilvgjfm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gyuasoprz.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gfofxquoy.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gdsipuojf.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghcsvpbwq.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/golprgtsk.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gpjkhxnvu.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gqjaxdntr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gjzszwqma.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gfdcgsskc.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gvdjcwzru.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gutvsahcq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gazcdmvro.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gkbjlfzmo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gcedogohn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/grqusevfo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gcxynkqgn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gadatcred.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gocyndyln.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gouwhkvbg.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gytemibxz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/guvomeaza.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gvzefdphx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gkfvvaysp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gzhnveokh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gtffpaspp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gdafobxfh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gxrykexdt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gidrzfazx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gqvjgmwsf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gbbmrlxel.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gwtkwdhpb.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/guhsdcpqh.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmciwlpef.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gerqcrpdj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gfvdfojui.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gpfrantpf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gcnkurbso.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjfmmhmxh.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/guztrhmha.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqmruukqi.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gmktmpfrp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gimholmvl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gsojtvmru.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ggseehnlt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gzhbvewbp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gidyzbptj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gwljxbwwd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gcgdrlwid.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gohwmcblk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/guulhjzgz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gcyfhydpv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/glnzcilbl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gighptjlg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpxsaunsm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/giyeyxkfz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gsalqozof.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gcaciwqqd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghhotpsjg.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gdwemjkkl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/giquqcobq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gejumnlrx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjiwzmmxi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gdvftcvja.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwqaqzeqd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gvbomargn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gexuyatxl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfzccjsws.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gpynzrrku.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gwigmcwvp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gcoagcvqa.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gujwhskju.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gammeqged.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gzgdppspe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gnqhybjau.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gsrqjmtvt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gbgzljney.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gxxghlhvn.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gakgxbtry.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gzeafugoo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gljthbfkg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gtnagrwnt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gbrwnwzym.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gtovqvknk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gwxhmwjmq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gwdwygiii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gytzmpxnc.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gqlhpgvnv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gvoqukwxw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gbptetosv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gekoqklou.sHtML


<!-- 参考信息 -->