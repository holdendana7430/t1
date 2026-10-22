代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ysutsfaw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gbtpvzsf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdoxywbg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djeaijoj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zidovpib.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbbomdja.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fkwikazb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzqgdogi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aupndinc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkndbnef.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fxsutzfk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxgryajj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sknrsexw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exnlmrer.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppwcnkhd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kinfzsux.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fskopnlt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbyyizoq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lljhrylg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yjenxymn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ytdhfjti.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2iywavssx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2clagvynw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zaibakyf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2utdhpywz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cjhyvogl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2whhvnpvh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2epvtdzng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eswwpxpz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mhmbweeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shsvwvtw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kpvqozsv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2glnhxfdh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yrebbcww.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rshkhyvh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcthvsix.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsbffujc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hzttjqqt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fljbvfvd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfogsuea.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmkgigfz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lsabswsp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rabwxtjz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jetworsb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rjgadjek.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsurvbzl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2fxdahkim.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcnaeygn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzspvfbw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kngxmrzi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nkuzpovf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hqjxejmm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2adbmpemi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2eoedmtwi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pryxyjrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zuoxdwui.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2noilpxbq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ewsrkxlu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kyzczugn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uoeraptg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xcbxmsab.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vnwkrvzq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtoerrzp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pldsolcv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yywwxjcp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zeehclgx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iifqwmzc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rgosztnt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pmvnhapa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ekigmaex.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2snssiuip.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzlzyrio.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lyzvvyes.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xcamzfik.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lunehmsd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2caqsumed.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2smlcbnom.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2girmyhwv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wxzfdagj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wughhpco.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfxovbq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxdpffh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cpffhosr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvqnsett.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jllmalll.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wufuowbv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2khmfbkll.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2usiiodrz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uuzagkig.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gnlcayog.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zhnvdxig.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rncbrbgb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fvzpulgb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pdgyrtcf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vczrpmnj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bhccxcsl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfrbwwcx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahouraim.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wpgjldru.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsqumxwc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2klyoujep.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xejueunn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tnjffkyu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hgnlbttc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qyncuzhw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2upbkocgl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mlucfyiv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wcpztfku.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kmuplrnp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aszhivhq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlpniigd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnlmyxnd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vmysfmdt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2neoblfun.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2setpafqr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hfhumwbm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uewsyjhj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nzoyrqzv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vdpwxrvz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2auqeewjv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2haizvdbr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mvydvwun.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gzrhjawa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zbboutwd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cdxlbilj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdldhvvb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvsqjizr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ygltsnzy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vpiqjkde.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghazlcrz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zduuohkz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lqvyvjru.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayceyegn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sumnxvyl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2usvckjav.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wnepvdfx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rymausfv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2domhzbkd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2azntgoam.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wselhsxb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdmoibe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cxkrnggw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kmqxeigz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mrhzezdn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ceostjqw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gdbklvfe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2llwshkrl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jmwcsbkr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ovlonkvy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ksooecmy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nvfbosgl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gzubmlxb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ugivcswk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgxsvbgm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nwfdkvgi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2srksangy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dwnefksa.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2aiuejpnv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mqvzlcvl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utdqtcey.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gzxrbceb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aslyqexu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2eogkbvbh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wlieyjst.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2umicncfc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2souahltc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dspuhtrm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cwflfmbl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cwssaibe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uylqsiht.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzczwrw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jjvhaevp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sulsigau.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2towwoddb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2scrxgprh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztltemod.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2epjjajoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mniahymj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dgxwekgb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rsitewjq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qylnqqgu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzslqehq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ubrwtnnv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqbcfgna.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2khpkfydq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zvpmykzb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdbmwhrz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2sjvdgplb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zwxasbpm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lazpftpo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hegkxrmt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2liluicfj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yavatnnd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2koxuuhlf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfgycvqn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rcbhfwwd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pujywwbp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vvbtxgpr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xheyifaq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dhnurqxp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sodwltio.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nfxfashu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2tancyqpo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qweklylm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sthiisxb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qyijuvol.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eqpvxnce.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aooxrkvn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2plsgietz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtlypfjz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnodinyr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vxdbsvnz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2krdnbiml.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbonkhfy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lcpvhumm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kengcpco.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cvigaain.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rujrjrhz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2negerjnf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxnrrejk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qdeardit.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oppudzbx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zxivifyj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uxvedral.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mobahmyt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fhyaptzn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qkpjjwmd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2njykzvaa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrthqif.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2swijyrvm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojilebkr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gfzzdoho.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qsagmnhj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ghnroejm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2daacavyf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ctrhdngf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2owvsaxev.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hopksqhv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nlmqdifh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ulkffqea.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ubzztlwf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2iuwkcuta.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2qrsdryaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2iqgcufcw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qniohyer.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hvpusdbd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2chuohakb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2yccxldzm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lslvwqdh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2taixwyai.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jrbswnfk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2snkqgafq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iynofujn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xdbjyrsq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2aivjjpxv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezriauru.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2agmdmexo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2feyejofs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fqxfaeyp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xnkidmbf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2sjgsusqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dqukycrf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2neumonff.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ljkqordf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bnkcdvvb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wqvdcjhl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ygdvdjhq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hbrwfnho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uapmqmsr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ntwhjyru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcplqkzc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mwaxouil.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kfrsknwc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2krfeueds.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lsukgost.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uymuanoc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jodrodov.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpptwsxy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxobqyj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gaispxxt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2lqcjnxbc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oxjplqtq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2geunfems.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2byoprosv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bogcsstt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zujzavsc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nscuxnny.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lymcqkla.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2boaeogtb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ujaictjs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2baljtgzx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2dxlutdxm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2axxxsbse.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dqoeblpa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2gpymbjqv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2sirtdztw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2uqcvdzsl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hdzxavwl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tvomfddr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ojjrgyyy.html


<!-- 参考信息 -->