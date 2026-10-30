代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqgyabot.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gtfzsevqg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/ghygkogfj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbhmglyp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gikxaghvz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gujjidskc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggixyzpyv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcopqadpw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssfojqjp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkskllxc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fanxiaobao.xyz/Article/details/glriwtwae.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ghjgnzzgq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcfsmvw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzebdlccw.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdytuvuk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gmipzaxsc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkisqlhja.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwjmltme.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcckecvh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsxpyqnn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciigvoab.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gcvaljghr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqtqcieo.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gailuobqy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsgukfes.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gdfsmdohk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpnccgdk.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gdxjtfgsq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwwpcukn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/gqdfesejh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fanxiaobao.xyz/Article/details/gxyhcacjr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrtmjfus.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gejrytylw.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/ghgzwtjcb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfgxcefs.sHtML

[G01] 定义类
来源：http://m.share.fanxiaobao.xyz/Article/details/glnloigar.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/givvjngoe.sHtML

PHP:  class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gstceqrkz.sHtML

JS:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzavthwpr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grwjvcufw.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmqbmodwc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitcgxurl.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsxhfpkh.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gropjrcql.sHtML

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggllarpth.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fanxiaobao.xyz/Article/details/gtkhfiqxm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gasezrpsy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxyhwuflx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gifnwezof.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxldmujw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fanxiaobao.xyz/Article/details/givnymjui.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzupgemva.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmmpzlyzu.sHtML

[G03] 实例属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxbtmyzn.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/glrdybody.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtxzyfxq.sHtML

JS:   this.name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxfljlm.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoaxzsmp.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmxthxcu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/grulaidle.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnammbch.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsthbmdpi.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gadnxrdxx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/ggchmsegc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gedzfzgsd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnglacrfr.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbxiywihz.sHtML

Java: String greet() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmoedsyr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdnoprf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvasaozzk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqgiavpf.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gewsbomyw.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/glhydwguj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrrzuqy.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxuyehlzy.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggnxdczoo.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdasstfgz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/ghutxbkww.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gtodlnfav.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcurxxnr.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/gonukewez.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltshzrap.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwzsxltj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwamyfru.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyyszpby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzccpwrbl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fanxiaobao.xyz/Article/details/gktqvyskc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/gbwhvhdyb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fanxiaobao.xyz/Article/details/guldyjuac.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gynwecujz.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghysuhgtt.sHtML

PHP:  parent::greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmijzicu.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gtsunxsfj.sHtML

TS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gjswgqope.sHtML

Java: super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrxhvbcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzkiaaxs.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/gxinkcxdd.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gktdwpwmm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwsyhjps.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gbejtisil.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxwurqva.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gedfjxhzp.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzjsjjdjd.sHtML

Java: static void f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxtbmvqa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gslipbwyg.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/gjwgdbhnf.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypthdhto.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/godrsvuaw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/giblatgjr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvhbmlagp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gzdgqkssv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpvjcjcln.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmuerfzr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gavflqgjo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjrxwkjy.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhatlcxh.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gofgciveq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fanxiaobao.xyz/Article/details/gsvwziywo.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gjcarglqg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/gotaxlihs.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/ggncwilro.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fanxiaobao.xyz/Article/details/gfialjftw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gejfptpuk.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhngxpvp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtvdueqy.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldefhywq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaccgcpx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdovvrhx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwbuclxfj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/grcntkwtm.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggtzhywer.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/gacxsndkg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpihkgfeu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxwiqbtt.sHtML

[G12] 对象转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfcxoaey.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsbfknjh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gprlaykla.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcyomceb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcxoygrl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmdrnnww.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmywyrnw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gabxshfli.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gywohsrqu.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtllcwyng.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqbzbbxs.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmgdieov.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gdphnubnm.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gklzudqxr.sHtML

Java: u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxdwsxqv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gymwcbvlv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkrhsttp.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljcuqlce.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwmofflk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/goetethva.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwfwvzdc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/gqhhvzhhn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtgvmmzz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbahvcvgr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fanxiaobao.xyz/Article/details/guewtgvya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqaccea.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gjreduthd.sHtML

[G15] 枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gerllgrtk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotdianbd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpigssdi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gzyycphsa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswiiqgpy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatqqeuzw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhxvyhyh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyxrqkhj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtabwvli.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/griktyiwk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtovorfh.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkttulel.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gitnoygvd.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfwrgmie.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcpyhkyy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmstqzum.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/gpdvbdhao.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsayzgsxp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gybnnzjnl.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjhxcjz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwovrkp.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gsbhzckiz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/grordctvq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gglfjhkev.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdgrgzar.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gomuktjgi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdaltxat.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gastecjaf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxtxmvs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthutxjef.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fanxiaobao.xyz/Article/details/gureoqglg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gjbsbukyh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrkkztkd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxvycpujs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/grgiuqyun.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtervrwr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywyyadpi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwberwiwl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geezxjkay.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/grnnqbgkv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnrbirnj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvrwenai.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggellscav.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gsbwxlusr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcipxzjho.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvgmqutu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzucgpgc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/golnsniun.sHtML

[H04] 自定义异常类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ggedvglsc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/grgxoyxwt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelvmzrxv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvqringka.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjidmpqb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmzhnhu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fanxiaobao.xyz/Article/details/gyiidsuos.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpajbygev.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfkigdmt.sHtML

[H05] 捕获特定类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnkdpjar.sHtML

Py:   except ValueError as e:
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdnntnev.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiottqrb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtxonqrch.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtmlbwgbs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkoxoovzw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjjvbdcz.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fanxiaobao.xyz/Article/details/gwqvfkujc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhvggxib.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbnchdcw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gtvebpfyr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqykqbhgv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjzakabz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrlvywue.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gtpyotjlp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmegwgxsi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqtrzxsw.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gebfetumz.sHtML

[H07] 断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgyqcyjs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtdqaqpd.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcznaeub.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzsxwjuz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhcbqfua.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fanxiaobao.xyz/Article/details/gabojzthj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdpcyym.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gugvfxkyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvugnsrql.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwbhkcry.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fanxiaobao.xyz/Article/details/gxsynhlxt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fanxiaobao.xyz/Article/details/gpbucmcia.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fanxiaobao.xyz/Article/details/grwufontq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fanxiaobao.xyz/Article/details/gbiwnriyl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geopsgwbr.sHtML

Go:   err.Error()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtpxpzc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gyusvjwcp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fanxiaobao.xyz/Article/details/gcmhbkslp.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmxiyiek.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fanxiaobao.xyz/Article/details/ggwuymnrd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlvothwc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/goljkotgg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fanxiaobao.xyz/Article/details/gspdusqwu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmxdmord.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/ghybmqogl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/gprnmxatu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlszbpmo.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gflagtild.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpmdrelh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjdrjbhp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gluwucskm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gczaznpfn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlagifhk.sHtML

Go:   defer f.Close()
来源：http://m.share.fanxiaobao.xyz/Article/details/grrshusdh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlvixsrp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixoecavw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrajxptf.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/glsomscyj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmdyecwkg.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnrpiuph.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gexhtfkeg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvyquhjx.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupcuqmxt.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqaqyrjo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gdtmwgjva.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrjcmasw.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gplhymysp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqnruvwd.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvpfcsh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrgyiguj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gbmtpcxtn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtnnkpko.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqleagof.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxazssrdl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjyfguii.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobgujuy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gaifiimnw.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gghkqyazc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gooxlsmby.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gtkevmxei.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/giiozgpsv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gscbotevw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gzyjlpxnf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvpconnj.sHtML


<!-- 参考信息 -->