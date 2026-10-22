代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bvazhznc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tvwfwjbe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2osgvidsi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2apmatnsq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lhrokxqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2eizzcuth.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tkpjqfdf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nagdqwqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnxyguha.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xustpkze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzedovvr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2esqzhjiz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zjhpvcao.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ruhnadji.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkglaykh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbnufkus.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xbcwcspd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ibogaswq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kztsxfsj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vczjgoqm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2imukdpzy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tvnutweu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uozbebok.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2olyiierw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xvuabmow.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qvzvkjtn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gysdfwph.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hhzdrczb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urnqekhw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yfuilfcl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nuvzfghw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2axmmtgtj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdzrlwvs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2riildwen.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hlpnajxf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qoqbbjgf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qydrmlcp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gazvqusn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jxnzzjyi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fqbcmnmd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ihivvbmv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2blvqzkqg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysgtaepq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxyrady.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ludeoohi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tglhcdti.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sxqtunlo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vbudpjaw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gsemzgee.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2krevxnqm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvhipmqw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gramgbjl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvvhpiqn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yirpmzgj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fhzocxgr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xpwfsfzd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jldkundj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2upnliptl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jvdcvmjm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhpmfkhh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kqxbvudo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sgplbuuq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2uprhxiod.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vkrnhovl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jltovrjw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tobwzjyz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rmszstyi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vaeizhga.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nwznswam.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fhjvwxiu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dduelbdc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jkhtykkd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wcmorcxu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wbsblggf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2crazftep.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2csttspld.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksssgpaj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgiawzhf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qetxhfxj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlwdegtc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bkruvlpw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mkkkdhkq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aysmjsmi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kbyksjqc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wnlzgwxd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2koutazlp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fafsyald.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pbbsczam.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2omlfnliu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2starkiij.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qnlcsgjx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hxbfquyo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uubsygqb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rlebsgwz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kajjwdno.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2triwfpee.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bwgqfiyb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rxappwsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2twyhymip.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2opyoaknz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hppeohtn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wxzzwfzp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zpormfzy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgtuymvj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uuefzthf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rxidgctk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lqdysdsc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxiulkz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bebbefnc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kavjvouq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exexbrco.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zzxabdiv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2krrtespq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2emqwndrq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tqdvlolx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ykcqnvel.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zzibowep.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2roytatcp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bhfmglmf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rwshuoeu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2twgmdtjj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2akycnfka.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gqlwxtii.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bswdsyee.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pgqutxuv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2khfozqnq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fyaokekf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2asmqequi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wqoiwvsh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cswasbhj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cakrgesh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mrlvkimw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ogafulym.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ozkipppj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qkvslwlq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2abhzzjjb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lkbbtpnd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iaciqxxr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2erotgwzo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvticyfe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2smzrxuxu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oewsrbty.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zmwpctxx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ezqarlwx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2filkzamb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tnupzgkh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wtldbydy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lrfhkvgv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2strltvdj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkpjjbd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogmeurwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jzwxwgno.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2swbifsro.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2drshjalf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kjthoxnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idqzzsuw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vmvaqjiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpxikuhj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dxywdmxw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hdltwuxq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xrilhpwa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bashxcmf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2klzcsuxp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2whionnme.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ydpjhbyb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2seqcbqrv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dqqqvkmj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qcmmrmeu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wckmkxlz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eapgwexd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpkyatsu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpzhpixu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccnvtkpt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ghzesxan.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ggvxfpkf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2itqfpcwe.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lgfglgrv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mzhcsqme.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uulusgfz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdkzicay.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jhqmxnro.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2msihuatt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxmumcg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtxhhi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xdjsxzfr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2opnrwoni.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qvvsolxd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2issdpndm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuhaxoew.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpciljlz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hafafalv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2edxwmvvd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2luvahjjh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2nceyrdgw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nbbxogmz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2eejmyhqr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxyrvtxi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jvglfkey.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhgcyezl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ypzfwzlh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvwodml.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2punpnxqd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vsvvijjx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fgalvepb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2edogrcgh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gizadnlh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mjeydvxg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2erxnxwaj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2klfgucha.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cndtihwg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jkghyndu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dxzvilsk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2dchgzixr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dozlxpah.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ixrvymyy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aaegivzo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2enpdsots.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2frpceakw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mgujloni.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tsgrfucm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pskgxaij.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kjzkovoc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xnlncrzz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pqukrwqn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ukhaqxbk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ggrciabn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kpmlofyv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ssjqldoe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2oyueanhn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2iceugpfr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pxlvzhdi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2onzthtoj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bptbscfe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vhwalyiy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zotwtjje.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmjkgite.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2olyddlit.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2zjgprmuo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2zolobrfx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2tyxabjvw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jwiknmga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dhzotcul.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ovaxflfh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kbeirute.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fmpntahl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bnpnxoot.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yoaonhyq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vawmlpgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbubmskw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jnayyixm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jljalkgn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fksodaxs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oybesski.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtkjcpez.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vmdghlet.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jieimbqk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lzjrbrym.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcbjmcbn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfmqdst.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pdujnnxs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qacnhhom.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ebqerkgf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uankunlf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2yxcqtmfr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tdflthxw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kmwmhlhy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2totopjhw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2aabttlbi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iutlwxrb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2uoemkoes.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hqcvhjfl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2msicvrei.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zchykjpn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rwjidort.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jmpzascc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hqjymabu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ytodczyn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2epukayfm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2alpiknxi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ipfgvzas.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fjfvkvej.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rxugaxnw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fjxsdxiz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2prvsragg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ducqyqoc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqrumtk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mrwativt.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vlrnnoru.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndglncld.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rexpclqe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dmdsnkgk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uhwpwuiz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xwlwkjtq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2empthyyl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2knkgzdyu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pddwlxtq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wrtcwuua.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fxyyejxq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2cpjpbhiz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2giopauoz.html


<!-- 参考信息 -->