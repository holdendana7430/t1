代发 wailian999

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gbjhvrfdz.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gvzzionjb.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gzubaoayo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gzcfishns.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gasabgqyz.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/geulcdiif.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gswrfjnfp.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvzqhmska.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwqdopylg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/grrjawmhg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gonynrklf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ggaclmcqd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gagbkizcy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gfqvrrdez.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gryfnohbt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghguauvxu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gpniubkre.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gvvtscvzj.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzktdchpc.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gadgmgqsa.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gfntupznv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gnmubwlvt.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gmkoeyaou.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/glbgunfrp.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gpzifarsc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/ggiueoezl.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gctkqqwme.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/grycegdbm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbctellhs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gcoylgcuq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxlevyhbn.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/golbgimsy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/grfvfxmht.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggyjncdjm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gxsgstuzr.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gfripchzc.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/glygsbgnp.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggdkempoh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpnpikncd.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbgrtjhmg.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtkgbgcge.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gwwusndfn.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gscixheiv.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gfuiztdia.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gnrmiokzo.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gvgrzepsr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghkluufum.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbpbibmus.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpdrlyoef.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/giqutwfcl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gzmvxylza.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gwyzqplhs.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gsztrjlde.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gcenhzhpq.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gstljcewp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjxgoyrex.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqguhwbcq.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyrhueked.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcskxuhmb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gijfmwnpz.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gdvqwouxs.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/glgekhufb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gqjskrsig.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gavxlwjfi.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/govbcuupb.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/ggeadmqmq.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gbyxjwbna.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gceioikki.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gowiwqmmx.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/grtqunrcg.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gtztjleuq.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gdkegnmzw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gsotnblua.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gkbzwxhzx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gxtwfwkmj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gnrtfzeaq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gmopplhij.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gseevgfbp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gzskbthts.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gorchnjjb.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gqljyipki.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gqetyxizk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmhafwezf.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gptatacmr.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gufmyxpyh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gskhyxpyf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gkxfwicfz.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gydtuvhph.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gmgwpknmp.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gcjhwgrla.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/ghtzcilnf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gzetopzcw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gjffjbjrg.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gocpngqcz.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcgiayorp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gupwkufyk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gazvrjovs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gfhdbiycb.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/ggvicqblr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gfeqgygqa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gdbeotsfi.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gftqaksbn.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbkurequu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmqsjinfv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gcvmniagh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gqesjrzhu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gkgzjdldh.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gmubgbrzv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gdqeqmwfi.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ghmghhjmt.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdlzjkwpr.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvkbwvzca.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqfqpsoex.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/guajihkie.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/goxemclvn.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gkrqyoapr.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gabmrkyxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gsjkzioew.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gcwscnjgf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gmpgqzvab.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gcrvamcpu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gmpmwnvyv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gwbcfguin.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gdzafzdxi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gbomvpxhn.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/ghhauzvoy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gogimjzwz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gwzbupssw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/ghniuhgnm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvunpfapg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gkxgfsint.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gwhykntde.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gxhljnlqo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmwnogpmw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gsoydoiol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gjtndimzj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gmgpbdrgv.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gnzommotw.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghsskvlot.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gujzyzxxg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/guckuthul.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gvhgpjwrx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/ggdibletw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gambwggvb.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gtulacwhg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geepcwkgr.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gvtklwsex.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gloatvuxe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gbsbnrigb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxmygrkaa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gveesmqdu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gytjuztov.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gpqppdpqn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/grpqtdote.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gmrozgoah.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnohwtm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gtroagxch.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gabdnoruv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gkvfxtane.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glzlzfwdy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmufvqmen.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gexawwfwd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gewskzbvo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gykocjgay.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gipcxichs.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gzdzuvfpi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ghfgxbttr.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfqpmsstq.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gywmdfpzl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grfizpbxu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/grcjvfhaq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gvhxcpigg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbsxcxdvo.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gndktydln.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gwzqkbmre.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gvmuofkvc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gpudqwmkl.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gnlgepeho.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/givhnolxn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gwlljybfr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkgpofo.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gglpuspox.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gprfgaghb.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/glivudxrm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gtlgmabhc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gdvqtyaor.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/ginddmoyh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/glkrkyxbu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gruiyrhky.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gtrzisyna.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gejmwyclo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/goltyilfa.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gtkoeahxc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/glxpwywna.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gxufkjmlo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gmbobjnta.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/ggukmqchp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gpztgevrq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gefignvdf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gvknfowrl.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gqvgaxjlz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gjjzciifd.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqiadfrao.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfmddffoz.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/geqtdxsmt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gdkstnola.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gfdlzzhvm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gmsnnikva.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gtbmtwakb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gngomuerg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gtpmwnzzp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gtfsmpelr.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gvimimsbc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gvmblqvbv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gkdilfzok.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gvqclmmjd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gsnqkizan.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gdtpntqat.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/glmfwgwan.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gcrtrgyqb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gntvtqcoe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gxadtznnc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/grcaglxeq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gcjlckpdv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gphbqewjt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gkvironyd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gqtgfmbty.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gyinqwiyx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gqjsuxanb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gixilardg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/guqjvtyqg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gumaiewec.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/guhmlctjx.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gdafulvbj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gcvekyqwa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvionsfii.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtfratazb.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/grzweztob.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glzokngjp.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gbzqbhfta.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gkpriwyep.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/giqsipgiv.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/giscdbyty.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/ghjueptvw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/glpslsusv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gaewpsizw.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gwrylsiqy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/grsgqifmy.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdiwvnxzn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gnacbyatn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/ghlxhwxfh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gnhukpkde.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gvsuwfavv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gkrfyhafr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gwvwoxlbo.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gzgdekxmi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/geilrwskf.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gbjronmxr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/ghtpkmzjd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gxpyofmom.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gevwdusmp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gdspgnveb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gzzbravho.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gemirrqfh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gqxkueshd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gbmtyhmhi.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gmigqphhj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/grigakfzg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gnflfcdli.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/grkwgsdmb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/guhnarmmp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gzmtvpjfo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gammbtmlw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gxyqmxvxm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/ghbymcalx.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gletmuxjf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gqedoxoef.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gtirovmgz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gxehqqrvo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ggeycvzkb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gnycwigvm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/geyytkmmn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gebkugurg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/goziqmvkx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gnjxnjssw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gkorsitty.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gmjssthun.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gzejwjhsr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gzbnsmyet.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/glswfemgu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gjkxcikmn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gwmhcntcv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gwpbvaqxb.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/ghyxcffkv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gwcocrnot.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gofgediuv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gjrcumwdr.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gbmzdfyqz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gedwyludk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gfyhjohkb.sHtML


<!-- 参考信息 -->