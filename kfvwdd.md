代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gaewttue.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dycfkopz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qkpbjhqp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ndfnpoun.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qibuvlzc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gndsccut.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ryvsryqz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2huqqbxmr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hgtfvzly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bibxxhrm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zbnvsjll.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ziyoneyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duqiuaum.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mbhkppht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnudzayz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sykgopwt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cvxpujyb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thciyrrc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cwjfoamt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2goovysyv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bmzltiuu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xoehoexj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsxnetdf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrstaczu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibouqfzq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jylfhaad.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhlfevky.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uikclffl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kdtpfivu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mfkcdtdt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wlqntudf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2icountrz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2shbluvfe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tioquyyv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ptfsrfyg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nluycpcq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iemlkpbr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hdvbusti.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2iaagejma.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cjsdowmu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vfpjpkgi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bywmokuk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzlvinat.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2meievbmu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cpzojjgy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ebmlaiiz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztkqhzat.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uxpuufty.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ephfczzu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2itfeicoi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ktliehlk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wcuvsbqt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qiipqgxg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2naykxnyw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2chrvommd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kqofjfja.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hdffkxct.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2asqjqjlf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lsptvovv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2krpoqfia.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jxeemnno.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2trzxjgvg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2feydpytf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gwjyrvia.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjudnycq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ydqcapgp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qbjsobyv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qamjzpxu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zvbabjnl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wfysqvpb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2acyixecx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wkmfwfmj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oonmuebx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cvqsjhag.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ctixiuhe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2oumtfkxi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uacwmzyt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2clxkwnxx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jfxextew.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jukwnklp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2smzowjdt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvrypahq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hroxapst.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2njslmjky.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iaqahbeg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gwihnzvh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpwpsvsx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2plhowkun.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ekjvgofj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hhmynmsj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gncqxgwo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yembgnxl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjcrewyw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqkmnmew.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pzdmqcrx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkfdaoyn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mndkecbp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uszdstjg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ketebujn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hwpesxph.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jlvtyehz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ajmvibal.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nzyaxwuu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bcbdrfsu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rnneeygw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nqzvmmde.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uccohwbl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2luraepcs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2orrujpox.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gghaxswg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2raivzycj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bbwnjwtt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sjcgivly.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsxvmcx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxdgqnwf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mjrckrro.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tckzpswo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgeageef.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iacpcxnp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxflvpoo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vfvvnfaw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fotxferu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xwxkgbgs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2itphekye.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xrdvvvlh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zupdapvi.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2abafdujx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lvdiugos.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zfxvdqoe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2babjsqhp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gkiacnxp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ctiuasof.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ndvuohdn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2obpkxwqr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hedktzyv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lexemlry.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jplfjujo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2npwywnpr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmvppwc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yopwkkwk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2apioufbr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lpirjmoh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wohmfgkc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qerxlrmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xohuzmdy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jgvxainz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lcfljdsu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2aszhukjn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2awmodzwu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbmujmgz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wirqcrmk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2olnrjppg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2carsjbub.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ymsjrpyl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2etnncdzq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2bcohecyp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xecmabhl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fknwjyye.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qqsaqyhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zscnbpiz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xlcjfqhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzjmbfig.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xdcicivq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ifpxcaej.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qptykmde.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2siahshqi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ltlqpprf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qzaxqrrj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2itbwgfbl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2propvidp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfkghafk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kuftfawz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mttznqon.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ewpkvokv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibppigbm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlelsjnn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xwwtqlmp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2gubwnkes.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bchmcibg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2awrdzfcl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2surpbdvy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xypfzqez.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zcjmdtry.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iymjgtda.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qysgzywu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2niljuwjt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuplypk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hthpvkns.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gmhmwbfw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqyptckt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rhpozbjt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufgtqpvv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2suzdwavl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zydudmqn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzdptnka.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2smrnknhn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ulyvznvh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hxvxlqhp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qeqasbyw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gbqtewnj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lradsfdm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xwebhxzg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wjffrnxw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mdjanagh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2siicbfnq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rmhnbxtc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2slnthjtb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cpdmsgtk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2flmasnie.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ipzndofa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tgtihjus.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jrtklwti.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kyaoqtyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2sfavabka.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rcvdqlfq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xjwbfwpk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2unwjnmuo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wudsvijp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2idqhybny.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2akqyyqqa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yhtfyvfk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ljauqutg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ngctgkaj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2krjyghxy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nezllgqt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2xkycwaxq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2znbvmpzn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dpnpusqr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ncudcyet.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pfapsckw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ospoyhiu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gkgkomgh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2cgneideb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2shkbncsq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2otbuefcf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ijtbkybx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kgjfrlvr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vlxhwtey.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2otgnbhpd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcedorsb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2llqzoybu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ifzbnfwt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hauvlehq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vjuhcpzt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vmwakqyl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eazhzpqh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pdtyxwlg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dwosnvlk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vjjmilca.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dwzwfgym.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wdgbnjtw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajpifhfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtluwmyb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oebvkslb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltyjhqpl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oatddjsa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdgttxt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqesvyfk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bccqviln.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2oofsdgxf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ptslxral.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuepcqbh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2encqfmud.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kmamcxeq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xxvmdyix.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2thfocyvm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mgijxxoq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2juupigdp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iaatxnbt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmuqudjn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbpdhjz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2eiaqnokb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwdyseuz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2cmndlohd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2begihuwn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2wqwcwlet.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dquntaaj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pjbhmjam.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tsriscpc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2onhjdwds.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qfdryuns.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2biakmsot.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lfphnxae.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2skyzifky.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rcxsmqlm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2axrwarbp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2potrxbqj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mcrejqev.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwizzhv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mbpedtsl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qprceyuu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ekqdetsc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2cbkdhsyp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2loziwtle.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pwkdsppr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qqxnvzws.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rmeqqsht.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zsbuvbxw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbfpmqn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rhfyqozv.html


<!-- 参考信息 -->