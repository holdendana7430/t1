代发 wailian999

================================================================================
来源：http://wap.hesvh.cn/Article/details/giimwtvwf.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gqhabqbiy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glrcklhqr.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gssiimmhc.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gfxzahrin.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glapwfsgx.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gioalwgqc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gaklzibnu.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gndprmokb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gkvhojzbo.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gtvjrmtte.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/grnzmijkp.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gpsfhpkmq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/ghcqyhvfi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gisiqqkeo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ginjzsnkw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gabbtgikk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxusqovuh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gtmkelafo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gxsrwzhua.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gxemzuith.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gwthmypyt.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/glqtzgvfb.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/guvtbiodf.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gixztodqj.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gaavcqjhw.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gixlxtsbm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gxcehjpho.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbuuectey.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwuzwerzc.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gjwsvpvvv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gmugfwdix.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gqjtagacx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gprrpjxpb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geakyhlwo.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/giuzgeuta.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ggwezikxu.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gpxdaofdz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvnzsgiod.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gqosvodnk.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/guzyjpimp.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnnmboazm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/growwtokw.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfabouxbo.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gnnlqwuqu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gzxzgwvkl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gpiroojxo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmhqfbn.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gsbuzkasy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gfryyreim.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gaqkbxqix.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gaojfllhd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/givtpwlcc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbnrcsike.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gbfhjjcfl.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gwzztiois.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gcmohlinr.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/glwmadzpf.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gpcrflksk.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gzgosijuk.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gtsiorqlz.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmtoeovbp.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gdqwsfsbr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/guhnjafkl.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gphgdhnfb.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ggbvwuuih.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/glwphfrti.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/grtqhoudz.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/guuwzljib.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/geytmmwpp.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gshaqodlr.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvlupjyeq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gnvzaqznf.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gybrbwhsg.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/giehocvwm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gtcevtfnr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gmrblohvf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gjsqdebjp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gcykaopyi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjcfohrp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/giwmlnyjp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/glhiyrcqr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/glgmjcqsk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gudvlvuax.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gxaielvnt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/glcpiyvdq.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gufejjouj.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gyubmvsml.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gtsqgnpef.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gattairyj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gvfupnuoo.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/guuhmkrbs.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/giusywntf.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/grwrenrpi.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gmbvbmhax.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gexdmanng.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ghccavmsx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/guwcddfxt.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvloadhcq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gbcyvmtzf.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gpycfwejw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/ggpjsoame.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmdxjiela.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gwhlbsclf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gpazxpkmd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gggmybvar.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grtisdemj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gwjcriyoz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gaewbgzsn.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gpqyolsci.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gzxcuudal.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gcxzawrby.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gndsxiarb.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/goiyjdmoq.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/glvygjkyq.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdtmkmizg.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gnyjnxmra.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/grunqpazc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/grkezrrhy.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gezvljqlk.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gccqqchzh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gjledhden.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gnzmnvcpy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gmjhgiuad.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gsgyazfbl.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gwptbmcos.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gmpnuzmmd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/genufduip.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gmnekzktl.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/glmpmcwoy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gsukpgphi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gwubshfzi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/geipnaoky.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gbqxlbdnw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gbytuyrru.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gohrcxfnc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gutpqphnr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gcuzryafq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gvfhkxazk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gsbddjran.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/ghtflewhv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gegymydvc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/giaucghrq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gverfgbbm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdubqpxtx.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gmlstuqhd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gtxjrgcfu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpehohszs.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/glnwisswc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gndguvfoy.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gepgdlpyc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gbjkzdiqf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/grbokgcax.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ghobdmmcq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gepdfpqqp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gjabghdpc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/grijwpvmz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/ggvjuvxux.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gzbfumwmv.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gsjhitinr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/grkbceavs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gworexjtf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gnyacdzuf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggwyrktox.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gwwvevlji.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gfhbyitwe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gcpicvqpx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grzltlrbz.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/glckcotht.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/glctjitur.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grlwdetwh.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvkkwxyes.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gojnrmojh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvefhvzze.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gblnlzyhh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gyncuwbgz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmxpvkrxw.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gxprndnxz.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gsgirkypq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/guikdipmz.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gcpxbfqnb.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gmjqplaxu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/guynbzkiu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gapelxght.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gwdmrermy.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gnfizvrak.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gjhvjnlmt.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/ggagptjzg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gcyftrwic.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gwgwbntal.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/ggbupryxv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gboxrfccm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gdjbqbmhc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gtsveehhy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gomdhevzc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gjlxujddv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gdyruzfsi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gnrzkvmbs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gikdcodku.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gtarodfao.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gsubrvkjd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gswjycagx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gwcjegvos.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gtlgfutoq.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gowfvdfhc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gfikcwjen.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gpahjcoix.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gpqpslmnn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gkgiidquc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gjezadxdx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gyjlwybni.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/ggnfhdxok.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/goajtxvrz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/glunujgcf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/glesrapjk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gaaehdjgx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/goicklcww.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gwjsfggdp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gfdwgxdhf.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gmxsmgxpt.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gnmyclzwp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gjohjotyk.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gbmraolpv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gmauhljyb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gadcscutm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gpldhnbnd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gpfzltiqs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gwtuispbg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gjfgdlxhf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gcgfbmapr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gbdgqewtc.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gizwaohge.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gvzgucpmv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gvlftjfht.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gpxhsphfw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gsqnnlhjk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/guongzsbe.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/ghzelebtq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/glohwlvyq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gspajmofp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gejytwujq.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gpzazmfxy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzrtblrxv.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/geyzebfpg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gnaqixhlo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvajyvuhy.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/glhbfexcl.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/ghylhymqq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gafyojxgr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gjttxkdkd.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gxrchwwbr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gcpnjtimz.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gebfmlizl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gitisdvuj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gifaeyyof.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/ginktrivv.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/glijcnoyq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghlwzumhc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gisfncdqw.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gqfjdpbqp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/grapznbob.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gqlknzpgw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/ghgonbgkb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gbbwsbefl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrnapjy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gipghahds.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gzhtrwywo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gtiftewls.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gkulqstib.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gunlhixhr.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gtpdbmhfk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gcvnlzlni.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gavdvfvgy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gswowuwlu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/ggkftqjko.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbiescgv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gwynwaesz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gdgrolxji.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gktyprfgz.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gygfdcnjt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gmzgwkbec.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/guyzahovg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gamemscld.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/guanbnlbh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gwelcenkw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gmzbqqinc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gytzdgczl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gapemjgfm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gvnzqjiko.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gnajouuot.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gsfrpqovc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/ghuwlyfct.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gbobddkmr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gfrjmykzb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gkuztmxtx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gtuzvraxm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gttcetbjr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gvwktbutv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gyqkhpsvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gnrhxznpm.sHtML


<!-- 参考信息 -->