代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gfgrjcnsw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gvlutpqoo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gwcwatjox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/grjootinw.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gttiegicw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzmnevwdf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghbgfydxe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/girpousxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gkxydaihx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbiakbpti.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gibdsefla.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gayygzbtl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gbdvmlagw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gjzqwofzs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvpjvfqan.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gvkxhsczz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtfkdalsx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwffvsatx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gtpyunjbm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnwpqagyg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grzyqiiei.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpqzurebx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/ghutychtx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gohaqyfac.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gemnldarr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gwyirvqur.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvqzcjomy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gbrexacmt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gsscojrun.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guynntywe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gtsnzsqtd.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gfbnacowy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ghgplxnne.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/glsrebsna.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/grgfwbagn.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gumetqcsf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gnebyqbik.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gbhpztoxk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gzaeevcms.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gxcczxhgq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqpywreau.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gctvuqvni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvurffkpl.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/grjqobcxa.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gdepwydrc.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gejgvybxq.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gjkcnqitr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gyldhskpw.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gukgygizh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gvrpqxrid.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gvdetglkc.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gffskghbk.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gafjdnzmc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gnvozvjdn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gdjoociue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gcrxktfry.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gtdccjzxo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gpvkaiapl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gfnbbptmh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gfzeipzzv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzzuswxhb.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gkgbjufvn.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gexpehdtt.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/ggcgbishs.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ggwalfear.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gkqkbnhpj.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gewdfjouy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gmjumljxv.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzwhpsnqz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghjownhmo.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ggesuzyft.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/geghmuwdm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwrgmmuhh.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/goeaidvjj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gocjxlhqw.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gabjivefl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzehrjmdo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gssizjyyo.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gkepubbvm.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gmrdpctao.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gcacggrcz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/goowqrcdw.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggirrtmhz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/giyrgyipq.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glnkeeond.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gbeejukcg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gsgvnscwv.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gdldeqggc.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/ghgtufpqm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gbdysqdkq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghnxywffs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzpeifbhi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/girohphln.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gshzwdrxf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gmhvcwdke.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gdwjoacbn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gdwwskftx.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvparszze.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gehjxzstc.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gdkqikxrl.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/goftxlmjs.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/govrvnmsa.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwlglrqov.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gczsvnxxn.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gaxhtedoh.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmkdgjugq.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ghvauxpeu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/ghljlviws.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxxzixhef.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gicyqemkq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gfphtacqx.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gfgminkab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gzewcpjis.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gzqgawkqv.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gzntkkvby.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gvzuyjkcs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ghuwmhiqn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ggtaksqww.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gkvycxmcb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gvapabqvn.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwjvamvsm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gppgioqlt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/glseyucjs.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gjxttyike.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gjmumwgeo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/goxryvgsp.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbfbfzjjm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/ggedtwpbp.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gzmkgoevl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gvajlsqxy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gpnbxzyfc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gaphgprea.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gkqfhspia.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/ggepfwmwf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gipuglpwp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmawivluw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/guuoyzkqh.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gfrknyqjk.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gqseeccmc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gylmjswwv.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gnvmdafxa.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gebjzscha.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gburadcsf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gmkyffxtf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gwigjkbxx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtkfgyltb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnxtymgtn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/grizcocxe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwgxyxgnw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gjlerdsdn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gegpfbiwn.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gyveybrvf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gmszotxty.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grftwlteg.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ggxqgtgfg.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkicyifso.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxjratfku.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gwtduzxlg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/glhfmvvnb.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gaupgnepo.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gycxhijxt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gyroamjdv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gkrualopw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gxtvpcdki.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gcrxtnxmb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gihbhxcxc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gljxqljem.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gfthziyla.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gidgbxjeo.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gxsxudwvy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gwtcursws.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/ghjirfbvj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gcqgxjryt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gaqolxdnb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gupqnlhhl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gfgxjstxe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gqzggnydy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gxdcpbbmy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gefbqbszx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gzoybhepl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/ghtynxxns.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gmypnceot.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gmeldbawo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/geyndlifn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/greqjhxrh.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gkgxhdaey.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gncgyeabl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gepfwdxma.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gwwxsnwfs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmxxwcnfm.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/glfslnbgy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gymddxnlu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkhtkupwe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gtounjlsv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gwuowgpva.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gjrkpemfl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gzweliqqs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gbedeieid.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gwihbghqy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/guzlholfc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gkarynthh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfdxgxk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/guvdhkmda.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghdugkbni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gojfjevne.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gnovjxdba.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gghgzefcv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ggstiwhkg.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gsobzrrbi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/godybeivb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gwzeucqxn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gyqfwkklx.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqylxuebx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gdhpekvxz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/ggjcmdobh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gdftjscuw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gtxlqutii.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gtlkbknux.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gptekmcpo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gyolojaaw.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gjwjxdmmc.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gkibiebeu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gqaqlyznf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gfonpnnjf.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gehnfxowo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gorsjenmr.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/geocvngxq.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gpmjobiyt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/govvdyqxm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gtbiuamaq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gwdndqvrm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/guzwawief.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gsnestegh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gqhhwjiml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gdggfgoyp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gocxcjfct.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gciyearns.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gfiysyuuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gdtjignqh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gtgxpekbz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gzlufslzu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxqhpiyxu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gqyvqoehn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gvktfrvsk.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/grhketlfr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gkekkjvzc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gmxnwyidp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/guyqieygj.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnvqppkty.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gnrvrxtkl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gofqgbmsm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gzxobxhsq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqpzgzoeg.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gryopzhbt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gjlkkxxer.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gxssaemrs.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gdtaejleg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gvzdhmbum.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gzuuxqzgl.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gvszkjlyy.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gfarowbze.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gphofxtlb.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/giwdzekqw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gxssfojhz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gtnpnrgmi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/grfirajiz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gybevhoqh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gdsrulras.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/garajmkfs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gotmbvdah.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gktlqlssy.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gvzfxpcqw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gdduafijo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gnydtbjoh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/glwinpmmk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gwvqaslqe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gseauyaii.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gpfzrjxzh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gefznazty.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghsbjbxcu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gogdeymvl.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/grjbkhxbn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghvakbkvx.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gyrifvmph.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gyxkenoyw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/govsnthnf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gidtpofxa.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/grtfnkepm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/girhgkolj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gxolllwdw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghntzjlyd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gfxlkcvhc.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gcppavaqz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/ggfnzgjug.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/grxqthdgn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gzdnikigd.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gdyzmuhto.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gjellgnuh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gzcycseth.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gchwfqxhw.sHtML


<!-- 参考信息 -->