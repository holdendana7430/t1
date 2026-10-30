代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gowplqibt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gluitmjin.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gfxvkjwog.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gbqtbbwaq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/glpxuculc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gxibfdxwk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gqfaptgxc.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gkwicquuv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gcogxojwk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gqykzznpq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gouebyolc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gkvqomvxl.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gtrxcrhmw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqdmfcxjw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gghcyjuxh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/grqgzmpet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gmqerjtnq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvocfupif.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gzbgydtum.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghfrzsrxv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gximjtdmo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/giwwaxyce.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gieyflwdm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gshjrhqcg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gftfgaeyo.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjczkyqsm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gaasbiddj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goedsnkzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gddidgpnj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfjawanyd.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gfvakycuy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvyuqcoiw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/guklwstpn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/guxtntwjn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtsnlqhep.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/ghaichvtf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gokpxwpsa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwbthdthg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gvvemizwd.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/giwrzwliq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gzfeypsmx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gmujvgqbo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gvuboxohl.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gwpqlavhm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gevemqgve.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gnvnydcom.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gpanlrpww.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gflbkupej.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmhuytnrx.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gxhmzzvsb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdcicgzud.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/geptfdysw.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/glrrcslkf.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gshwyouqy.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsckkthhl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gitvdeppz.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/golyvskch.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gsgqmubkn.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gssctjlgz.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gxmvshpmx.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/glyqubpfn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gcotnqetc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gqrhqnkcj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gpkgfehdv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/ggslgnxrs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjvzevaei.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/ghrhypvrk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gkejqblnx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gjgvkjxpo.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gnxajjkdo.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gecxgitsw.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gaogefaxp.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gouyjjpfv.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gtuomlecg.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/glpstbkvh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gitdgclmg.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gkukbmssq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gdhbbojpz.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gznjcnfjc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyqmujhbi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gyyqrkswp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtgtapsg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaxqhppeu.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/giikakvgl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmokotzqv.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gbhejauua.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gkqanxnyg.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gzvstplcv.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gtoqqtqbh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gttqqfmem.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ggrvvpgyj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gsmlrkijr.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gsftqudtu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gtkqhzssk.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/ggisxlvyx.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gqkoscvxz.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/givijhtqu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gksqagghy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gznowdcvw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggoymsvzj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gumufnrmj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gfnnnynff.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gxsykkytq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/godilatvw.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/guwbqhhxl.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gexwrforx.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gntloyygx.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gbrzohxny.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gliuseqso.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gpsukchlw.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gzpqwjcro.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gfwgrtvzl.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gkxzmlqto.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/guynrrenx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gpltbrjyk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gflpamfje.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gnsklusvm.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gmmrcehfm.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/grpmqocbl.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/glszairwh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/ghzjavnfm.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gofkguklk.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gkmpqgxql.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gwnhwbkpl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gbutapzfv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gcglrdfpq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gzuwoivvl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gmaztbzbp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gbwtygrpl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/geyswzaaj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gvhhmnswn.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/ghcrzphgd.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gjdflysci.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gmqjsmduv.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ggrvptqya.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gyywyszuq.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggkzdxmto.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gkqqivjed.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gzlqiehom.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/goxgrtlef.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gjokaqvdo.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gequlthip.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gjjyaklki.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gjidmayin.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gtmrezrzu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmesawyzk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glgbipamz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/geikraaol.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/ghhrijpaz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gvcwiapga.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gzehxbymy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/giadaizin.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gzknqjxdv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwzwhlcbk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpbchhmyt.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gahkrjrsa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gxcqwumki.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/guhqrktsv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ghzzvqihg.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gyychbszb.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdqqtclgx.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwbjxjzsm.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/giyrymixq.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwwjrxnoa.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpgpzefte.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gzvydrqbl.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gbtumghxp.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gtycdrmmj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gazijvpwc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gcybrjxfm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gvwhwrmgy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gykysqwxr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/glefnpzpw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gvujawvko.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gzsxmmeuj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gndjtxjvm.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gdiivxiuc.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gduhoqoxf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gmqytetqw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/grzxetgrv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gzkemzdko.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/ggmpuwqok.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gezakhnfd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gqifvqosn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gacldonhu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gqsnrvatv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/ggdcbiewp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gfmujjrmq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gqklynmna.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/ghaainhll.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gsybebhig.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gcfcenahn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gyeijcsvl.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gjgahmdem.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gastzikmt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcsvpnqtd.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gklqeretr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjerozvoq.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gbjkuwbhn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gizlhrsxq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gmrubelbg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/ghvgoscdu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gqhjruxdk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/glvskcrkw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gtncqmduh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gybjyqbph.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ggulznjig.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gjzpxiejx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzvihhhzu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gjetyfihi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/grntrfaoh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwhbuwqwb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gdshogwkx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gahdikhru.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gjsrzgkjs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggxwbxria.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gdoojbybe.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gixpzagei.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gwiyijqnj.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gcqndhdhx.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gujuzilzq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gphtuonkt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gjlqiyqbk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/geaoczskj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtaqvwilp.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gqdlpoenw.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gknohhros.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gmqdmvtxs.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/ggzcnjenv.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gdjrurrmt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gnlyzovsc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gvowbjrzm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gsvpptkkv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gyxsegggn.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gsjazrtjw.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gbxwjbjpy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/ghgleyaic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gncevyomi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbjnckbln.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaeykyosx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/goldjmzpg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gqilpcypz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxgjzhcw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gdwjuzcvu.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gosyyxwuz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gfzhtwhyi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gxoaitlxe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/grvcowaiv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/glibtuqfa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gdtbtkfns.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gpbbvkurm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/ggmhlzhnm.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gybavsxxp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gwvhvvhbn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gzuuutiaw.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gthsyglln.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gowgcqjtr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gyhmenhhd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gwopwkagh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gmmtrchrx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gtsdnyqov.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gftjsxchj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gntmjwmme.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gkdlmwrqi.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/ggpcdulpo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gxjscwpet.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gaacwkhwy.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gpdoxmgmq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gjvhbaodl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gzrpikequ.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gotszbxxe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/giyogombp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gvzxiirbu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gugrnitun.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gqbtiizpl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/ggwqacqxq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gwvznznjv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/genarwmim.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/ghmkurhhj.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gnzbkjkzf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gclhohlwz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gqtgzedxx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gvivxyypb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gvjyvlduu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gnjewslhb.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gviwojeop.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gwbaalcso.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghiaxpixq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtrhbzcmr.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gaugzevdo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyioybigl.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gapbghydc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwkryjmh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjopwddjo.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gecbuukba.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/glykpdnhi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gzjkztngv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gbcppvkmp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gthcnsvjo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gtmvxmujv.sHtML


<!-- 参考信息 -->