代发 wailian999

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfvsueun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkrfnfqm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpanjdip.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjqfyedms.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppurlpdh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdusdmtvk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gridxgwla.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyuviwam.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazpylxiu.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhzpkjra.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjptqwzjl.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gwvkbvyhh.sHtML

JS:   this.name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gnybdrenx.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/ghmnpunah.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiyjwoyo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/gdtqofqez.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkklfjxq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkbnumeo.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwyyjnls.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngynyra.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigbdqowp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqymhrpv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbxqbnj.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gigogfelt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtcahviw.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/goqhfnbgr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gxccsautv.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmmqkcgp.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnocarwe.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxpgexw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxgmqrom.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwucybtim.sHtML

Java: class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbtznxiu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpajuvqt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffvuryk.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyiccdxg.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gzapejlvg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttqczusk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfputgmca.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfipkwts.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gotztscgg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipkixylp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmvobmxn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/gdrokjeap.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbavlcmf.sHtML

[G07] 调用父类方法
来源：http://baike.fanxiaobao.xyz/Article/details/grchxnfjc.sHtML

Py:   super().greet()
来源：http://m.share.fanxiaobao.xyz/Article/details/gukcflvzj.sHtML

PHP:  parent::greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gsejwqlcc.sHtML

JS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gasiudeke.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbmdprsw.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/grtvipaxy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjauoqsh.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/ghsiutvxx.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/grvmzlgma.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppvpkmfu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/ggrvgaowh.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwiundvj.sHtML

JS:   static f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwjjyxnxo.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjrglfa.sHtML

Java: static void f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gukemhhia.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwvvnule.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvphgovfg.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtghtujrm.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gpprgmxbv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqcuozhd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwlkdaf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/gxcilhvbk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghffgbfiw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gebqxmixh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmqseunao.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsnralai.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzmozhcw.sHtML

[G10] 访问控制
来源：http://baike.fanxiaobao.xyz/Article/details/gzwnzenmz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fanxiaobao.xyz/Article/details/glyfpadbj.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gfgjkgwij.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fanxiaobao.xyz/Article/details/gtozozhfv.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gofdzedmi.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fanxiaobao.xyz/Article/details/gdodppavq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gdvuoafhw.sHtML

Ruby: public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gtssqhssx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjzstusz.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgfxpyfj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fanxiaobao.xyz/Article/details/gpmxsjaxl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmctvlz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtitbeids.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gefeyhoww.sHtML

Java: public String getName() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvosggxij.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gapiaatkr.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/goyxaatgt.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzeofpeol.sHtML

[G12] 对象转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdibzwkht.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywgnbtof.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gamamxlbj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjewhobxh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrztgvdq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmqokinxg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gplnosdsd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvysovqu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyceieosg.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxrfhygko.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbxjlzqz.sHtML

PHP:  $u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gyejsvovh.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgpbnwsc.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gkuxrubfg.sHtML

Java: u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gcxjttuek.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdhyyaoz.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhyqrrgh.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxgyhdhb.sHtML

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/geqedzmvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkguevvk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/getbtvunw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gupzpzdsa.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/givvmxthw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhcbbwd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwshuqjk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaougnfnk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdecxzxp.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyaxlmua.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcejewzdv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkxczuxk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fanxiaobao.xyz/Article/details/gdeugmgdx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgsalwig.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/ggqwxyxbx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpviwgcyq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsaxfplx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnryfgwmn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/glnnirsub.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gisxysiel.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gqigyxynv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfgwqvim.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gghmwkalk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjhdonof.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvyjkvxz.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/goqhtbeps.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gwinjakdp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcyedxyc.sHtML

H. 异常与错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyielnkey.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifiipfbv.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkvwjvzq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhqetdn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxyqeeznf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxkgynhf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzssuoxi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/guyffpxti.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gptfohtuc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrikdmnd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjslzdat.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfewltfrf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjzmjkzm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhyncimc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsyvgorq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnwqkhaz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/geksslzsj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssbztqgg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gimwevjdb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwsiaonb.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gqsrjdmvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmshkgik.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshxxotpz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gucalueew.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczrkzsfn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaibrvht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gcjadjenw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnilckkc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqqdbymf.sHtML

[H04] 自定义异常类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqdscnlk.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gthxmrvgm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuncsvvv.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghydgbcbe.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gypylibzy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcskrkovo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbpfunou.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxfssirz.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grkvsnkmh.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkznmfdye.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsajiikr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnugowzyv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/goybvyxrf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzlhouut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxpsfdqro.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fanxiaobao.xyz/Article/details/glgkjlbbx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvqfttpm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gerszkcow.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdxnscdw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobsbpunj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvfamvaq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyogxsqf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gfyskvnrp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeotysip.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoliebez.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegmdapkl.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtmgskvf.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gpkpfokxy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgytcfbj.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/guymhbgrj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gzgenpgvu.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrsmvnfg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogtzykfc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gjywkgewv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fanxiaobao.xyz/Article/details/gadwwqjdo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyxyfhol.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/grfibmjyq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmoxvoq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gyioaloyg.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/gwugykfli.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggbobbvk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrueadop.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjqcxvju.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fanxiaobao.xyz/Article/details/gtjvaoznv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxoytmgx.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbihyawf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gpsfslaur.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmcvkjce.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbwgaoop.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflbggomi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzhuaxpb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gzanpjzup.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvfjuhgp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gmttsnlzu.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/goracczhd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhhqcfhi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmcijivs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gksyucaew.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxzxhzad.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gkjwnzybt.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/ghxichstb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/grmbnlhvv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gxxvzeeup.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyibvhyf.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxumgjqx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gugacvdta.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gsaqlbveu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsrnvgvna.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/githshvgp.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gokfspxco.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/geomcvfut.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gfnoqtqxf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtqbqhkt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzozpqabg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gptxfsnon.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlcnpyk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpnhrhab.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgosaycb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoqdgtgz.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gtppqeyyy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpfkolmf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/guliyhgtm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmozushjw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ginqmohug.sHtML

[I03] 提取捕获分组
来源：http://3g.fanxiaobao.xyz/Article/details/gkfegtqor.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlrvpzn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdtfgani.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/giropqypj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahrygcqw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvivwjrec.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/gyvmrjqas.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbreeyoij.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/gfagdajfi.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrkynyyp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwyapmrvr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvtxofry.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gmjyopggs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/glfgignmd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqelceol.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxhqxlgv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gclzscrdo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gihsmerev.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrpwmeek.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnmrsnla.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeumjtni.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gulkjwlxc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gaxgawrmn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gpexoorcd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnundodjf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwaenlme.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicmdwdsi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/gglfyiclq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyylbein.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjxfyuas.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gvclaykjh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gpuibqgwg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwyirap.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfeulcsh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxewlbgvy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/ggjgpyzvn.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gupeqpike.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabcftrdy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuqwddud.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwinaijtx.sHtML

TS:   /error/gim
来源：http://read.share.fanxiaobao.xyz/Article/details/gutsmbotn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmquiylvn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoqtqahw.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fanxiaobao.xyz/Article/details/gxobsppnw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgdlalvq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gngellgfx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvtsltbx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbceyklk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqjeohvz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gyjtvxzvw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gvblfusdi.sHtML


<!-- 参考信息 -->