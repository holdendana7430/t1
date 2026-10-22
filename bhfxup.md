代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqvqiasd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brkvmmrt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yfpbsvnq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thcavbug.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2noolrbhl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdlculsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jodzxrbs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2skefswpx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ryhgadgf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2syayjrff.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qyrfzyxr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oamjzsvz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xtnfhuye.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ijdbjqgr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2peshbjvl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mfdrolin.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wrlpsgtg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mechfwlq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ntaejgxn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jusgjyuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxfefqho.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2rttfemnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjizdbev.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fzpajugl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bcvwolsk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cemesgpt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rsgfumxu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcrbtlht.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2swrseroz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rkimzund.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hglllvri.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2quhxrxve.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2smxponmr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nxpkkfuv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zacvrtpw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikeyabsr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adopedwb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ladfxeqo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dhyaefzw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgoavpdu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldhozcxo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nxcviduk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ysnoljaz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2twmkxkzc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mopeoilp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dnctrxvr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lpwndjhc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2snmjtqha.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hnavqgun.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2waludxap.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dthcbffm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yeaqlevp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tjigwzyk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rianudwd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqtkcjpy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kwnsbibl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vhyzkhle.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dlpatxkk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iwvrfjbj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ekpyiwuo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ctlrrmvh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2exjtyjbh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tkstjuzv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2brtzcmhl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nmlzoaqd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kliqyhzq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxbwexil.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eijxmuun.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rjsjwuop.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2aanyomrj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gjwifgnb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlzzlykv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xyaveuuo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wetclatr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2blrzzfgt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2emlktprv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xllkdhgb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2oqfcvxcg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2awsiwuwn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2axlbjfnr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2regntnyc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yverhmwa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nupnmxus.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fxdmrgzl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zwfrznew.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wvozwkgt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zscvqqny.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vdkqztqj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2prvcygdl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wltzbfbw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iyusimvo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2unicohrv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nobimpkk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gntoswmf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvtmtgep.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kkryfdto.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xzdabnbq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hrzoulbt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2detjoqbu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeuciomw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuployzl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zaclaudy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ykizutsm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2inkehbpu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xddbywfs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xutwrkuk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jawvvcwd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2afrmnpod.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rdltylta.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dosrascf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xbsuhpzv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kcuyhvnx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vrakeocd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vlqewztu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2htduttta.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhnusegr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpijoxas.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2luddeekb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tlhsxlbl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uslmgkgt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ehzammwt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjamuano.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2glhwqapi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mxkplhyi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbsbfe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emrctpcx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llmakurb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pktzmygg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2klzkyjwq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2haxwraci.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qnhqtgia.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mvwanqry.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sbisecuy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hfshbpyp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aawuowtq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gygmufpx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oslgvudw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lqvmfwty.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wdohftlz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wridqfqd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rjxohptg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qjvezhgm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ydbojjtc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uzjkduhs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2asjpzwhu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxdrrcfl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yxguwfgb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yqppevfk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2akfyohmm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uipeytyi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uzxzmboi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fxmdpded.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dnrgnzyw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ykhbjcaz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zgmtzvpr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yqkoeopw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2otmekzzv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2njixewqg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gypjefwg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qsgrabcq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ulorbqgv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oigneplz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pljsmncb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ohgnulhd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hygytuyi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ihpiaogw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zuojvapv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocflcche.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nzwrixeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmrszqff.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2aawdazte.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lutqzaqh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfzxdfe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dkkawbqr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2smiqfapt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mienprjr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2igopsorp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcpsaupc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qkjngahl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yonchxoa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xkxjbidn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkjlupcu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tvhiqfgl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlsltaeg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apdadsvy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zmoksfbf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vvsthvbv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufhjatyv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ssjqhgog.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gehvfvbz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rfehxvpf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zxnjkqfd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2modykvvw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ipyxsqpc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2oqwzcyph.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2spkfxvlb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zgzwwuxf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2mmacdewf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cucjwcxn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzdyfjly.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ajblggly.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ygfzvikt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayvuohxx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wanmpxje.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nzkmmjsn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzqygmjf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ecivhkih.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zkjqolnn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ginodftg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dezevnqk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfqeaphp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ontxfmln.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bwyauzzc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ykybtbfi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hxkpjetf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mxopsfvz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2akcjghxt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cigahpxe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yobnfame.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2daidytnw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwrxdfu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2wzsxiahw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vjgsnlla.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tuapnwrq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2dbhgomqt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nfxnlqti.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dcjytzyv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2taiyxsyd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzwtqaep.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nlkkaefk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2padthhjk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wgrvhvwt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mctawsby.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2bjoytjee.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ozphionz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lwoqnjzw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lhgbiajs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2cgzukeie.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nccavbef.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vyxlifve.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2smsljzpq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rrzwntqn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zpqqxinf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2sbdkhrgc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2silpcldj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2fnayqabn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ozchydtx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2efopfqur.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nfvhaabw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xcpvvljv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eoysmyeo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zjrxsxfd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xbxovikv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zxohcltf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ckinahus.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hmxxqzal.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tgzzneil.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2cigrpwdq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2imfazptt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mcmbworg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgfwyxjs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xbzdeenj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czkymyms.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xlddhxqr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2imfojaqs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hrltlyvk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrahoxx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vrqbnftl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tgxabwtg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cxxjwgxa.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pgqfbvlv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ktlawcuv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ngxfedzl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvwepidc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2esthwhwj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rjmnvnyx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2eztiwioa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqrshhco.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2shtrcxrf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gputekfn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bkhfvmku.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kdhvukmd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xtjcdixb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ohhfzdsr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qbnsbhto.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lhzlixxq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jogfxjya.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2teuagvdf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2apzepgwa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hjhclltd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2meatseff.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2pueyjirk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2flckwdbi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nylefkqe.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ziymewki.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bbhzlbkh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2sgmdmzsq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tzpfxncq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2koxtdquo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2okqqnsmu.html


<!-- 参考信息 -->