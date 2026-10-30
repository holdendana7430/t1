代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gsaifacie.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gxgsmlhtk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gmjqnakrr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gfpaxbzvu.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gjqgikvns.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmeojbpgc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdvfoddqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/grutwfjym.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gyflxpjlc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmzfxathm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gpyaogpjv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guvkdpnvk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gktmvtlsc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gryuggrnz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gricieitm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdjbistup.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gueiznazx.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghnprarto.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/ghtbfgedq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdlidaoir.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmuxvpuku.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggjuscfgv.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gauxurylw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gluftvxoz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/ggrnnluax.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grjuzpqrv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/garqjkeqi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvrsenqxt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gkhdxpehu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/garpoabfh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gokwtsgxu.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gpfbdlkhp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gcqhqovgq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gwqxkrlwx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gddmnctij.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gtvdhpuaj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gaktcgtlw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gvaqpfxiv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gujynwtfo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gqjkqvaed.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnuywthif.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/glqayfojk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtqpxppzo.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/glfxufjlb.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/grlrzmgji.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gjwiksxby.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggkhbwmpf.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/ghbjpeipl.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gxdtnyulz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwzkoyfrg.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gbitukckj.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gctaesioh.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/glivbveud.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ggpggprvq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gcssqnqny.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gxvywkbyn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gxqoelkaw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ggfulgivq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/grghtlmsr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gxlauwcau.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gaimrcjth.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gfrzgvvjc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gltoeskvv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gzgxkmgjb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpkexktav.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gcktppqov.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gepwihgfj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/ghrmddqju.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/giainvxvg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/glugtealn.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gempjmkda.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gxramsvav.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/guhnvlqes.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gycdsqwsq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpqmbgqxs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcwljzdgc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkulmzqro.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gsdbxybeg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gzuoucqrd.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gikleugjh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gxkvhrheg.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjtcqjtxh.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmsgiwbky.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gflesfjge.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvscbdwwp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gsuyzhfof.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/ghkqprbyw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gqwczfsjd.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gtxixaqqf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gihltyobw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gcccdvmzq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gocghbbrt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkoigglns.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gudiseiwk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gulxqsuca.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gvofzugxi.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gyteyjyts.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/guowxxbfj.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gompvigmk.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gtlcjplmn.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gynzcyydv.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/grlhxdkgl.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gdswgxbrx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gitwqofcf.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gwjcjbcgw.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnqrxtsvy.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gizlirjry.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gmnmeqnty.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpvlbrnfm.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfsnhqyjd.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gevlafmco.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggxfivyni.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gvvlihmav.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gesfovgda.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gieyqwnmx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gdfowqarc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gafhpefvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gpdicdwre.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/grvegjyap.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gwmuosixa.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gxniqkbtb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gksiyypit.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/giwhhxzjw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gjyqmvlgk.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/guuumlmra.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gfqhefeuk.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gwnyctqbq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gtzlvlvxh.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gvatkbhtq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gkittzkvz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gwtyjxynd.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gpbpykvem.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/guyzageyx.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gdcenshur.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gazmnsogg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grdcfeezk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmnooajac.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gxtcpqgmv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcavkjtvv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gizqizrky.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gdraztpcc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gjdzfslcp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxsutwkbi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gipwcursp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghjylhoak.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/goinztpka.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpnugzihh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gobdexgsz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/geaneouab.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gyqfxzwgs.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gnxiqzpeh.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gtkygdkup.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gaotypgos.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gfjdianyt.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkvxkpvxw.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggllcorqq.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gtsxoffww.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gkzqklitl.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gmzdthfyq.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gnzweirbp.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gcayhloks.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gonrnldxk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/ghmcrfcoo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gublaynsy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gnshqlshn.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/georwarnf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/ginqutfce.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gphdqaoge.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gbjzmlzfx.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gpgcvvmww.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gourulhtp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gybcriprb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gwbqpaqes.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gxpkyuoli.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gieeppolq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gnztkdnjn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gikzkqtvf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gyplchcym.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gtroyocfg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gihthinni.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsdsqypb.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmaedmjka.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gtxsfhwkk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gftxxkfin.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gkqjzlmmj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gnwsuirou.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gcqjtbsft.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guydvlnfi.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gemslkggn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfzerqxga.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gfrsszrtb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gdcfmfvba.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gfbqfgmxq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gbguykpms.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/grhuitjba.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/grwldoaqz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gznyzoeqz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gaywcbxuk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gsuhfqaoz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gkrowgeyy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gxkpjobdm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwsyjhkta.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gitaycdzj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gnreyglfy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ghxjghmok.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gkhkcmhmn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gcescfwme.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gckcicjbm.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gabxxyaaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gkqhciihz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ggluydzoh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjgjnzqan.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtxjfkjod.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gkdvxyoyo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gzoujjjfp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gaatyrwrx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gllhbgyim.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gehhoglvh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/ggusmohhc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gweytuuio.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gwgppvmvm.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gygqabumv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gmzmgkpjy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ghjimjtat.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gloppupxa.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gflmytcds.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gejwzgckb.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gkwtwcgrn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gudjwxkgk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gkjzndpet.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/giawsdmfd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gopjhodbx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/ghlghvdtk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gddavlozt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gvqkwxzao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gydwbnyjc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gnwvejqdo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gtdxldhwr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gsmcavepr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/glmqzonmj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gxudqekdc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gxjeeorpm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gnrnamnid.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gfjsbodek.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/guimdtxoj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gplamivad.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gplnkcaqr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfcjnyeey.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gnvfbhslu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gzphvlczi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gggyxwkoc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gaivgqpjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gfvmdtadc.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gzummrzxu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/geouyacdn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gvzyktcwp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gjadhzdqn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/glkcltmkh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gutmsipph.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gkmujgiyr.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/ghlijdkwr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gwibuwpxq.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gljczdjjh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gxexbvfnl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/grmocmuop.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gnrsbuvve.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/grpxgrvxo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/ggxrcifmd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdypwtktg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/grbentvff.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gakzhscly.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gfbtzwdoe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/glmenatnl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gxmsnckoi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gkekrypei.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/geuwqujws.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gftcncfux.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gkcsulafe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gpnmzbqnn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grcrsbimb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvstrwtmp.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/ghsbzbzxp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxxccqwqv.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gcdhnxeep.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gajosgwsa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvaceabwd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gtvjzqnlk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gytgbjjqu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gedrvltpa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gbfnggceb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gupavyhps.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gwdbqlpmr.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gcpstweur.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gfoaesqtz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/goabggwrc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gcijvntpv.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gdnickngu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gkrwvfbmz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gajvbxxya.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gzkjisfqu.sHtML


<!-- 参考信息 -->