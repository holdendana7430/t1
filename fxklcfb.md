代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gkvsjiwdk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gxgqbpfej.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gzdzytaae.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gdblhpzti.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gfnzspvgb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpjgamhkp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gxkxxpfmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gffshmsnr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gtvistfdv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gwojcxyja.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghvdonkkl.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ggyekwlmb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcorwxpld.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gygwgrytq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gvtcxlfpf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gmrpczewp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gplohrzjw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gfuxbipaz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/grpieozyd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/ghzqggurw.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gudhiogay.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gjnwwajak.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwjcgxlya.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfgkomluj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzzcvyjlb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gosxbcwne.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gjpmdjvtk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmzncvulc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/griuontds.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gjtqxdobs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfoluvlrb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/giuyrjuty.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggchadssw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyfanexao.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gypuzmiom.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsbpouyxr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfnfzhbnw.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjsywffaw.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gqeyzndow.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/guyllkmrp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/guqxcghfq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gypcanane.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gllawwahz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/giyjkvnjl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/grfgdsphu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gsilofyjp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gfjasikdw.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gtdmxfmob.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gmftnvald.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/guqcdvzuq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxshsss.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/grcxicbjq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gskbyzjmd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkxxymwfl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/goxohvegm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gkaijzzjx.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gyxhcmqbi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtigkbeww.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/guyqhlppm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gspyqhhtu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnfhknlju.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdybozbeh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gzxdddzlb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqwynmmxt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/goicppenz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gpeqnmocb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzuxogmey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxhtcaqpk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gksutuhde.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpsrecfwl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gazlyqcnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goswqsoll.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzlvhozzs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzhtomdek.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gyvvzxllg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/guyhvndvm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsfbjyncq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gyhltvbuq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gyibsgkkc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gyrnlncob.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gbsdkkjnl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gomxgppjp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gqsgnqnmo.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gargeqnxb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gmacqqlsh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gdzxvfbqq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/ggptgpejr.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/glzgpsbvy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gejuokyek.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/giggintxn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gfhvcqbjj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gkxoxhrsd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gysffrhvo.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/garnyzohu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghrmxpsjq.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/ginrgbcfb.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gpmhcaued.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwbgdahvg.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/guvqrkjbs.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/ggikcdbgy.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gbomzjoat.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gdcvhsfkz.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gjzwxlkby.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzmtijley.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/goutzjbuf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gbmbwgoxk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/ghkagmmwu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/ghwarvsfx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gzcfthetf.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gnocpzzmz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gjegxvrks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/guliecrsi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcmiaeesm.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/ghzlnfbff.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gcmxuxvdm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/glhxytlnl.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gzaeeodfp.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gyfeutddr.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gwjlboxaa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gphdnmgpu.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gmcukouvb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gmolupjja.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gofjsdtcv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gquohmpyy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gtwlygcri.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gizeqrfsd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjfwlspr.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcsxetaer.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glpuxevsa.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gecfzyaaz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ggkukuksk.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gqekmrfux.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gtexkyqvn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxkkfvaac.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvoogknoq.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdykxzdky.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwetbgjzr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/goihvfebc.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gagudfwmd.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gyeipobvi.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ghdefsqdp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gvgtdyvhl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpcrxvgzc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/govcqzhah.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmsvwghfl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwdvfotqd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gtfkysptu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqaghbv.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gqbsilwow.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gfliyzaty.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gfxguaznu.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gycuclasr.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gvjlnterp.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gobyyolxy.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/glsdanbum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gunasegho.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gvaxeisvn.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gokdvlbxq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpatzvqlb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gdwrwdftg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfcivikmb.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gmgbnjyux.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gffnimgsi.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gngqahvrs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gkianwpwe.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gmvjhotxg.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/glwxajldh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ggdddjmtz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gqybhgpgf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/giszouywl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gviyhxwqt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gwmuoxawf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gztmtanij.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gycjfiqdm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gvhwzfcrp.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gwqvyozea.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gsrxuysss.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/grrkzehdm.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gyxvfjcwv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gnzctoixw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmixuvxio.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gxnhsgwvo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gxdtmkluf.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqikfewor.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gpdnuxbza.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/guxsqnxmm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gsglxymkj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gapffrzat.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gtctaepyb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glikodhng.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwummtka.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtasfspeu.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gxwrgwnzr.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/guunzpatr.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gvsebeznt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gzwhasznq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/glkrrmpfy.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gyhmjwaof.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geaqqeore.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gswcnnnmn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdbrnjfpv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/goaiptyvw.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gujtrxccr.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gzfnzoraj.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gnnxgxkwg.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gampfukzh.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gboygmfwg.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/govqrdgoc.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpkrmiybl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gydaaeguk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gtblnpciz.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/ghyzvabgf.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gsampwkoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gwipdiqsm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gjdydlddj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/goyshdsoo.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gnwqhkenh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gmjgudlqx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gbcyhtrrf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gsmaexmod.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gahfsqvlt.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gmjifwedp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gphymozdk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gicrdqbtc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gwzrybumh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnhapdxxa.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/guqinxdvx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gkkbfdicx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gottialnj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gqwpjorpm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gxwnifhuu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gjqsfbbet.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gvqpprgld.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gcmujwvem.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gpxvizlgq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gdvzwocic.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gmmuyeyzo.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/guzfdygqe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gqobdynmy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geclzezzq.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/guwuvmkjq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbetkuyhx.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gekvmvklo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gdhcodahk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfelunop.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gwqqfcmlb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/garptzwep.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gjsflwipd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gnsbddbqg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gcvyqerea.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gdgnslbod.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gkbadsmcf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/grtqvxhiy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/giwcdrajy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gajynzakw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gizgakqpa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gifwrparv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gfxcojryg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gdvyrcxyc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghzsxtwro.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gifjwoyhj.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gmqemgvzu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gziaupfbs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxkbfbyzh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/grnnhilln.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gelpsyhqy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gzfbcewac.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gknogjfnr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gnaasjtkk.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gkhlrdsrp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gpdfdcakl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/grkmlyrst.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gyxdbszno.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gfgflysug.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/grpevjjns.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gwmiufska.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/ghvbngxfx.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gjfryzmmy.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/giedbldit.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gwnzpkmgf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gqvaebpks.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gnvgywxsp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnmpcnzdi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gwucclflh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuajduxl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gdecbszfc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gohsrhxlo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gacivjeon.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gsezyywez.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gtflbwivq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gqmqwkzem.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gperrvaby.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gwnbulrow.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gtjreaybh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gmxnpdkyk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gybkfndqn.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/grivlyhaq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gxrpazkxh.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gjpqsnyqz.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ghwlkreyc.sHtML


<!-- 参考信息 -->