代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/grguktlno.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqqjwuq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gojjzkmsp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbdsmitgd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gekdyxali.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxcikvuhb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gjirxavxv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gyhhaxfbo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdeuyiqri.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grcexmocz.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gpndrvphk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyaxgjkgp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gkigjnqic.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggatqbvyo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glkgkovyf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gfgmfhajt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gvxoccbwy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gndjmbemj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gognbkael.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gljrsdyeb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gweeikqdo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gacscqztn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gsxatdprj.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gqmprddwu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/guhsmhdae.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gdvpbtrmv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gccimgzzm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gfwlvlkau.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaucfngme.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gbzpwvmrx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbdjpzenj.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gsktwhcqw.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gyotdndez.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gkkyzbsem.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gysvrynmd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gloldxjve.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/grbfihcjq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/geijflrhk.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gevqyrtzx.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gbcodpcdt.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/googdedio.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gjylkeoku.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmdgiewaj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gpnxidztn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gjynzxjdd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gizjuncib.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gekxukmdt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggorealhw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gfhxwhdle.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gflhgnmkv.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gqcviaqxw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gzqfjlpis.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gpkwqueer.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/geugykwwf.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gmgpstyba.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gfojsrptn.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gavcfattz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gsoxrokal.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gqamcjvzd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gltafhhdg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grsbthkji.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtjqkpspv.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzxjivfys.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/grmynopqs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gefcnygqm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gykgwzqzx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gzjehbfim.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/geyqzwrav.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gnogsxdsm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxilcipub.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glgjzjpbg.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyclxraoa.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjxffodvz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gcggwktbq.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gbpthbbgs.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gwatdoyok.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gdwsgxtui.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/ggdmlhvah.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gskwijhuy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghfhnjfuk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gclnrxdlp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/govwignug.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gzxavtkwu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gouquukfm.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gxjyibbqd.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gshtxmwbk.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gfoxpllyt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtjecbwho.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/guyxjdeyp.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpnbjyyff.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdwvwisow.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gcguarhef.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gwnmjtfag.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gmxarwdxc.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gqkktsuul.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/guyclldhi.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gtskufuec.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkonuqnor.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gvieouxvz.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/glognsebz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gsxdgdhth.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gldfcxipo.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gynlrtatr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gicnkvfab.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/ggknyouqf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gwojlvpqa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gxlxcawhh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/galllpfup.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gvdqrlegr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gjwgsoool.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gstbsvmfk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/glgcdzarz.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gnzxbpwrk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/ggnypogmc.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghzjnwafk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gylfdjqme.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqjzrxtwh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gzjhudjkr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gaegfzkvl.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gcsdnlbql.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gwxanelbf.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gcucmosdt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gjipibfgp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ggcodcitx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ggxhrumds.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grvzejqbb.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmmxxdjcf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ggnuceqyr.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gkyteaufv.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gcxfhemqw.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gsgsqvdjl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gdouknpos.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfofccijb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gnumfklgp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gctiaplfw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/giijpokhj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gwjighpnf.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ggnrneyao.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gmoqppsxq.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gqosqtjsy.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gdjbhrlum.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcohdskpt.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gukrrlgih.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/givpigjnu.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/guvmeqifu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gvjqhqgwh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gdyteuvwr.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gsayynlog.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/goabxahtl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gbirguujv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/glbyqwjeg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gprfljhlz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/ghvaedhem.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/grixlkxdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gqyjiyavv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gmrnaroei.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/ghqpyeryw.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/glxjvyygr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/ggiffsxug.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gsoqahpvb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/ghxhvbgep.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghkefhamc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gmiqbbrsx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gvmdzevzv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gdaaaugyt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gqbbysnaa.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gwdebdzio.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/greobxqwx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gjouakpne.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gdcoejmmh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdebtwbre.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/guegmfdct.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gsvamlnyg.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gglyefwhs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/grrqmmghu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgevqyvn.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gjxnqbazt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtzxwibku.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gkhtclsql.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gqbbynxwv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gflsbpvzx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqqgwvllv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gtztptgtb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gtlwvfpnr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gumrxtkxp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gebiaciwf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gjaxabtdu.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gdtiusmeb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gwxcdtvnk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glezfdizr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzdwntcvb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gklepjgmq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gzewpsulc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gzuqomqns.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/ghxgvmcay.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gkqmgucbp.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gmnyhdkmv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/ggiwnlggv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gozlpzzkk.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmptvkwmw.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gqqpphcao.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glkruxymd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gostaynrw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gsmeoxasx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gpihzcdii.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/ggkotywwl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gagrckixx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gbcwioeyb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gqlzdfkyt.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gwchaegnu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gfliuaxlw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gxxrcrgnz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/grdyesylu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gxcupvrga.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/giyqyebvh.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gphamivlk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gmfakxhky.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gzupabeex.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gtlvxbqhm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gxizfdrov.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gpljapmbb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gwrwmdrxn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gkqvjescs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gulemgjkv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gopuwceat.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/giigvfxeh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/ggtifpsmx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gofwwlxlv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gtwxmpjwv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gpousxrcq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/guwajuttc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gkjrnbeqk.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ghagmukwr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gkpcrmrrv.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/ghjcninfb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gshdlytda.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjjtmudoh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzbeocb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/ggzwribtd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/grdembxej.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glvmmunwo.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gvnhqflyp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/glxywpdqx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/griksfzfk.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/ghcgzpaeg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gvtjviycs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gfddwihur.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gbqrbddzn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/giqrkyrkn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gwkfobzor.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/ggogxsjbk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gqdgblwnj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gbknpceve.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gwtmsasep.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/ghosfzaqf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gajmkmggp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gtmzckirr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/goyzjvfmv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gyumkxpwh.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gkzgbizcb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gmccqvyaz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gjgjqdtyl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gkadbhqrn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gfmhtiqkz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gijiusoxh.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gxtskybel.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gehudunqk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/giecqgigu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gutkxqkxv.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/guzjpynij.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwvykjhrn.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gbjqtvmcf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdiscfqxo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxxwuijgb.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gekewekbt.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gmyxkmwkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gufrldboz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/glhkbnknp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghwgjopra.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gotqnqvzl.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsipllijo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gxrdmocqd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gzzjtszxc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gvvzonywr.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/ggagqcmyy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gxazckcwe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/ghnhkzoui.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gzapgkscc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/grppwtgnl.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gbhednzya.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gxhmitawo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gijfugvdr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gskwpcsrp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gbyllptew.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwvljdpyu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gojjabftk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gzlkkfxkq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gvinwmavq.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gqycunxao.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gsuutxjqh.sHtML


<!-- 参考信息 -->