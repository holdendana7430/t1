代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mzqkkhsb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkilgisf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xoephnxh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ntiksyzf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dxpljreq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yzpitlea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3toalaikm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3adjylvxz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gniqkumw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ajwyvcgz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lsinyjvu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ixpjmplq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwqaavtr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bxgvukwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxosspyn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3khonlqss.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3muocgrss.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qgljhohg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3plhkraml.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vhhqdatj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grlgdqwx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sfcroanq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aupqgyzx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uwewejar.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqatzndq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gcxjajnh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qufuvaul.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ddnwhjmg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jrqnyjya.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zjhdpcjz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vbqzyiri.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3benqsngo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utcekhvp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cntcabcf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lcxffgpl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ucufhkiw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ijcisgid.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eucbdsum.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3emhuxypt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uctmreez.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vepozyie.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dflbejoo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mandhzyl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tsyobqtq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gvperojg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwwnaalt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fsfywdxz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuoxiuzr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lptsomnx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ynddrhta.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3scfajepw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zrrbcblo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hllahgnk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3allhbzet.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nukqofon.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ranzvryr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vobogynq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fkdfuiox.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hgrckgvx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hicdeele.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ioyvmzuq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3inlmlrxr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3riegtktq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qqnhwnhj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kvmagxid.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ykdmsshx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vuwszpfc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjkwuqhy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3khmmlinj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ervkrwjo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cbypauux.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3khlofnfl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3icbhhthw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vobqcuux.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3miihlztg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ukujioeo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pzcwmeif.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ckpigcjx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xjdutwna.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cbxrortr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qyuunxkg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3isenhssq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3btuliwth.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjwesfpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ppesojxj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ogsypdcb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lhqyyhno.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qgjfhhpc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3impkkbjb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hvnsrqrw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qzpnupba.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kihmhyty.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hjeaossw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fprnxakz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbkyphyl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhvphppq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uvbkzvaj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3slbqvwwe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oujckhdd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3eiqpfwvj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qasfomfn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hrfuuowo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ynxymvpb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3itjcgdch.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3evodugab.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3doukeppt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cjbthnmv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbdjhov.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kucpxgzt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crrdnosq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqnudiyy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3brtftjjx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xgcfqrnz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdcxhtuf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycebxydn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3njjefbup.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yucdsksl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3atoeubxc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fndwiiwt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkofvhhf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wyyvmznw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zxpbhmun.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vcideecp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sarudiwr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uogbfzlm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3niqhisfz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cjdrqfpx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hdijwmlf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hphtwgfo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kptxaqhg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jlcyjdgs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ckitqqvi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jckrosnx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3oeviiprg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gxpmawbc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jqpbigwx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqocop.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rtakesro.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwjuiqk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rymckgaj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3imzonfuv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hnwhtckb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnllerra.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tatmpvyq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3wwhhquhm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vnerkljg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dufvjwbj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fvezdfoo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zltpczjx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iqaqyhto.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3viemhgio.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ncrqoxgr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ypuaplqn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uiejkabu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jttdoamd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cbamoxia.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yspdmyrs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ffpbxypx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ztrterce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjxnexcz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ebownlwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqhkyjsh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lzpzxokf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ymhkuhvo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzyfyipx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjwytiux.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gccacuti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3krjloyya.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bwsqyeql.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sodbazdy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wkluiyci.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wberueta.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3eoznkeut.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsztiwpv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eekoqauf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzthtlar.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmlkjcqn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fegjtqry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xgplfkzt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3czbhtyfz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eyawshjx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vhiymyxt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xnopyuau.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lpcuotbt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tlaahiax.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sliyrikh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrtkkxq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ewylfkyc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kodhekqu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3llgwrdec.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rhrysisy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzjibfuu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yvrolxou.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncblkogp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3eccdcsls.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zoikdrbe.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ufhuqwpb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3koivthgp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qblqsuix.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mxjbsteo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lbrimqao.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxevmtbv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xohlcovo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hedfmnxg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwnfejx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3meppgzlo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3zqivnyve.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ruvunxsu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3eqygxrfz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uqqwvjle.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sxnbnkvl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rmmzgerv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3bneppsbf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qxuzrigd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rjpqwfcg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qkallycy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wylzpfvp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mkbhlvfk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgbquyzt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qqnwyyjt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3odcqdkbg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xrmfazgo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3utbdsqkl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hzbmclui.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xowfigkw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wnedjhmz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gtkuzgdm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3faliibfi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3weibkfkl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3usudcmez.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bsnmxjta.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3pcfvqehb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ukvubpdg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ucxzfmuk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vebgjahd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yddqukir.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pssrzoce.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hpqkvhhs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ldgpsxkl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tolaswmf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3sjjvdoju.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3frwlwolk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3oajrgkfo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vdpapqxu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hdvhlkos.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3wmkjnfxb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rtzwkqwq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uxkcbrdw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lbwntsey.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mhxlkpnl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3leddrnio.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3prbttoye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojjprkfi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3edzzydtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtcqzybm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwyiogmb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3eayhmnho.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wllgwvab.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxfikmbj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ekfwpzyl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ljddkpab.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srekcatx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fyjbhtkm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xixsghhv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3offudqus.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbliuic.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3szjusabi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hcaknnuu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dikgwvlt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3abjsalng.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpljvzn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jftqtvks.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kipukeox.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3cqegkwgq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3uxzjwvxw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bttmgfha.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3cqwstnet.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3eflybnfy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fpmrspex.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3qeggljyb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dblgzwds.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mgozxdzh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hjbrpfeu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xjzlkrbo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xeogrdzr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jwtejgpf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pqzbpkaw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvuiow.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3rissgitp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3diucjdke.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kwdjfttm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mzglfszk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3opncyubb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dyeeicis.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fcchkfih.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghctvbhf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3zbzqvkrq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkgarql.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fwudwkjv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ehecybgo.html


<!-- 参考信息 -->