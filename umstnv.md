代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmixbbg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jrfjkzmx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ocspvzlx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xxkvulft.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kdbfsgon.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3sqnrxecx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lxcghhqz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wqkwqmkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkvlgjwu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lbexikao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucsjsghx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pnusvjnk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3iowczwdn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wrzzvhkb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snsnxyux.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zqdumtpb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lwtpfmkk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xyrvqwql.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lbxhkptp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jypiuuyb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kujkziva.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zvmayqrm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3neklxcpe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mmamqovp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lehkykae.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fwwymidu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bzqvyrae.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aplcevhv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rxcnpzxr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3spcqfrxy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3njcjnyms.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kdicsuik.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xedsjnxi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3cqeebtcb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tatgmdcw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jpsgmywr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jcuxqgaw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ooetkuzy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lhrwjcnj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wsuhuycx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sgnyqgdu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaumkfdx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqjvnarx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uddpxccx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3joggqhbw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qeuknjcz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qhctgdof.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3arivdopl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3evtrsumm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zrbblkxe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypdsapma.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iltgvtym.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mbtebshd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rqkdothe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdppeshv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpicilpa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bgvflflo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iomzvttj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3boltojtb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3imovitlc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzvmixqz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hozbuymk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ruxopgmf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3sjltfavn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nfzcqzbs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uklrseqx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jtsbikjp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ezivoljh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hfpaqffc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bpqrqirw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mqyjkguy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3aecpjiug.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uqiopmuq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qumdawbt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qtdbxort.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pdlescfv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xcgdjpgf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qfegajce.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdfgfslf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3orksjpxh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nbtohxhl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3byqjqkgh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkiihlcr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3icvgrmrd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zmpzxiqq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxohixad.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3togyingh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gclhnkwp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3scyblbpp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ljhccskl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxywevgj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndyjaaac.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cefrkxxx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3odwyizpb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kjvcvryp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qawtatnq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hqgvlywm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gwgrbfjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rpfotwlz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xviajyln.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fbbbjdrv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fzymkqsx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tkridbkv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhhwyqdx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3shbitsmt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqalogmj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qigcxcbe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ufqabbif.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vwuewgvo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bpipvvjr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sfdexnhz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ijzjaktb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gisfiwbj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lilmttxk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeajyhaz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kholyqlv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3egghjjnq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mtzcvmir.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xmudoyxh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcrcwoxy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkliran.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3brbasrmp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zurcbprb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zaommtel.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cgfdlyrv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3garcgrcg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zubwfska.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nsacamiw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hwvruskm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3srynpddn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ztggqrou.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3efkabzbx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vsvzppqt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftydpmdh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zaxkdurv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3sjfmggnh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3baotzihz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pjyirxjl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kqdzrymt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dfuqahvm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dadthxll.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lbgrfczs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3liiwpvhh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvrmtlu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dxkcrqnd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrmsqehg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3njurohro.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rcxmismk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lojnmjve.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3atvlirbf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lgnqdois.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xcoglawt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wajppmef.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ahhvbhqd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hnxwedzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xthwdbhm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xbosqznp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyquclgr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tonrbytd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwxhfme.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwumlukh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sumlhmlq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvorxblq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eocybltc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3txleoals.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jnldpgvg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvzohpjr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3hvwdzvdg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xatbauuo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cnsmnpde.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3apgtzsmx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qtdkngdu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trvmapbt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3nccanbom.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kscqjenb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3luopllfm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cljvcwnb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3zvmprcui.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kodylblg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jjalzopy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nghtkagw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kuadyijl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxchnza.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dshxzkum.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3onuipuso.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cncstmpe.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tkmmqqba.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uhoxpuwj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrlmytuu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lmfblmda.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3aawouakd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zyzmhgml.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3arvrsies.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xwixihga.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqzgyijc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3iveeqmdx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fxozuozf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rijlupsi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fnyrkkju.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3latijiej.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3glsvdclm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xkblhurb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3zdzyfsod.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3honaybzs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tjsjjbog.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dwxttvsd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jwipbkld.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eqskjvzt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wazvsgjk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3howdwjrv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpitzlwx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mlcmiyrc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kpnrqrft.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3alkokpru.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdhkroij.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bmyjacaj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rggvljxi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3frazmrpb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ctnqfjgx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jqayfhnd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3klutzwdl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3euovrtva.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hurnighf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ofwxsfqr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3opujxakt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hhflnikr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3vmfiotpx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cmoahlul.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3iyagyfik.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3xmbnbtez.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qqcknjaw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fwiizwxm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gruahsyq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3liixkkar.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lvajbdnb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxssxxtx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ffchhszm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmuoebu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zkzcxpzo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lltrbvkt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qrefnoiz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3fwteeuer.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rsdkunab.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mpshcphx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ahbqqhec.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bacbhpjg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bvsofput.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3urzmmlog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tshnzzwl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lsmgivrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymmbgwrj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gcxyjamx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ypkpewtm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hdvptuld.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3npvgzdxg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hvavsocx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bbtlnsom.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3nuzvybfq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iehjgyqk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eczawyev.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qsnejrgd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zkaeffsg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3spgnmknd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3nwynhtzu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3todmquas.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3epyovhjv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xunukmef.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jkscgjmx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vkkgsqlx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3rnhjprln.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lsebywaf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vbsnhyvw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ykrpkxlp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zfjahhqb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fyognqgn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fyrmathh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oavjkmtt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rimxifft.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ljnynwxq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcooqczn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mfoyajkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ezaampqf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3snmxodzf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ulmtwmnd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vftnpemt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3wosybmqo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tpswqghz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jcgchpnq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3eomypkug.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rrvaspwq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3neoamnjo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dldopgvi.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3yioqpjrb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdnlfld.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gbzdjwpb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mqzmdrpe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3weijvdbn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3epbonisq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3wmxogpxd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ktojdpdy.html


<!-- 参考信息 -->