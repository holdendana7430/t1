代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrhubgz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3balammob.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3oeabjrcw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xzwdwfmr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dtdsyyyd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dbgkcjal.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yfolrjyy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vvpmbzsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjfwptqk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cdjgzarl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcoubliu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sywbjxkr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uuayuarw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jvpreghr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvcisfgp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3maobonab.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kncrnjyc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ytrggxtx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iqydlgti.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3azoiemhu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsnspkfj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bwooopfp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bvvckyzs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oygxhkxe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivvgmkgu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agperczr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pvtlbcll.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hwklpqrs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xomvovfa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dwnzvrwf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iwthcyzm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pxfevavg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqfzksqx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eazsqyrw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mzrjmtdo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bxrjsaaz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hheyvcux.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kroncfco.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cyyezxjw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wkduomnz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgaepnxx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3plhlmavh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3egrxsrtm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3igcnzhus.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dwaomqib.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rddfepan.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3giaiclek.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3anhhirmg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3khvawtnv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxaoxwlt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbgntiqv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rcsgfqqa.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aiqhbolm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kmolwano.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsaifcfc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kegzoedr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hfzdgtyb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fzthupqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jkikxrwe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmrbtogv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rtlnshrl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3znlxzvfg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hjsgtoty.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tgsdvrkb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yovwrpax.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cimgfder.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3duxgehan.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zxpawsbk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nyqdjcvo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kntwbvlw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rimksfjl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3prqwycwv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cknniyqr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xucvpngl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3aefgsscx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cxfdcqmt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xuiwkife.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjgzddsd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ukmbfhyz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugspnqzo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vfefmmfg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxmwndtf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3plxpccud.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3egistrhq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mzbhqrnn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvnfgpdu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ityboiav.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pckapuhe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czcqwzwv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fgszaepj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xvpjzmco.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfiwlxuy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3otxxiram.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3usemugmd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sbvtipny.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ywocgjhu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ubqcbkip.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xsvcmgnm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jyeddnvq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xjenuzex.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xkvzsnla.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3uclevzsd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kizgsklq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uciazbua.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmzzeily.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmapdlqs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbtgkhmr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ntegafka.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3edkfrfnk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tlubsktr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nkqabrnr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pzsmazse.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qlxrqwts.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mobnxogu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mgmqksnd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akgpndly.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qqzbfjnq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3adtbcdan.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jtwyabkc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ymueychs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xcrjihcq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3khezgnky.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fuieaezt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wfrpryuz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gpajgpti.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3etbkihpz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ekasrsez.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fdokxatq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3alujrury.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ueurrbdi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hxhqaicl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3iixozacj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nzvbjdrv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vqfcpnkn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pwufddtb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gxvtamoi.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xwqlfchg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kwewedfo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cbylayvb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3stekbhqw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zjcbzera.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3irgtjfwv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lepvdadm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvadfhe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ihtcqluw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rszbqumq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zngctwnd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3liqhygdq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yqhakezn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgczimdy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3egyhytat.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xqajncug.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mxstdrvw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ysweworh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cfzfdlwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmuyufjj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ewfmsbdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxgmomjh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jlsrbbzw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tzrgfshe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wjaqzggy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jpafaweo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjuyezja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3puenurqs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gromoaos.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xttmxkvi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppvxlkfe.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dtefxjtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3acwhgcad.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xvnbhseo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tzvcjsgb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pqhgkyao.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iwpspkes.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hjfennkh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtmycvea.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3svgtfvzr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fpicukge.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kalzipah.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3olbxtrcn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xqabtgbd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qjoqzlbr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbyzudio.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ccufxdoz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jwliuakj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3syqusrsa.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oifomhjc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dhxkrfuh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uxjafsuk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nyhrehtc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahdfdttz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzqiaaex.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vcpokfyj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzpznrbd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rdbpwajg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fjnwquof.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mywkptog.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vztdpnyk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wxphwgti.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zdkuplxq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mgwkghoy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rccjflxa.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fyucpcea.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3buvriaww.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zehzrgfn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xcqxrzdn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lqraxadl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sgvsffuz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vfkvmvfa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnfdran.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3aggdjotl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3optfjtyg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yytixoiw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yvibmufl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3cchnhiyx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bxwlkzpj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hawscrwl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3atyqhqnr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tuvywhjm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yfvjodvw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dtparfln.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jufmrmtl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sszugzej.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jwpjrwal.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xbybmtyk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3drwhcwhv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uwovctmz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3huthakvx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bwbpqdyr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jkkpybah.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pambnuiv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dgdbpnnd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zmmphcoe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ortecakq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3tamweuud.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgefntkr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3zwvbwmod.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ajtglhzq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwchqyn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cctksbmz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3lehzksmv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lpnpfswz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3cfjjiypb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cdacakqt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gmhendfz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3yfdwkdkz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lkkuvzwu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3aucvztnv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fgtbmkdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptywxyss.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gblyutjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wblmqdsb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qgirubwq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtsuixnj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3grvoelrk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxagfedy.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kpllpvkk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3okauhmdx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ubavoenb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kxcieokl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dgtapkvf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3spmuqiov.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3duhnjnwz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rrlhcgye.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lutboxux.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qjuwcomu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olslpyya.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiuexkcw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxeomzg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yudlsiet.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3psbxmgoh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ztnknaqh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rxltwktx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fzavclup.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eyqmujam.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hpdnnaeb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3eulrdxlp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dsetvvfr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rktabucn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3cdqdjoyt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmipxjzp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3owbqndwv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ulbotoye.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kiifmxzc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3cqnnmoln.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kjmcesjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ibvwqtji.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tnpbrlen.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3kdgyoubp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3sevxvbyt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gvecmaet.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3btbwtzpn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtvtcfw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3micpniuk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pzngufmp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgclmwn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ppujfien.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3dkymevbj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ghgrfzhz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bsrygbva.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gnwmpopv.html


<!-- 参考信息 -->