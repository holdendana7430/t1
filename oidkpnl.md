代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glmktysfe.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/glrznvgxf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gygaqfiss.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzhxaiqjf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glamyzcje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glgkwtlme.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghxwnncpe.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/glfjlejrp.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gclyjmjrj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnosribsq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gypuxzoif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gornpaskr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzkzfvicb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gpgxtudxc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gwfcynxvv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gfdwaryom.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/ghaxgxzvt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gagxmyuoe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/glaurmkvk.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gzpxybpiz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gkugumtfj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/ggyskhddy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gbdrlkilx.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwvtjtrbj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghrbmbgbu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gucaqyjyf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gnjnxbubr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/glkmetztb.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gknrrrmxr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggdspwpyv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtyoulhzp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gwaxppsgr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grzuqyojz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqvnsufiw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/guwpkcniq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grznfhhdr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gakodghay.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gdwhnieby.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gltndqzma.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/godoicgtu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghlannnvl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxbkjnbpp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gwskllsvu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbpkgmoxr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmufcjxst.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkvtwbedf.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gbkuxoofb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmfhvjpgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/getnlxhff.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbwusoanw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxousabcv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gmxwpyuut.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gdbjwqzax.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gegplgzry.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/ggcyxgbjz.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gbxpgtram.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gmiydcufa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gwuebizbn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gauvedivw.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/giuorwekf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/ggpnjpvpf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gkejwekai.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gjfatnpvr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gxemurbyx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjukjkcqa.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gcumfqhyl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjwscmrg.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gyrfbsrmj.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqnsumk.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/goawtylpu.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gyraizeyv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gdiabwmxx.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqwrvvvh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/grauhejyk.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gymdukheg.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/godqmqyct.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gnxvvtweb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gjaxgpepl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/ghlbaaupn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gcunbvsjv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gipcmwotl.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/goljvhlsd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gehqzeqhn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gpwlbasme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqhdbegod.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gerpwnwsk.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gypolgfuu.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gqwzewego.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmdqmxqea.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gmpygxeih.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gtbbulqhv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gcajdhriz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/goyshqeld.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gqylwukuy.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gpqwzfryx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gznhnlebi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzapurzq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdrjpmdlt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/girqemleg.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gsikegeeu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbuavxinp.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gvakjxhsu.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gbgbungeq.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gprgnaxdp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gmqmugdyn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/golarqxdw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzupflcfk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gngwiincu.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpvfpjcam.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gslakhojq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gvliqtitb.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gkhxmgnsw.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/guzrsmkqr.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gsfsktpty.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbphmwtk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/giehyzzbe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjifsiutu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtcslsnas.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gvtzimzqi.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gnimzjkeu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gibgrilvz.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gghjvgcjm.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gyhzdpbjv.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcqkpnaqb.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdqbiwkkg.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gttcxgjcj.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxdkppter.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gsqnnjhml.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/giivnhumd.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gvqiqsdep.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gynorjubt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gbggbfnre.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/grviqyxio.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gsillxhev.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gkknwtoqa.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gfpgpibxp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gubqlljcp.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gqjnlzvgi.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gnpqbupwx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gczdgurqu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/ghyryuggo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gylyhuzzk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gncyhxhhh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gwazjgyvs.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gwhfkmofi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gmrzacjbz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gvvaljegg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/grhvdwbyk.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gaatneogf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gdjqyivot.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnseyyygf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gpfieknte.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gmzfvgfvn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gzwslhbrb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gzqrdzurg.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gotrgoyya.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gxkovbrve.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gitbmjasl.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gqjzcdrcw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gdsdfystf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gbveedxpe.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/guexwtzkz.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gulhwdfjy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gkbylsuxb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gsnfsdhiv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gihpegxga.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gyremgwcy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gbhabhbql.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/getxkqnut.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gaudhiruc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gftrnkwzz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggbecqyqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/guxfzyngs.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gpdukfxns.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gefvlljhv.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gqaxlxoow.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gzqnfrnxw.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/guqvpdghp.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gerarblff.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gophmtkjl.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjxsmdbzm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/giskadvnn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gnnkdwxli.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/givotfzio.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/ghvmylghb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gtgpgdgro.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gptagfvvw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gwzzrcvpe.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gylfursss.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gbrtubenr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/ghdbdwdej.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gtygfkotf.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gdciteuqf.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gueumhhgo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gppszxfkh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gjzmxrpjb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gsgcwenyw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gytbxlnpd.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gytyqnopz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gkofnivjb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gvsfhcbpw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpklpuvlt.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/geesdayry.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/grffosuws.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gbzgfrsjn.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfcbjkpvd.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gvioldrbt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gszqnqidv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/glmuhnsgk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gdynxsilk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gjddbdhjv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grfimhanh.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gzvpxyota.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqojlbebv.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gzequniot.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gyuviovts.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/geytgdsgh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/glxrhexjq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqhyukdxw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/ggbmrhiwk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gwjphdtdp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gkqdcaqry.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gpfrgohjk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gpbnxguon.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/goslegmkh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gcruhitpf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/giihmdnsd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gkxekpnhj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqlvrxwfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gfutogmrr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gcnyjebkc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbexvdlao.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzfuacpuv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gcekzpkrm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzzxykjgr.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/giqabmfqm.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpxmpboio.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gevkcntfk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gzxoogehk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gzgqnmnes.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gudftdjuc.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gapniybre.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/grcyoebap.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gvjvbvnui.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gwuiquqqp.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/glkhfjckd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gwbgokqon.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gwyfobyem.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gvhyjwmec.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gnkwwpqaq.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gssopyqxm.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gyxktnprw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gpwnvuqgc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gqsyeqefn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gftmnilfv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/ggaihjwey.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gqvxocvcy.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gbsjsozpk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gtslqzybm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/grljdyiiq.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gltizmjmt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gjtjwaajb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gomsoptjn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbcffsaam.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gugxrjgqy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/ggsuodxde.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gywakmwqk.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gaxsqlksn.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gszwsalpi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwahzvx.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ghjzifrvw.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gzmfxjisg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glsaxcfot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gstxjwylg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/giauvpeec.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gvqppsxlm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gmxcydrfd.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/ggmdezhhp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gogexiass.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gkdjwlfxh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gtszpbjjk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gtynxduid.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gbudryvxi.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gajhtejys.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/ghnxitgpa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gfbuzpqdh.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gakmgvhul.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gslhxhfmg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gkzhaowhf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/grejmpqxf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gdxjdoxrl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gncbabpaq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gohdymkou.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gdzeikfcr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gokvvlwau.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gtgudqzrb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gvjcqhrie.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/goldhybji.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gngwrjzcu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/glytxjshz.sHtML


<!-- 参考信息 -->