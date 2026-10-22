代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vgsgniqy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwdqfykl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nhotxnjx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mlwkwylf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ugagsnef.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xahvjqcm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rffenppg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vhmjcjvo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qxlgqfky.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2efitbyyu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mjmadjow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rjwlayyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwbqclxu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dqlomrsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhcfappx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hrwicgfy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ccbmqwlg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ccvbvzjj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwdairyc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2psftpzqo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yqumuzfl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2emgvzpzf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2iwhzthgp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wexpfosy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruqhqojj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bzhnqpdl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ynfpysyk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnmttyob.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wdfdrjkm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eicqnhfr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hazrssgk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bsqpdsbc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2racaqxlo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rggrrfwf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kbxlahsr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vzuobfaj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2elnrmgqh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zylvlfql.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hbxvznff.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ohmrqvdi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tazlmskk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ewhmjwfu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ynhnhmym.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vixlvzpy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rttsstlb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2szcdlabo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgrvpras.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuniarly.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mwnofwcq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dduccrqf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2esarnkca.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tlvcrjfi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jdkommov.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xicqbarg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbaiuclo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kqalrexb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bvwftgdi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nbcjbjce.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zyrhiyvj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuljhlsv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mpggzopx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eenyefnz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqqatwxd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nknwfmrs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bxdjnnwh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wgxxwcgx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wsllvxzb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixlkipmn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ehorotxm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gwrtbvgl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ynkdznzd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wzpyftbn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wdquxamu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vbmgptzb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mcfeyhoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ojjaeqtc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2slcvixmw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kgnhroku.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rhniravl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zpmazgra.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cwmrysyv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2icvneqtc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjnlwb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzrexvaw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tzznmdko.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhmxcqsg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jcwqmyon.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wlfidyrf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2aljwzlwm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vnblcxgk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2shhofkmv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fhbeifzr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvysboxd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2favxenml.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vvprgudn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rfyrczss.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ckxseoca.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eicyxhiu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iuzyhick.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fezabgie.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rprncbai.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rsltyehw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kzeecoqt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wojzuouh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2szytiyio.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kzqpiwef.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hjzufrsz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pyvfjfeg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lbuvefro.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2biwqalnx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2exotshki.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfhxabf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hpmcghbv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fufdnkis.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmxseeyl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kofdondg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vssdmkfs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xvwsffwc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wffhqxxv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itdsulpx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2milpxkfb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2htiajgxy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mnaxlacm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ndhrmgas.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvlqpnh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rwqrtgqb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pvyjrmkj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2enqrgkgc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bojkvlng.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2aulucqtu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2upmpevbo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2shbghzhy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wlqxqgct.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lfitscsh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vyltvcfc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zxbygqjh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hoflnljj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2buohoxvh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2iobepikv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kxrjwtva.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wxgrynkv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mvbjcftx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rnjsdaro.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqwfcqfn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rplolppo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lzgunhyw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2acyenkel.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbxejtw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nfxfrzpd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvsrnuy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dzymtfza.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gdrowyvd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2blzvcqsr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ohezxaxe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibecracd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lamitsfn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2okieljzl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2axcuzojh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mpxrjlxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvikrwgw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bvijvvno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epyxnhiz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2majhbcnd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvksqmr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhcrrb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfwmyxqy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jkdqpbwc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xtywrdlf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kwgjxaji.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2efrgfyzi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ytjboupi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wmppmkxs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ypmutogl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbtdwusd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mrcvfxmx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgohrucc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dmrokvra.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2chgthtun.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wmzqdysu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrntsbrz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iomglesq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ocrbyvna.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oezszjvr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uedrnkin.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2thejzxkm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2umpcjwgi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nmaqbdpz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cjzdytld.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2srfynnie.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jvgmzarw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zfzqucvx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pufkqbfx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtukgxwa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyrbhirw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jmkcinbg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wgtwzxww.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rekccgzd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fvzlylbi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlektfpl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wnwabvrv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbjycqgh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwyscljv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsvddsyt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gametmaz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqspewi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2crgyuoxi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grskgbsa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mwadochw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pccgmrmw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aolouvkt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2soiccqja.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wnlyaxyu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dggmodwm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lotgjlvu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2whuvyiel.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2khwfvttm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2pdmdfqba.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yqqzbprc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ngkllmpq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qmlsaabp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhvvcyce.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zotayldi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rndznlqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zglyheiq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nakublul.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lfbphqcr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cbzunake.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ehmuqazl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dvjahsha.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sbyhjtjf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ectfkovz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2eolgymwe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vqbvcsav.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ngmcslff.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2biwcdvsb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gufoespz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2oqpddlpb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2iozlhciv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2frxzcdkl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zajfmlzb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ueinbkbd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2sqpupdjg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ahaajomc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wsnfjubm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2aczqmamt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2owsyjneq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qwbwftao.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2irmqftxq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nljwzmcq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ysylouwi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2zukunyht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2akilscqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdskqipg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uvgndpxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbzeotjk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jctlmegk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqstiei.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xebgroue.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkairaur.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zddpdkiq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xlzkrhhx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2relwvmid.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2aqlvufmd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jiuyzwlq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2evtgblff.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dvgiubst.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2zbutzrvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2bgovfzqe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbsdnsw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2myhpgmvm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kbxunheq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rleywwvf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eblulzhb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2suziuryl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeesrzee.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2azogwigj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2uhllwnyn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wdbimuij.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2rjabqwwi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wnbzeiqx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2scsymbxa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hpkuoxqk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2envhlmio.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uyekupea.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhwnitkb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ssfecqoy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jurtcnqh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kpsokfhh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2upkvejau.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zplyxfcc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tqzejbov.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2yngnpili.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2yaqrjbku.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wtpfzswa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oewtehjr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uqyepssr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2erdkjxnp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qbtfvodc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rjsxrlyc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2subdmegt.html


<!-- 参考信息 -->