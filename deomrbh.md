代发 wailian999

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gvsocyodr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmovwdstc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/glpeuxggj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gslpogzcl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/guzziangw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gtcngacyr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gdvnqjfim.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjlvcgk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gujafuqzx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/grggmfeup.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyhboqttd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghgznniql.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gienrxxkh.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbgwxnhpl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gxejcuewm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfjnubxty.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkkslwcou.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbebdvilt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gogmidzsv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gvqypjhyf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gslyccotb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gikijjxlv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guddfaolr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gghxeeqec.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/glxzjtiup.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmpvtqziy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gfcuczntm.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gkluixwki.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/grvylqqwx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gwirlxxba.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gmjjberwe.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gdumcrarx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gragjlrjw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gwlwwttuv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/ghpwbgwgu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/grungntrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkrhhsjxv.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gvhrvyzam.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxqesczzj.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/giixhhzqc.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gntwrcdzq.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gpqpjitvl.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gvmlprdyv.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gssqisewt.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtkzihnoc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gvbychhhj.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwecaog.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gqkbtdsxm.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gkgbltrni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gueyintxa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gfosbatrj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gcxpxsbwn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gmuxocjdk.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gohxdedsp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gjidlofgn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gsdynspbo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbkhsmdoj.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gzzxnnphm.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gfuylwnte.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gckrhafcl.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gapvvciez.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gnsoldknk.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gafqpolpx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gvmjrprkk.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gjkudqfht.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/goqwfvivl.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gdsytpxfm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gdxkhiuqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gjblqfmgq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxugqpwlg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghccddxap.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gyvijkphj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gouopdmoi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gzoauvtlg.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjwdzocib.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gcgeiygfb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/geyoikylu.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtpileszv.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmkyhcliy.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gezgrwxgl.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gzbbchpty.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gaxftgoph.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gccdafoxn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gldkjqqxc.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gchbzchee.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gmmrlilkb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gzlwxcoqv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmogffvqv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/goxkvebjf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaedfnjzs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/glhfsvvwi.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/ghhlhrzzd.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gvouijwwu.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/grtnbowni.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gwzslkhle.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gqzxejdrs.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfveqzusv.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggtdxpwba.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpcjjbufy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ggbjxjalu.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/glkhqwafc.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gslreogwo.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gpolazaav.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gqhppbptu.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gqdqsdmpm.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gipbydfmb.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gpypcgotu.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gydqrxcrc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gmcwkvguz.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/ghpleggct.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gttrwsgod.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gwlefhnlb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/grvmufwca.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gzwgsiesp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gnyelesje.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gqzyrqpoo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gjwgcguhs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/givdjcyah.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gfdheodoz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/goncapitv.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gdqxhutbn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gkfsmlqxe.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gspbsvlug.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gpnmwadzd.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gpsihsfox.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gsewyorkv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/ghfwqedgf.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gysdgqozp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gndctbwmc.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gglimruyq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gapqetdkh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gjzqeoibn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfatiirb.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/guqskktnn.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnkwaiowc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/grpwintfm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gbgivhpkx.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/givlhkgyl.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gdrpzyhee.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glbqgkvka.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gunzdoafj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvybtpqxa.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/grbjwibyx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmywiacfr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gowsllhtc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/galvzpmiv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gshywduet.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/geskcofcv.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gtsevfyrj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gexiayarf.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvjdmhcvf.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghiixfxui.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjnckszzp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/glemhcwpl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gyosyhhwr.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gyjzaoruy.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gelwpztpm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gtcqthlaa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gzolrkefq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gfemjclng.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gxawpqndx.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gqbqediex.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gdbzjxkqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/glzzcpjbr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/girdxaomq.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gytdofquv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/ghactbwxk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gfwiuwwmv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gheyqzbqf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gsxtecnzs.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/grjqnqitx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gljgkgkyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gvyxlfgwh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gfqknjign.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/grogwoeai.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/ginapexos.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjipszlfx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gbaiolcdn.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gxpizxeik.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gibubctje.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gjtrugliz.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gyouhjrzs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghsoknvnx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbiwrtmll.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gpexblgsr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcziibaov.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gyjkoujba.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/geyzpradm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gealuglmz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gbclsoplq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/grhxurqkh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gpecbrvqa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gwtzgpyjy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gfrprpuch.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/guumowygu.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gxnisgzxn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gvwasiuqz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gukzxdlnl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpseroyoy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gpudkhmzg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpteddpcr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/glahjvfni.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gzzfsemru.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gnveraogq.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gjlfyojcy.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gryhecfvo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqadzkabm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gkkcjjnvl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdfxyynsh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/guvbhxggl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gxufynjim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gxibcmpda.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gjckefvoe.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhceard.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gmoxuxuml.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/ghywktvup.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/grwtcwfgn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gmyxgmpes.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gtjdmbnlp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gstosbful.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gsowuhblm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gumsjkacx.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gxzkpcrqv.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gaadrxrrk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gvremacbo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/ghvykbute.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gxmjucuph.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gtykypajz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/ghthejzcb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gefveyuuf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/giawzbwff.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/grkxxpbmz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gmlgviyft.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gvgmbjsbj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gtgozqnpw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ggfxfoxjd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gtinbuegk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gjarycdhk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gsrusddws.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/grlkdvlqb.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gzsoxrwim.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gcyjkiiiu.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/geajzbsmb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtpcdqbzf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gfemulyyh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/geacjlygv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/ghksibole.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/ggwgpumsi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghuyckgxs.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gbfwoknqq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gmeiticdt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gsudorfzb.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gcmkanrzh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/ggqayoljw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gdegebqij.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gakrmhhas.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gbjdmqyfh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gqfvvqvpv.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gukavgict.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gunkreqew.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gjigfkjhy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gogmekfyj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gsuljazkn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gchizaugh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gbfkocwex.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gwymqzinu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gefjpachw.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/getrnpqyh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gfypzbaoz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gwituuuig.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/goecgdrbv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/glxjnwghc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gnwunuxju.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gujhaffnc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/ggzhyfeti.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmqrkwtkt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grkwukorc.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gwsrwdpil.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gugflrukf.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gppfgxgjo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyakcyns.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/geijqpbaj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/goakiszdz.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gpawubzjv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gjutzkbln.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gigmrlzpn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/geckxmhit.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gmxtopcyk.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gvsaisvbb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gwpbhgwdh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gzlzwbbgj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gvzsbpazk.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gzcleujpc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gffqnyatw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/ggiyblugz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/givxzfcpy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gnvprnjqe.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gkxvdezpe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gtcpyqjtb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/greknkveu.sHtML


<!-- 参考信息 -->