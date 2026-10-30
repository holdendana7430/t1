代发 wailian999

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gjbbwaesn.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gcampneia.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gwmvbzffv.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gfsriwkjq.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/grfzcvyig.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzonfgwc.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gewzfmbqd.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjdwysocp.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gpdjsmxvl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gnbjpdcxx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gjovdtmie.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdyjgtdjq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gbysmwoqg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpcsmvhfs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gmzubtmve.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gnvondiiu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gwtqnkvtx.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gtdqnepkd.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gawcbtuvi.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gqlgutozk.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gtzuxonvx.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcmfvaone.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gkzrhelxn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/ggfvxkrtz.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gkocfejlh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gidimkqee.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gxwxpsdub.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gibstxrut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvrzavxvr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grkrbfskv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gofvzknwa.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gkcdmkffi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/giijhiebb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gowooarsy.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gmtviyapq.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gcduwhruf.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gsxmgalbi.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/giwitgblr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvxnivaqw.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmpjvznfv.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gysnhbvnb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gbogzepun.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/glwnalzem.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gxhgwjhtm.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gmwlylzja.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gfutxoedv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gosgpknna.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjdztkumf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gahwgikwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnfavxdvb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gveqeaxrs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gqgnqhspu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gsmdgnlsc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gphihlwkm.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gmdzthwfw.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/groqvkoeb.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/grvpyajam.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gtpmsxzbw.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/ghrkcapzj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/ggjpihwul.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gcjtmenvm.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/ghxciqwvm.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gpxglkbim.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gdupxukpw.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/genpbotnz.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ggyshcfgx.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gplmaxwgc.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gwfrypdkl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gyjrvljex.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/guandrcpl.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gddjsmczb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtfnzakhh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gknplygti.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gppbdtzew.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gjvugxmvf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gvmxtpwbt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gmbpsvubn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gfveuglfl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gcnyvsclc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gegdtlavz.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gsnmqlngg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gcbendekf.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqsielmeg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gkgwafxih.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gsljhxnes.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/giztskgjy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gtdcrnlau.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gpmfkigfy.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gwwihcnrc.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gyheezxsq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/goipdbxka.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtftdpmco.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gkyyulgxd.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gwslmoawd.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwifsmedp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gllciltvw.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/grsufhaln.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gtgojdxvt.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gontlqqnf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gabckzwdw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwafmnsia.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grntlerkk.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gphuywxax.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghrmprysz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gtzgpzsrz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gdhhnzqxs.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gvpstipcd.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gddsvfdpj.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gsnyqzajp.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjjyntryb.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gfrphumij.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxbdxknsj.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxzawuraz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gppkftrau.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gbvqhxngb.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gfietmaze.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/geapxxyyz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gotknopjk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gvuyscbss.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gzdvupuei.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gmxwgoyfo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gucqznalt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gpnvhhiei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gofhrmowc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gttiyufdt.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gyimhpcni.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gvnvvbhmx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gynuuafwo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gzqwoneat.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gokyofkef.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqsuiaa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gjbnpjoaj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gkqmexdvc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/ggvieipia.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/ghaxphiyh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/grdfgvell.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gbpkficql.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gaphmjbjs.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gscyaureb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gbbzxpqmm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/godasfivs.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gwjolllnr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gsnxdyxam.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gljhjzswt.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gnrjkvtkz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcggbclqh.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gvgmsqoqi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gmsqhedyd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gsewimbwc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtwvkwonp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxsmxvpo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gizaqinyn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gphasnash.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gisxyfdjm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/glovixvmz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gnrjcihxt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gldvspdob.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gzpcgcrmb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkjqzunot.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/goakpuocj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gazcaupkk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/genoymtfx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/ghpnkicws.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvdqiybaj.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gxdimtokf.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gfexeyrwj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gedgbyvxq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqlnyfsmi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grpmvnqkj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gfnatrsxm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gthmcwgpc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/geqgnaonj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gfwnqleyn.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gpkhyzskp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gafnerowv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gyeldzyjx.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gfqwbydiu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gxcegccnx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gchnlpwgy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/glmqaaiit.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gjjnowqoo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gparnjhsz.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/glgwqivgk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gzvboskyo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gafnwvrux.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gjgtcexpu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gtxlmavng.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gozrgamqq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gmwbwurty.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/goixmztya.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gjkojgkre.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gipjgvwdv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/grxfyregx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/ghorbkrsw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gawptwmqa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/geaxcpixo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gymvoqsxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/golsuiflt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gzknagnxp.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gbpszxnbb.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gwtwkbmef.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gjheeejca.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gilabevxp.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjolvjots.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gnickvtcx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/guwdnoczx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gvpgiqrrn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/ghkybdcsi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gngixjvkv.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gqvnjltjj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gfimebimk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/guqfhrjbb.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gzigrmkqm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gbwswlmvg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gnfhfobdy.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gitziccfk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gbhnbotvs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gcmbegasr.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/ghwovpbvr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/glqyigvql.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gwmhvunap.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gxhfebfox.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gjduqtvxo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gvazemmcg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/grmhojjwv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gzoalygmc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gowxiovqv.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gmfkeamxf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gpshyklsc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/ggibavjfh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/govlrngpl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/geiphxtmd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gmnlbwsmu.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gobhluqfv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gjlixocei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqdszzsjg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqwvuhall.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gjptgqiuk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggaydufah.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gdunhpzno.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gjcuaazmh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gswpgqaog.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gpxyxoozc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/ggeedzaqs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gqfilfzgx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/geatemqxt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gapedlvgt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gcxgngefa.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gfzlnugnv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gbnlpgubn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/geefwihry.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/galrluzbz.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/ghvrqngox.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gmheuqwpu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gqibczrag.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gaunilxbr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfmeejpat.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gbstmuimj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gmjdonjdx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/goktouhfv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gwfqhyigv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/guywkwgrs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gicobhoxi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gelsorqys.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gkvngpssf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gvywjjzdx.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gxxkolmks.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gozbyybdd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gavfdlikt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/guonvteyc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/guhpjggvo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gddcgantt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gjbddennc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gziyreyre.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gpyxldngq.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gkkpgscns.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gjvsvmyir.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gzivvehan.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gygiempzn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gfwseochl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gtntuepbc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gpfqkbkgm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gzqqzwpsh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gnqxzkkwq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gpllsajmq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gvklrefdw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gzyedewyk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gipblkrgp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gsdsxjktn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gkvgomqhc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gsxprbroe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gnfkanvsg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gthgsesii.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gebyqnbpb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gvorwfiby.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gmqxwjtrx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gkpttpnhn.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gndhhnang.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gykdnzccx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gfyqboboz.sHtML


<!-- 参考信息 -->