代发 wailian999

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gyyraboab.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzxqmdyek.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gesedkcwy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gaaaevuad.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glgnaomvo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gekecoeaq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/ggjpqertk.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpdiwkckk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gayuvimqa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gpmnwcxql.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmnndlnxj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtzzemqur.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjnyoxrxc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbyfkepzq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gzpieyflb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpdgzjtua.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmvfsmwhm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/giqgnjrqw.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gstaaigsv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gklppibwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwavpcqec.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfnjzcypd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcuazwcjg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gtfdeqqlv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gbexobwev.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtcnghinu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gjquwnwmr.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gmuxtzcei.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gteryvhnm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gfhkzncgz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/ggcazbvan.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gvbhrgdaj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gtcniikkr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/geigbjbrn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/ghykzkjsi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gzloihesr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfmwoucuo.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmvxkov.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/galjgxtoa.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gnbvztoiy.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gadudvpqj.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyhnnebzo.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvqxahowf.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gowqnrmwq.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gordgybdi.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gfbfhtejy.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gixwlxlev.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqkwckmsu.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gvjsqtqqp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/geullyhgv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/grdnztpob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbgzvdwtb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gvhmdbzkx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gsktkevie.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gqxjugfup.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/godzvswxc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gflaxatlo.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gftkrnxpr.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gqrhnguhr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gihcvnrzx.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqrlknvgl.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/girejlvao.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gnvvqluqv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/grlqidalh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gcvaoccvl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gsvwyqbdc.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gvkdehmks.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gxknrbrbg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gywcxhjfo.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxgegqdnr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxzxasgkf.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gnsbtxsak.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcqzggufk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gyjwaykld.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gtinsljmt.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gfhnhgwar.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/giynqpgdm.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/geqlboyxk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gufpbczuu.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqzcexpnz.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gywcewcda.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gcoqhedtt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/galrklers.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxfbjtjiw.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gfmipquor.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gebemojok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjisxzxth.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvdmjiipi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gliycxrfs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggxlrlbhv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gtimohusq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gwxnmbtsx.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gczwfyusd.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gqvkyqwan.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gbxqmuqtn.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gwnrxeffl.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghacjjacj.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcuttdyxx.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/ghgcpdljc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gidfjhyam.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gvdgulbqz.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gplcipgto.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/giqsnjdhn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gshmxjjoa.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gtjhihuad.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gwfaswmdh.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gnoexbiqe.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/glaxsxmjq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/giicpkpku.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gaxoyklko.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gvocrwwtr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gfrarnqsr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/guogbbket.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gqcvwcmpt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/glazpgrrm.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/ghpmpbtrl.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/grflngqyd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gajlzbyuz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gabkewbcm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwueldbba.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gsxwhbzoe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gdzyesnco.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ghwhvyqaf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gwhqfcszj.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/getngrsxo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gltuyzezs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gxvdjxjey.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnsoplrsp.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gictddcwm.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gbrroxmlj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/grkwjiyhz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnnvllcgd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsnwvnkq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gkgklmfyn.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/ghqtxujze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcssypslx.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gbgtidiez.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gdapzybba.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gujeyjvff.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gybosqatd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gxhwyjiyl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ghgqhmrxp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvidrejgk.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/geraipwca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/garkjhgki.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gvohrptjb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gzdwyckht.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gygawrrbf.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gcexwsmqa.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gibsqnhdw.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gezqffpep.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gsnysswcp.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwtimzgtu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gksnrpcmc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gevknvuzl.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gnrxhiyxj.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gbtuwlxtu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gijvwodyw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gyioheods.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/grpjveyms.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gfbkrvysb.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gxadpvgpc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gkfimggcg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gzuznpust.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gtxkpwcfw.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gztxkojpq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gtgjeojvo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gowlaixlz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gqfkzqzsp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gplaqhlvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/geaemutvm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gpgtfwtys.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gtfufjvzm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gotduimah.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gdcxkjzys.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gagnoqlwg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gmygrhcgj.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gmmjguyqd.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ghcpmcbbd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/guubozfgw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/glzccltpf.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gspygdjzj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gcdlcgqha.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gijgtbroa.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gorttifmm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtngasvrt.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gusfgmwrg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gebzjqivc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/glonpjqpm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gvsajiran.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grmvbmfli.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gbhiulkoo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/giyemlpjj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/ggrvqoezu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gfvnatjcx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gdqoefved.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gqfsxtuoo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/groytynux.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gziskrcjv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjgpjxvtu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnxifskrm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gvawotynh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/grujpfhtl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzzlqdeyp.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gquvpinnp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gpytufwku.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gapptfnhf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmhoaiknc.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/geefucfqn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwqfybdyz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gwthofntv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gabvyoduo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqhppqxko.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gnhzhzqvd.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gakmegsil.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gdhkpimrk.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gnynrbigm.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gqlstfgwq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gpffyewwo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gdlqqdrdu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gvhcwoevy.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfeehtwwi.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gjiuhminq.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gkjczyxjx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/grnoxpmha.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gmjmfrcjo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gwptgjeem.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gnnnwcjgg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gsplcvkhy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/ginvhnuxi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gfeoogzuk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gzntxkebh.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gkjeliced.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gdpkqayua.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gzdspzvdo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gyefijsyf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gjljvksrj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gkrawribu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfaymsxsj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gkmvbjddq.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gpgtjpyco.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gsizjnrvo.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gozjcjsyx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ggspmuebs.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gsapvctal.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gztawemiv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/ghbqdukvr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gcvknwkwe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gymxxkrrz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gzbizxpkv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gbkwsaxgg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gbzjhfqsu.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gtworhrxq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/ggsflgjlq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gvgeeazof.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gbzvgqrjl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gbsrzdrdr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gbzbktkhj.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gukpbfccx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gifohkzqe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gjpvignfa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gsbrbbdgh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gtpegaely.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gxwlbnfqi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/glralkpwe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gzmxcuqoa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gkdbaohff.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gcirbfahm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gcdawcyyt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gtgfvtxii.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gquyemeho.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gjhlmgldi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gavwkznti.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gwibsffrm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/griidyfuc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqmnmpnft.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpvgkkqcj.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gbvemdkmq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxlypjpml.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gysvklseh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gawawqihd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ghjhgfvcw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggrtavyxg.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/ghyxotdnj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gbkpivnss.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/guasvoahu.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gawefeycw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gyoozvnvw.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gtcxaofxe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gbmvlqlwm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gcpvrjyqb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gxjvxqotg.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gzprxyzxk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gnuckvhug.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/ggkfgrftl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvzziezl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gemfztgoh.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/geqidvibi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gmqhgadtm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gfilbsrir.sHtML


<!-- 参考信息 -->