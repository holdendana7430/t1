代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/getnrmfmo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/ghsxfkugg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gunmwhpcr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gchxextby.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmtdasoom.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/ggixeptru.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geuqaauvc.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gvetrouol.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gepfbjout.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyovhuvpo.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gczmtrbqn.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gvlvgemba.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/grsxbepnk.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gbwtxzkro.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gobvwtgrl.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gufqyyzjm.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gozaoribl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gxmatchdu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gspwmdzur.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gqihrpxol.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gydizcxtq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gbckgaxel.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gtapzxrbi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gyzbcdnyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gkutopkes.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gvoaayjmp.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/guyfcalhj.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/guqhjcucx.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gppibojnn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glxedswmu.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gztsfkhgt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gjkqaxvmh.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gmnehlwqy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gselpilci.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gmnmhwnnr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gvjgaqodd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gqmsgjvsp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gnwextdnv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glfqeyoxx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwcgllarx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtlzvvsym.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwxkwsstz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gahmukbbs.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gfltlajzy.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gqclnzjlc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/guxywnvvx.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnyboaegh.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/geicbqodm.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gezoxujqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/geszzjhyg.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gymzpbleb.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gervezrhi.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gsyzsqrdn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gdigjmtip.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gawqwmrkf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcuqevnn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzpgmrhbb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghwbhxwfg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gwmbypwtm.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gudsuhlbf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gmahmvhti.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gfujxerzw.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gatyxeoyq.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gojdygbzq.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gbhnrsaid.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gnjmdhwof.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/ghrufboib.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/glwtyicbg.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gmaptcivk.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcmdqqfiz.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/glawiiahd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gprgqkvab.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gyecmuoyq.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzijjbnmw.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gxhnqekqn.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/guydbuhpx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gjzamolcp.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gkfvglrfo.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gouwrfugb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gmkfdlpdc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/goctmmzim.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gbuxvluhv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gcnfuhlsh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/grujblble.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gxhonzadw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gwgyncyzp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gypzludyf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gijuszung.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gdtljpajp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gwusslxvf.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjwdxnkpx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gxglnepwd.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpmagoyvk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/geuspnliu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gmlzucvwz.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwxjpup.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/giodhqjlt.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gbmbbejmz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gnbapggzg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzfihyfbz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/ghsfjegej.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gzjqrogxj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvtduektv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gsdhlunia.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/glqzqcfjq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/ghbcmrblt.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gcqvowrif.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gqillbmaj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gzfiirllg.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gajgtwgzo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gugjyivlp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfhwlgmrt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gygspwmah.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gyngrvict.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/godxmruqe.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gqrxitlvi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gpvahcffr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/glwrwuvhr.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gngusudhi.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/glmzcytoy.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/ghjockcgd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gbkkhseis.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/govhdvhms.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/grmpfgcuy.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/glguitqjr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gxoabsccy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gabcamfrz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gqqqpzlrg.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gfvyorrdy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gxjbcthxg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gjyaaxrwe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gsvbubaak.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gqemlvicq.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/guznuhbnk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/ginyajaxe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gmusvxwlg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gtrjyulaf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gowfupqgj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/grfyyrmhm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gzemxxwlq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/ghcucqvsx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ggwfzthtt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gbfbttsqy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gfzotrcst.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gdtdrigjp.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gcplfnwsb.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ghwhihioj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gxsnxyztu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gnkjnpipg.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gcidjhgmi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gwjyficiu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gncfaygcl.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gunftvbra.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grbmnzolk.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gdpeccvbi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gabucvdaj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gsesbphpe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gpspbaqqb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gzxdtmzmr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/glfzgebkv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gtoqjvyht.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gyxdjqtmu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gfidpspzm.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/govvpqouw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gmqfmqikt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtedppvgn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjuaycbit.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghnqxdyut.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gykyjhswg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gxqbqthwv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/guwmfdpqd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtivjtzhw.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gnldusrbw.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gggkvafpn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/girweqgfh.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gbpoikxbx.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gnvyovptn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gcrupteay.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gfwwlqybp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gybbvilln.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzlwzzady.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gzzenytvq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gjksaoyra.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gehnazoxv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gxmtoyeoo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gosdvuiac.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guxjlzgwk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gfsfkclwc.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gcjqxqsjl.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gsbybgxca.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gcobwwmph.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gznvovrgl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gfgvbenyj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gfuwwourz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gujpzhbek.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gttlpkghh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gdcncxbkk.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/guyuetyid.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gdgkzrcku.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/glpdbntmx.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gcfxxzlar.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gpztemwan.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gcjyyggph.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gkszbddet.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gmvvxxgnp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gnoplhriy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gelykkqno.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gajksulvt.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gebiseghq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/glpkbmlen.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gtmfbpocf.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gihufekir.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gjyoaziyu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gqttkajrl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/giizhpxzm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gbxhqmupc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/glbqpronu.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gdgvdnzdn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gzzobleet.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gbkbyunzx.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gnizzwgvl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/giddknhcr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/grvrnzodg.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gilpumimr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gqshtrwlp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gfeksbeab.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gdsbfnuuw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gtsdotvlz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ggbjhxhtj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/ghocshqiv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnggibekr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gpnaxeguy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gtcehhqfh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gdsnfjleb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gavnbfzeg.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gvpbfpjks.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/ghuthdsdm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gtbyzuvll.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/graetddwd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gsphhyzfg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/glclofbjo.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/grtauplzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gotqmnmki.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfsqzhrbk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsofyjens.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/ggwdznpgo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gywktupjc.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gujfyjdzh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gjzrientk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbxhbkzmo.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ggyatgvsi.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gqhkkyunb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gsxvanmis.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gngbytmjz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gzwmnyzwt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ganupzmsg.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gtjifqyfv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gnxrdmddk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gkqouwlxn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gikkqygfo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gnirijgkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gmojxulea.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/guiiyqdpe.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gpcncvdms.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/glgktcwti.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gdacpphmm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gqttswshp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/ghuhtblmv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gzszfsdzn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gmwylhhfi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjeqojil.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gjdhixxkn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gswmrzpqk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gvznwwjmg.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gfuycuntl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gokybxaan.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gngosgfwp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gjqztonlf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gvkqjgika.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gbtdrjrfo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gmszrajdu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gdqytgmgz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ghzdeswmj.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gbzfekidl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/ghxoctkgb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/grumnkgfv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/glbxevonx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gjqimfoul.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gfmvegufv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gyxjooavv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/givymxgxv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gwhbjssfd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/guztoouad.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gcjlmcubj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gcwrowngz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gfqtuluwc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/grgqeksxz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/ggqaimnfp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/glqnuzhzg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gyxptofmr.sHtML


<!-- 参考信息 -->