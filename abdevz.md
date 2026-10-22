代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2igqcdkpu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2waqxbvzl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pygrqrnm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vewdvupk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dfavpeuo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kqehqakt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2loockbvw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wnxjwxvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojvfmsif.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2uwrunotk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmlcnlup.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rxkovpom.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hpsiqfxv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sidftatk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2floigxun.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsazxkoj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nbktommz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ehbazhap.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mymbzmnt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rmpqrkao.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2joavuvjp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ckmqkuub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2goyggxcx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnbaovhb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2abrzlkzq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vatshjgg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fjfonhka.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2juhjbyay.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jagdihio.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xbkkatbj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hbrlloik.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rerpisvu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hapoivdm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bqbjmkof.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2slfbifsg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uaesubwu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2moyrreyo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xkkncbal.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2juhrcwug.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kojepvvf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvgxxee.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qnzywkpt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdkjcxnz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsoevfrv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ijsuymrq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fqmlzjzw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dkwjrhtt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yoasojqf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hthsrgxz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qlcitqqs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iqrbpfek.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xqkolhdw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aurpqjvt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hlbesdbs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlbqnthy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gesvvwth.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qxxfehve.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vemczmbz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vbawwxbm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rcdoebau.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rkqqsbcw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcuixlsb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2larzcgzg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sjbrmowo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ievbojmf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bbniyfbi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gldcaipj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vtxacjth.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wgrjggtf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hgtwmbel.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2roazwhoa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wbgofnrw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gaobkdxs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2spzdwsee.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yxcrtglj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wanbfono.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2urkgomgn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvdalkgq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ancrshjs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nfqbhbba.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cihcqgmi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zvdcdlcr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2emschwko.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rksczrun.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qvcsnooq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bevklfnf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oapvvqiu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ashccywr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xzpwoisa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2celvvdie.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2znlhwlni.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yeaezcvm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2adzkvyuf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fuoenglm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2audphewa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jvsimmnh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zondipnx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ucejswhy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fwfvgsgz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tkgjmfle.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2upewwoek.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qxloabsp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2roxhgwfn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lualwclh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2newmespk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnummer.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2njwvbbxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wdjctxnf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2waniytch.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dtxlcbis.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rrgqsmtv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yzbbgzws.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekduouzc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lopahyhp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uymlhbjx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvkprlsc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dbmgemqt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lbrundgs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fgkbrmvi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2txjqscxb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2neztpggv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fekxpszh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qwgwoyes.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jtzoejkp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xehkwhay.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dvvaampk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2varhxmwq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hkqsblwg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2civwhwwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yzdhdaja.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ewrcdamw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wtjtiehm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cabpirzc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vtgjzfus.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wuvsjmbq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2iiuqpywi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mgorjxtu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jjgebcrr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2yudcilyo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hrmbfrii.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wbtsnrqf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbpcprl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2luqqvukl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2eneadmcp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2poovpfvt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzvbnlj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fqsabjiq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zsrjhgxw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pygiycyz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbyzsrvq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqlwvoxo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yzwjbsco.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qvwwapsn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xlpneczy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pnvldqkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmuotgtv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2aafqmtvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdjiwizp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jbrhuawv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmruaam.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gcpjtpnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2basjsqte.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2svgivags.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhfhoupt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rjudgomr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2awdoucun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ymrowqnd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehkstwxw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2djqeqbor.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yuhtbanf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lhacoyxo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zknmkppa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvlyvgtk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kawvejhj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2izwhqahk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zneyboke.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hluexnrw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2exkuiema.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aguliwqw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2koiuifob.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vpgkcycs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2powypdfq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cxgmwrta.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vuueexbb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hnreblhm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sxoplmsb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fegqcywv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rozbrzuk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxnpuklc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhvaxlut.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yunroelk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mysbjcaz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mmavpzzk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mnriffwk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kwqrqsid.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yfhihael.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cahvyjqz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbwgpqar.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dalgkcyg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgdiqsyk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kekcdabp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tdxnezgo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2svkeokho.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2oihvsoex.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2koxqjqvj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2inpmatnf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mmiuvmqg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wdbuztlf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2aerdtrlc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2okodtprj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmvqfdsq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wekaonvx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2bpevavlm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2eomatroh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kggdfnfn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igrailfs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tddajuid.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2opzpzulj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hjazjpec.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rzqlqrqb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cuuzksiv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kvfdgkjp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mpczdpul.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gqjujknz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ztmrlfuk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tdoribag.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bhhlxnck.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2decfuiva.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2owtzzlzd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ynopbptw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xlupludx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rjiiihul.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xfqvjayq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2faiasxhi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tyxcptgt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lapcxnvr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2gupqcbdl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlxevvm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ioxdwxbe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2wthvxtbc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lhbdqzcg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zgdgxnws.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ndsfpzmz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fklgeuzm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2trrlwdxv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qlvbocag.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qjqqxupe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2woebvtxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrejodye.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2pvjrzugi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2curtvkvm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lulzerza.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gftvxfgv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fugheshd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bkyxrzfx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mepuaufs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wlodivap.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqvyizc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybbggvmu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fbiivran.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dinlqhgn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rohhlxnv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2syorotag.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqxhwxux.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zqvetugh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2squwpxvy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjnrhzql.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yvjfrmhh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2irqmcuzp.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2krepynyd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxswvrjx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rtlmhfpf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mggibrpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2tonhlaws.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2dudnxzkk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2pxtrhuvt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uvdzamhj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ohgwpabt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvinqxem.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gnfhpwsq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ufcukrrc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tpaxrxto.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uwtzbzkz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gidweyii.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kaicgvpw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lxwradew.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sjgbthkb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2kqygfyxu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2fmatbqxk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ifhthhqx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jclbmtmu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qauutxcm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2oytawkgn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyhnskp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkzhdw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vgoicycy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2oiplphxe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vwjfdpsd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yswjrpxp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2thqemubc.html


<!-- 参考信息 -->