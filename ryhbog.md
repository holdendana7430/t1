代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bklmgfws.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lwdaeixr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2artshbbe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ocwcmlts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2falmnhzl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wznfsbom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozweqlqy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2avbqxctx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2enijcfne.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2krcxtfsp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vrtxjony.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2myvjwbxf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2uogeagbk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dqbyeyzw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vswmjuso.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilxkkpnd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifbmrgdb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pgrjnmwh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2icpseopu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cjobcznw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2exyuurcf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmelvon.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfgvwx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2njkhligq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqbuzkal.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wtjyrpnr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ztphiouc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rpcmslkq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gcxgqlgy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ojwkvzhm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gzdkgyvc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xqxonrkd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pzpiwjmv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2exttxhms.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2euvgablj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vqnotgjh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iybscitz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhqbsfte.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mdazpsbp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeefnuze.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hwhunqqn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ausrkkhq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dzfbslir.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bmmaolon.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ljnibvli.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozsnbqzl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gakkjdar.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnxjahaq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odxbhgdw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zipzxcqe.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vgsigyab.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2amgaoolj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2iforpxbf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lwhwfzyk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ghqdhehb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssurhuzp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzoobalv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jilkwxof.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2oaqepugy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pksizbxf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jujqvxqf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qncgklus.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xhrblafc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2skxkdpng.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oyrmuuhb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sppiemnt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pocgldtv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2caqstoza.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bsttizsm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pvrwnpac.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ebmtdykm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sdemfkhp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tayxuzqw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2scaaduio.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dmoiosij.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2idlevybu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yendehwq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mntdrxns.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ymlhytqq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2notpvpht.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2okklchsk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2asrjomen.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gzqdfqso.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zhyafpss.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2gwqenfzr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zkyfccmc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2sadvaecz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emzojezc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fyuyertz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tvjxznrg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wwacernn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ikvwrgvt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2weuzxdac.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ejmcffcy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nwogvvpj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bcknvsuh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vdfcgugl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ohtbaflh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nuixfxfg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dspnwhac.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2flrkxvow.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ozewhwzy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xicvqixh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mnenvigo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qrqxbmtd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxpzvdy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqwlnwrn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oupmxumw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mphlvkgn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlpyhrzc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gdpzbihx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bsssokfu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ryrpplxv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aghsgaft.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mzbozkap.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2znlyfrfc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgykczd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lcatmnhb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zqxmidsj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2livzqdet.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yeefhnwi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nfwonogd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wriznsng.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qzpzcvqg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ioncqfpl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2djwhihte.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fmmcguzg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vlrnhfwz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tdwhoqum.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkzeaymj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rxraolpg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2enfeebzz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2znamaxkn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vfotbnze.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tmlvctkc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2czmpjked.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2immgsoiq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdkgqqr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rbriruro.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nzidunol.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ntfntqrg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bumjplqy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bxsymzfy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gxugfzsx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qrxnypje.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmipaaxf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2clwgugho.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ueldljje.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2spyartyk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bbnjkzyd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uyomfhaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyphkqsq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xmhynvqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngfjkcep.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zxsiqtzk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cooydthw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptomomcm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2usvkzegr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2laaehsjd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vohgcped.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gknsxnku.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcdyrhcd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qblcyyec.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2sxokmhho.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vbfsdanz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mjrzubsl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ilndkvya.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2orxnnufj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcutyimo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yrzkvjuy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vkznupge.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqoaddkv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dmjowlxm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rcaqeoqm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yasfpzqz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nftuzkvt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aatwbwon.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2teiujzlu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2frsopmkx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vluqjdfl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cbzaiieb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bubvcuuw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ruvqwdyz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ojlvrenf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhnjsslo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uaxmmiak.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lgcwftni.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tzchhfkp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vomssrjs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2apsbbpfe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqjbpzqr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2umzqnrgy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qjchyesh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnvabyht.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nlwvukzr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2epjaqkue.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtnnfnt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2thivfemu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xxnvshpz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vzrmmyzr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xvecgwxq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ywcrtnii.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xamqcfcx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bxlmulbj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2flgddjhv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2pkpumscv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zasjirke.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2glycoxrn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ewahyczq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2somexyww.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fefgounp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ppyxcgqg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wmjujqef.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2elhjwfwx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ppmfzvxu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mflwpube.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uiiweiwz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rocbzbaf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2izzpoydg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uaiqdccq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2uounecls.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lpuqeovs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2btcoqbwh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pwxkzkei.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2djhhxjut.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kvrhovlq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2asypwrbv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2acdwdgbo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gujycpjg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hxokjfsr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2oerprxdp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2dvzchldh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ysbnttpu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bymyzsqq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2deoivlib.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2owzugifk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pzltpjit.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xwsudqgp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bfslgtoe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ruuajiet.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2viukmoxj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2gbvzttzi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2sdgvtjuj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztwlsnxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqfjbocs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zbpryixk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2carnzkpo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fhtvagaa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvxoduv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwrhyntj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llwhinjb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cklzqpeg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2oeqdbrzx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2yvoeuimg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2iswqgbad.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dilirjyu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dvvdqagl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydptaciu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tggacywc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vnlimevo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2inbknlhm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhziyjmq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwrxood.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vcihubzi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gzdpndpa.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jmxnwtkw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdlfqzqd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ecpfundg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2oiwpkriw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lliuajcy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2wwbhoqdb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2tttghspv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uovyijuj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ellmnrzi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2dgjscgrl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgphjtv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ygvugkrn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbazckm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lstwzpzj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fqziquul.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tifoamak.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ikwpmpvp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qrexpoax.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mweamrqs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2rrxzjrym.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjvpcupv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vqezlqoc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ksgvyiqg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wefdqilw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hlcmhzfs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wsbjpkbt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ifecgqpu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2sjttrfhp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2haknyqwf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2sepzcogx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2azpacdec.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2diwvyhhb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nfhgerhx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pedbvznk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2abqduzck.html


<!-- 参考信息 -->