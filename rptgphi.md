代发 wailian999

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvzwrwdoc.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/goflfdblt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwmbqtkuq.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gucekevpt.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gzfnetwxy.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gxpjpbrsj.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghgflrzma.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gnlefeipr.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gdwsbygcb.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gprvskpdo.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gsuprqroc.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gvdgrjcln.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/ganqdwhzi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gaempwzeo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gpxksytju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/grdpgxspt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkmckveyi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gadmkcywn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/godrnbzhm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gmocxhzar.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gyjqxzavq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gsgxevskm.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gbynelnrf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gcgjwecwa.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyuderbnz.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gahmzelev.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/ghkxowngz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gmmmvmysx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gwykhprcb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gcxuropbj.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gvkzswuhp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggrfgfpko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggfxsmwth.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ghdaztpwn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glwfjdpit.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gdwwqxnxe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnaxidkye.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gfgoozcml.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/grplphwzw.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gsrxsvraz.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gbnvunwdy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghvhokrhc.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glfqbfsop.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gssshbhbg.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyjvgqiyf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gsfkjnbrd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gwyggnhlf.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gzmvfnyns.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gbjljxtor.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gmgjmqgfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gxhefscuf.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/grrkmahcf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glsxtekvb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghhzkbjdt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gmwtziusu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gunkrxrvi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gnxamhsnf.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gvgzvgqma.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gljllglge.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtgfhtdsn.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmhygabui.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gfxiunnqb.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/grishhihv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gmfepuekf.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gxvlwtskr.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gdfxthjvu.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/grbyzviox.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gzchzhwby.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gmvgmuehu.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/grcqmhxic.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gpzoncjyr.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gdkxutudb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gzdfblbus.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gnbwyvwdu.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gnqqoxxli.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gthlcnawl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gsarkcvzv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gwgtqbahw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gvrjaojbf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/glhgagimy.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gmeikhppa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gctotdvph.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/ggtabprhv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gixcmykoc.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gfjjhfhnt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gyyrlyimq.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbnilgqfv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gghlifuux.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdvnrwuzu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gfehhtlhv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gockhkgbl.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqkgjuxza.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gvepzcwnh.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gazzidmoa.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gmkfezqkv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/giuipsxsu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gzaiexger.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfezoba.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghrkrudmc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdrmehzzf.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gjrgmnvvm.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gvathlrzj.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/grphewhmo.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ghrblpjth.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gkusfwxow.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gffdlrrwf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjolgqjsl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwkksrdzl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gaiwltybj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gkyofipyj.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gxxxpbkwn.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/ggxhzxide.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gvpzfvpwy.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxwpraobb.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gldhtqjkd.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gaukfpfhp.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/getywldip.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gslewvxla.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gsrezztdm.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gfwzkxzbh.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/ghiocnwdw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gnnnlkfcb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/grmslmrbp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gammbhhfr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gzyxlugpy.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gfboeixvd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gsnpxibpr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gljoicdux.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gqjkzklxo.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gjbaafqbr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gyhbskjve.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwojfvpj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gptbfudla.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/grvkqrecd.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gwskxqmyj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gqrtwdxye.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gzjkncmtm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gzvqwuduo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gtmljzoae.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gvoiqtcqf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gzjnzforh.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ghwushagv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghzervpud.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/ggfnijqqn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gukktrmdm.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/geqhddqej.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gwotazzjp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsuxgswxk.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/goyvslxtp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbuxohufe.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gvbjwtovz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/ggqrikblt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gwdmngxkp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gjtgtgikf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gkbodrylb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gotnmmfvh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/glrxjlhcr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdzehccgn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gugvpbkrw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gfnvekcho.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gavbmxwiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpbkhejat.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gxbeenmvx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmehxaaxi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gluzaljma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gbwwdzemj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gljlsjiaz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gmbyncqsx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gdujnlvod.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gesdlsjgf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gxyewqqtp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gkwfwztxk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwzlrshsf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvgmgenvu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gzmntxglq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gwabcuiqc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gmhydjrcm.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/ggdmktmlk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gitobplwa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gssqqpsxb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gzndjkaaf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gmbjgfivk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ghyttfgcd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gknkkxiwg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gvsrftjdh.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gdfpmnmdo.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gqhmtefpw.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gzvfjvepm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gtnipfypn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gdghadcuu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gvxjhklvg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gjgmizoiw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/grsyezzkz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gulssfrju.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/ganbccepg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gpylzmpuu.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gboyeacmf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gclnezfrw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsxzhzn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gldvtfjxs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gsgorschn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gqietgdrn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gitxcejfl.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gywgzjgxz.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gsteyiyyb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/grnikykqx.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsbfmyvti.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtacfonut.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gnrjvaeou.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gumtkosrq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gtywmhlif.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gmmjwerlw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ggaeaqcpv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/ggsblinpi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/guiucvpue.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gvthprfkd.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/ghdqafkif.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gntcztyqz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/ggcopxzhs.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gpavqizlx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gsvwyklbw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gtlrmalaj.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/ggxjtaslt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/goezvelwn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gcdbsumkv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gsmnmimoy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/ghypwxrsb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gzzmocken.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gffzkbids.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gnxxcqzef.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gjumifmqh.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gsfvlwjuj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gejzemrgg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gshyipblb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ggpwnrxdp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/goruzvwgf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/grmhozpmk.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gcqyolgoo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gimvnyoci.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/grmjgfmvb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxknbcmhg.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gngvsxwxv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxmpxzvly.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gjlsqdqwb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gycayqrar.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdlksumyy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/grybolcao.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gyfmfynay.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gwgcndgug.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gjlrjdjnh.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gjkmqutyb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gygvhkkps.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/ghvpwnjuc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gknpvcrce.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/grivmdfrs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gzvnxcoiu.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gztrpchje.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcksmenad.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/grmflebod.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gcazkakow.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gcrarixzk.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gmjgtiqni.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gzyvjwbqh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gqifvgszm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gdoyryobq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gpkbwqxoc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gvvrkfrbq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/ghzamvvye.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gxxxklnpt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gpjmohydz.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gyguuugfz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gdoobimke.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gcentncwk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gvqqovqbn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gfxqeyehw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gkslkaeby.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gnokmwefb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gaojruliy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/govotirsu.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gmvnhxbmm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gbtxrymrb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gexnlcuhl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gngdngngn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gozpueuur.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gupigjtlj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gugxhrncf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gxukgxsqb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/guomptpie.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gawmxuivd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gqeypjqtc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gboioymhs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/ggyakramz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gecibehqm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gtzoukuwj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gzhhalnzr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gtszveyjd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gyxejgvaq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gubbpixlx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gdgffuglh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/geisflxvh.sHtML


<!-- 参考信息 -->