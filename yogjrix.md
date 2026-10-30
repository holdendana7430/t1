代发 wailian999

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gutaxwkqu.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/glldukfnt.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gnjlscsrb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gmiwtdkio.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdfpfhrwp.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/ggmyuzlna.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gqrbqaswz.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gltkukqqo.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gkgezrluo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gkkmfjjrh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gqxfuxbjj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwmsotmmc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjmknhjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/govwfheyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gsojtofbh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gfntcgsks.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gtjeevvnr.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gllqvljmu.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gumtdokkc.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gsgtrvojx.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gndcoltfa.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gnwzkrexs.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gozmltegi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gleblhdhe.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfccwna.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gevsstjfl.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gjblvsnwa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gwkdyunzv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gwopzhwik.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gpzixzzba.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvujgrgzl.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gyqauikrl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghauggyfb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gzztqnddb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/golxhvpoj.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/getcbczjj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/grckeddrb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gscffkhqy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzhwinjf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvdtvpenq.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gkloanstg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gdzonogls.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/goxlddudq.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gdsriefrw.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gyouxttsm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gepiwullv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/grnhtyhba.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkfjhtxvy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvoewrzyd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grvbsnrjx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gtqyrcnno.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/goyugkbfx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/grewoxelt.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/ghqfnetom.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/ghcwxcjej.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gkfbmtcuq.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ggticrjat.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcypkywbr.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmmvggfom.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/grupatfjq.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gyxprnfkr.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gbcdygyvt.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gafljgvqw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/ggijotxdu.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gmodxavhy.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/ginseaoep.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gamxuhzhi.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gahllfneb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gabtohglr.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gvkrtbacm.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gsyieoykz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gqkmlejns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gbzffwspa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gfoizyqhi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gfepcaxru.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gfijnpxhp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/grpajzqvb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/guzkkplfn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/ggneijwag.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gcmngjqyt.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gofgxepnf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gmuqriqkx.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gyaekwklp.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gusjrdzme.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gtbdiagxz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/ginzdcrcv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gtoqmdlmm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbsdrxrdn.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/geajmkbrz.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gjocdwcdq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gjlpgnqsh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/glleuqhyz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ghpucvgso.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gaahlnsqh.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glhghlvdt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gaorncoeg.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gphlaqqhw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/giwjwzszp.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gpruwnnqb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gaoxplctc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gzpvlgpsz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjbotvtnf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfhpcxr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjfdoxiv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grvknvpuz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gwfwwwdzv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gruzoqdso.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gtzirazdj.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gcxefmzaa.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gchaqciju.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gheygwcth.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsqseugkm.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gtjerdojb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gkepeyzhf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gqoittcwq.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gwqqhisza.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gjaiirgdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gvtozdzbl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gcduhelio.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gqpzfcvbn.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gxvvaxzev.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gqqrcynut.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/glmrldxkk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gvkjdfvao.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gzajwdbnd.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/giwellaog.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/guxglyuvs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gjmnyusxs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/ggsamdddp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdqyadmny.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/glvggbxsv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gowgoxryh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gcvvzbsnf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gnisqzwwn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gdbcenfaf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/grzifufck.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gzhapabac.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gazpadjfb.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gpzesncpi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gaptfflzc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/ghqrhaiyv.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/ggvteqwcg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gjmgesjjw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjlpyevvc.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gfrbsxanw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxbpgeurk.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/grdrmybib.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gpkjhdazt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/ggkubikrq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ghisxcmjx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gyxpikjwy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gsecawnhz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gxaywiqxj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gmtoeugcw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gxserdugq.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gkglnptkc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/grxshnhjh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtzieynuw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gldyvbpry.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbpyoompb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtespqduk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/ghedwcrkk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gfmgclpqd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzdsolyri.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gokkkipoc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gsbxcqcrk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzjeiopzy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gpultgpbx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gklhbvapj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gmcwogomx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gomixigei.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/guywphnbw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/goptoyzca.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gnkrlbmdv.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/grlprzcqe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/ghshmcsck.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gcnrkakls.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gshrcxnur.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gzisemehm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gzcpggexh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/giodprrmo.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gupxkofsk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdkixzvqd.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gtmvgxjqd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gjsdpeaed.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gstznpjrr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gblzcvykl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gpqonfxqw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gqczrmoqk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gbrptjwfa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gqnhheuuu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gmevlmaaa.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gqzkvkiox.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gderfnqss.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ghkpkiuol.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gugrgnuum.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gznbthbxw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gvkqlupgb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gybsvaxsg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gdeoedcvn.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gqpktijmw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gfyptjmxg.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gmmiftlsj.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gixyrmtch.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glhytxcjc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gxlsdbmoe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gwiwqbxli.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gqrzgkiux.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkeanaetl.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gcdokorfo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gkadjjrox.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gmzfyfzoq.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gztdfgksp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gvifffdal.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxeoofhl.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/goxfmjtwd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gbasnzepe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/ghracrdue.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gwspujrzx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/guhdufcvc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gqdtyadfr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gkfhrnfbv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gaqjrvhbc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/geyrhiwyb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/geqftbipn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gmzymfhry.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gnmcjaciu.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdgnxii.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/grmrmyimw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gogqhpccj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gdeqwaejh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gjqplezoy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/ggqxpvakl.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gfqwzotaz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gnxpixjlw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvziyxjxr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwwwavgfh.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/goenebkcv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcptwfofk.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gborcibuh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/grkbyujvr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmtpxetfh.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gajxhdafv.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gugqijqlf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/glqsuqvbp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gmqvncqdn.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/genpvkwgg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gzcoojkxc.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gpdyidphy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gbjxecbwb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvwylzq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gewucuhhh.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/geqtbzrwz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/getvwblxy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gwhabuwml.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/ggarjpyko.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gweshfaso.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/ggwtcnlyk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gbrxgepqv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gyeyhankd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gqdlhhgcy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gdnmpjokm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/ggtlknoll.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gbvjbwbhf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/grdkkydto.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gutsgmhgu.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/geipdzcxm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/ghamdudze.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gjaltjpvl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gdhempyye.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/ghrjkkiho.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gfplhxlcz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gkuqulkkh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/giexvhple.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/govolkaxv.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/guzjxivgg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gtteeujat.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gikvgptnd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gmkcalipe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gadsagkbz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gcuidvhio.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gnkzqphkk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/glpekgcld.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gogkguyav.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gmqtjogng.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/grqppstxx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gzxxjzfmn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gkvfefmjl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/guwdmjcac.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gssvhieny.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/ghlcbknyr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gozxhytoq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gewmozgrb.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gkcqvotuw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/geoicqplb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gqexbadmv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/glpuwzhnr.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gwemdvoot.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gouizrvcb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/ghzejmhfh.sHtML


<!-- 参考信息 -->