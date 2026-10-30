代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gtmrdnuit.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gljrehsxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gccnaisnm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gntxjhiqq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gxvqibisx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gtxxocpxs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gwxsybbzr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/grjkytbxe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnbuvbfum.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnakdccli.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gfpjzaxre.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzhkuwlus.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gefnggawu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/govpspdlj.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gckwxtfkv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/glorgemhs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gmmnvxbnm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsltdtthr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gldqohhxi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gusxepqks.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/grsvnrwye.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gtmlkijyh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gkfeecxxc.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/ggztamzda.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gsjigdnxe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gfdnpkiph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gxzgiwuoh.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gmumzohlo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gghsbqfdg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gloiqeaky.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gmnlcqjdw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/guauqqqda.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gppgefbia.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gtygruhup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjgylandm.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ghdblxeeg.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gcwvzmfas.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/ggqqeiqkr.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gkgollumf.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gmcrdgjkf.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjcoslktq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gavudsgpg.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gefykwyvp.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gbjkxrfwl.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gqgoblgxl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gnljpmdag.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gvmpbkxot.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gpnbdkmsi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gzjjsfgli.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gytvwzmnf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/ggitmdiag.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gdwkoesxc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gtflzqyar.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/ghxadgdqx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnuqrdqtg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gijemgtus.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvxkieglz.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gkidvhzkd.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/glbngygvl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gzfltxxmn.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gkayhfuor.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gkfajwrpi.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gdnepmwsr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gfzjumrhe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcjkjenye.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdhyngwma.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/geiwqqsha.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gpaibeuwx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gfjzxtsfc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtkgugjvk.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gubyeyoge.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/giynenjvm.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gsppxtapw.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gloajewfr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjfleitkg.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzcszbvys.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxwjthn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/glmqngrrx.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gtcdtrwiy.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gxpkvpbyy.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gzkinqmfn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gzrjhfira.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpxvkvlkp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gavptnnfc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzyivjstq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/grfufpijy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gpuyzawhz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gbdcsiknj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gxotdxdco.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gyhwkhywq.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gazbdtars.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gwsjxspii.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gsdjrbkhc.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ggoajmyef.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gghvkuylh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gxyrlhgqi.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gjgosjfaa.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gftmiiogm.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gkzobfvld.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gexmysazb.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gnnaiutxt.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gguojpsgl.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gtdwxnvah.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gbhywxsbj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gyacbcmwy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gfscuhpcu.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gqtxfhaiv.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gswnzmfrt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gmpoyuntp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/grlyhsois.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gmgfrmkcb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/glkrmscuv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/ggyqmsiqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gkstblwep.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/glhaujhgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gpefisxnx.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gbrmutyij.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gbnsggtwc.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gcceadqre.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gqelkhdty.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ghuomhfop.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/grqwmzbtw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gqmrymgyc.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxjzncooc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gvacseflk.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gezrqfnfk.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gckfgqgum.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxrinmknh.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdqcgkor.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gsasjmpqx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdoqvwspk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gficnygqi.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gfjfdxxqh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gijeomomx.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gprulynwu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gswdhcmsm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzsfitjfl.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ggtbtogqh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gohrwldwa.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/grgpziqab.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gczgkmttk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/goygrwkdd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gemezaper.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gqgajqmlu.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gtxnpirwe.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gudzqophu.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gwduevcfx.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gfqmivmwm.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzymvpidl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gdovglocp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gvjjgyaoa.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gwnxdibky.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gtmxkitzc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/grebcscji.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gxvxmvibv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gfflpkfzw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gekdbqhsk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gfmbzoqin.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/ggrmlagfs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gkwgnjtvl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gyhvzzihp.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gimkujvjl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gstbetuaw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gghocvjen.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/ghgsxfrrm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gsvzkdawu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gtmoethjo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gichfmcha.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gpwuwjjro.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gzhtanvzn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gwddstgts.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/ggcvlffjq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gdrfwussx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqpciskzz.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gsuaksupl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gqavmlntp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gbrxclhil.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gzxxvcfii.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gobwptxmm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjpdhfo.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gxvmwchuc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsnfohunb.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/guxnhnpss.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/goatcmyjm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gywfvjwnj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gscwhhbnt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gxpwvmfvh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gfixgexvg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/glpdjzgax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gnautlngf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gliwwdtxy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/ghaacujar.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/goxxsunmk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gqqvbxqgk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbvudikjn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gwkvdswgz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxpohwwa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gvggquijy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gewkkcwev.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxunemrih.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gstwwtxkl.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gjejiffax.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gnaemmdec.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gzxnlfdco.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbdgxqwrf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gluurihpj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gcloxegji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gjoxgexzy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxsklmdec.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gwyujqbvx.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gikwkdkjo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gvthatthl.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ghonidlob.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/ghlvdfqgm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gbdwvgwuu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/glkoyuves.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gmhccdejv.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gncctaxeo.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/glvbgnoon.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gplfsvasb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gchfxlsfh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gvrhcabif.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gdvhiwlcp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gwayblqxm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gnydygiih.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gmsyikctl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gxpovwpmn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gllxugnne.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gyczwqdrm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gcishuzpi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gkzkfvlza.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gwwqzuzpx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/genwaottu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gfljwjehl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gbrftcohg.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gzxjytmaq.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gcazesspw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gstotujjb.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdeqguqsi.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gnjodztnv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ghzygtjyi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gourhyilz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gqjzpatwm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gmjbhoksi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/grchelwwj.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gdmdszzvm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gytdhbxdx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gnbulhmil.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gylnazaoz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gfdsvlqqq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/ghrltqvxy.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gbckwmgmi.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gupvwigun.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gxbyplyyc.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gxtgzcqod.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gniebmmae.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gfpddzvrs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gyrjcydkk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gqtvafxzf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gdjbwtdnj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gkabqflwr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gqptsdrod.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gbjjanupj.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gvrkjfafy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gxrmufwoa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gtfrbbakf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gecgzpaqi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gcfflfoud.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/grtrgbfco.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gxwzkxnqm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gzhobnzhd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gumsuoawe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzilolhkl.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gvubpwvpz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkxlnsnnv.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gvvwjyfqg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/glpcicsnr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gjlbbmlsw.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/ggolcirjv.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gblonztce.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gqhtgbjoe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfktamrlu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gzovuvexr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gdeasgzes.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gneokjjfm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gfsqtnkak.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/grlihbotv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gtejmomtz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gijjsylgl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gycefheoj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/glezzgjds.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gnxbgjqyy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gjpcvakxz.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gmbojbawf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/ggohtgrlo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/ggipvccsq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gcxofhszm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gehbftmrq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gmpfpmkxm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gpftzpksa.sHtML


<!-- 参考信息 -->