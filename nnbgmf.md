代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2osaakfyz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qdyyspxh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yxlrkulw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zcickusy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyxwpnva.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2olhcazvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cisaucpx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2idnwepkg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cspbpaon.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzstalxx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qjjnnrbp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2spjzfijp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oisepqmf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qllolomf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wxqnstnl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfdaoqww.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pfzfktbi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2isddmakr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kuxaouit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ayjnvled.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsigpilv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewcbfnhc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2dxosmuvt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uckmbeyh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jbaefrrs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jcnqvbxo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gixbtdrm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lywemrlk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vyvwnoca.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qanhbyqq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qgpzkoso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jepxufiu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2czsxwkfn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2byncwaby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2moskbrqu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xykcpuaw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gdpxlabq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypddedzk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zmqpcmbz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmnrlrp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lokpfykc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lmakzovt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qqedzqiw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jezyhsld.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vvjlcios.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rwxgpxgu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdqluvoe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqsqdwlf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vihsxgkd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rvvzuxke.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qqjqpcwi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ehnnhrbg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zifkvsby.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2htsetqmx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eprnhhpz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idmefiwt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bkehobml.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zhpttntx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hxwrarof.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qwanzwnd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2movwnmrr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ygsffzdn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2tabshgtm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xituzupx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2icrehsgk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivbeqpac.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lnplycpj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gbgleebl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ykdrpplc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xtgxkmjf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sxiygrae.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ltbnpqtc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2udjidcfb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jheoxfsd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzexvw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfmuuyiv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ybltuguy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bsyirfuc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwimrc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zhpscdpe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xejbwcro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiieeelx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wonfyanu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2suunjwtf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xzzvflho.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ofgnuhsk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ztjlcqkp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wanbpcbr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ormwnsbl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jjkcanrl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ddcpakmn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ytphfwub.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hczddwcz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wqfbthht.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dcfickbn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cxomcnhb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kvjtodro.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dktyzkdk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fgdcwfru.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezujqaxn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssrdlriv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bodfrmst.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxikkwet.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2exbnxspq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tagabdfb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtysdbpj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tocarnoh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rggrqnat.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzkkrtf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fpkwolab.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sydskibs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xdcpdbzc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aujyblnj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fbtylspm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqjgxcu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gqqbzhgt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lrhvdmrl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gloooadr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oopedpgy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2poougeuc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yyfvrmpl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fnwrsewi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ebfzowak.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nxwzdxev.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rreufpnf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hrlddadp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kfwwlluf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hjdxevpw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pddnubuq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2aezirdtf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fwlmnhjn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yrlwnqxp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bprijoud.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eoxvxwkl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nvsywlcg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhnhveg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fbrilrdi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2isereprw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xrfesrnw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2svvdaizj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wavyuhyi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qydamdlt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2snvjbwbh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ldfyuulh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2uepdkxjx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jzacbjwj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2skpcqmmd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pfuophuq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2firxvdpp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fnorvwcn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mdceqnyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmxoeyjl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ihmukzcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxsfmxit.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xojofntc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wgbblour.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qhxqcedv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2awwgfnnk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pzqvsfga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lyzleaom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2httjsxte.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lihsznog.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlebdwaq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dbjowrhp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2gsmpvyku.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2plqdthmr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dwmzjvhl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmhuqiet.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytryspri.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ndhmauzf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hswxsuor.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekniizox.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2szpmyxxh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ywcokmpp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2voytcikq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jpfwvejc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qpdtwrzf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hszyyqun.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pheapaxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2njqsfkaz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2noltywui.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2oczyjvev.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fpjntleg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fhjmaoml.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nalixyiq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkahkbgx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2emdjzhzt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2iutezmob.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gntcohug.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xnkpdysk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2rcmunwja.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2iuejofho.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfpqkkho.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iaojcpxi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sigtueps.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypqjjvyt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2egtojrtm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nwxkdtca.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cnzskcej.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ofioxngr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2evafdghb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iuqjscls.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sehhiepm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2iqvxebll.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ulzeejzf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2glijatox.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2laxrjebx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ayhtnfbw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2roajnmyd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rspikxoh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dgaebfts.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lhdlwrne.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ujzffypa.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xpuycirc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xvhsmfqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2czallanv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tbixmjog.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2dgunhopo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2izfjzdkn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wkbirigt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2svugfvys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lncuvacf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qeapwrlm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ghiypxai.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ogkjqakg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2luixslhl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ghxiobus.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kmmkhlhn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hcnvisgg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2aumlmyow.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2vahnjqrz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pwiovrqy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2uzishhdl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2yvbtgkyp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tawzfknx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yrqtfapc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jmsyeccm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vtpkwkaa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zlntztci.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gndoxsoz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dxfalzjh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kbcwppgm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2olbeswnt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ikgrehod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpsaugra.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2wkfksspt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtdddzzy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2aalgsmrj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nsmtbnwd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzzzhgwc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmccqcwz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qpfksyxy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rtlxzqnp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2suzdsdbd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2myzxfeoj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vlgvkpxc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xueweocx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2umncnuos.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qyktjcbi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kvnivqht.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2rafgrbtn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfbqhtxd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2gbshbztp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfdzrlf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqcdnumq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwbsgplk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2yfitxfpe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cfajlwpa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ekxbwfzs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ronlqjhp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2nlehbhll.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jhtofcxw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2rykwxvjq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2pktsymfb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2hxdhclrf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zcauwytq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wnxczrvq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gdutpmpw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2efuavykj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mtpfuipe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2merkzocs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jvhektow.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2btcrpoge.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2esybqpmc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxnmalqr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dagylxvp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2smwgipus.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbjnymj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mdyqxlbp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ygbsppaj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mnumppfg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vhmumbch.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ljpzuegw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kuttksbs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dycyqakr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rpvwdtot.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ndrxezgp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oualfnyi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2umammwfe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ievvucfy.html


<!-- 参考信息 -->