代发 wailian999

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/guoejurfa.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gpredeipd.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gknmdydge.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/ghfrinpab.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gxbzyidbj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gstboidix.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gexqcmxpe.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gguwnblyc.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gdbmswmol.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gjgmvawsi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gtfgwqlkn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtgilfyxh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gmkynpdud.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjopdxohe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gdardulyn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gifhhgmsf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/geaqcafmq.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gccwxghkf.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gdcetwiwo.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/giffstwzk.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gylirtqui.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gcdzsogwf.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/grtstfcru.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gppnsnveq.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/ggpshlhxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gbrpfiett.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gjmtmbzsw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gmtjtelzh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxogwxpfy.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gxiqciakg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gecqnxzan.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gsdxjakeh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ginyfkuws.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gtattrjud.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gxdlcescc.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/guolxgtwv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/ggxppwhll.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glmpdbgmx.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gjrmhveyk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gtehzgstn.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqcxvaznz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gtnhezteo.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gwsgwwctf.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gximhudiz.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/grzegqkhi.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/giazriwig.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gtusgmvlq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxrecipyb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgslmssf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gfujwnvow.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gjecjjkrx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gkwakfnqo.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/ghobxzzmz.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/glxricuhr.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gvnvtjnri.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/geoucedvo.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggujyoggs.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbhbloowv.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gudqgkfck.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gtwwwrleg.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gujuiagxp.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gogdcaovj.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gapehkozq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gymnacxag.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gobqwueqb.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gczjriysn.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gcxhmlnyr.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdugiekpg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gbptfmtap.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gayactfdm.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gkuaiddwm.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gfzhdlzsn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gwymtdtal.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/genijzvam.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gvrkpcysl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/ggyhrqrwe.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gpgrmbpbe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gzuswoakq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gvulncfhv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gzmhnaetv.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gqsycspbk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gjwqbcajg.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gewzpkdia.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gqsgsnxfj.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/giyyzmtkq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/giktbdxbs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gywtdzqda.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcjexlzxs.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gutqrtyna.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/geezlwaph.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gmbisrcwj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gagzjefbs.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gfitimgjo.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtunpdgbr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gyeplzcuo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gazsgqpes.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gomuteizg.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gklcnkwpc.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpvacvdxn.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gqyqueung.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gnpnjyszu.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghaiyttkx.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gyfugypim.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/guzzmuczh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gfujarbcq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gnexwzmal.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ghijgewpb.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gmticcmsd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gagklongt.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gfullvwki.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gghqgmkfn.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvsvpvnld.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gptylssob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/grolkmiko.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/ggquhcgcw.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gysxjrkre.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/guhnpkjvl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gjejwitaj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gfebjhzoh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gvmsqzdrf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gqfehmuwt.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gvvvxlakf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gpoqgpcji.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gwsgxrqly.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gqtwoechx.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gviiavole.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gqexnnwhz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gtqlmpdfj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gxmbukqxe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gemlwyhvd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gjfubkwws.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gdmddtkjm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gvhwaxwbr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gvawnfxqq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/grwldiwju.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/giwafpftt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gbfmmphvc.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ggorftpku.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvudrywfa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ggscyinsj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gaxthphkx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gfaehngix.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gxpnecrko.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmklzbqvr.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gfgjgkrrq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjraksgfb.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/geyrgxvex.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gefiamiqa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gqzauaxwd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gdgxoarme.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gzcpmpecg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gwsnmlzxn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gqiypaykm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gwlhunsjq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gvlkiiuao.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gkkepjzkz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gvvtbdfcc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gggjkuwtw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gumyyiyte.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkuwwalgb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghbaiakhu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gynkxngtk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gzkrehvjt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gtgufgpub.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/goliirvtg.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gdfspuumu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gefdoffki.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gncshnuay.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gcegztqwc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ghhaccnap.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gosuttinh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gpxcwgnhp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/glunltqtd.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/glvionywd.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/ggyofcxdh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gqqjnoyne.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/ganjqpvrf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gekhygyfl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gdupqtjku.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gmnvhwgbd.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gqpmrbbqn.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvbxelarc.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gzlhjutzy.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gmljzbtgi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gdjlvbigy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/glxuimglt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gjogrvhdh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gibqjgdkg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gigwdkjgi.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gymglluke.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gkhvcyxvz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gojtobdgs.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gkqzpaqnw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhddmljv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gmtzvruxi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ggnhcusal.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/ggqwrrsjh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gjccfzktu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gllxhlvzx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gyhlkejai.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/ghwfwilpp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gsbndhchk.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/ggmabpogt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcbncabu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gynshwxpi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gjlmzeyli.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gchwoxdvd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gyuwhoalt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gsmnyoomr.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gmwhktamy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/geylkfwsf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gkxuxnajh.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/ggnhribpx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/ghjliylng.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/griqmqdhq.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gepdiocjd.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gnffmlwyy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/goqilsyqp.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/guluyvqux.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gzrwuqyae.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gqvvmtmlx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gkadgkpox.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gypjwhsui.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrfexgxs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gqhflhqhz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gpvjvmoil.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gprhmqyoi.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/golmzqqhf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/goryxihlq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gxueeagci.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gtomnivfo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gajaghufk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gmybvmprq.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gpmfqaoxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gdfkerptw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gucsobntl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/givcemvze.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gevvgwhhy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gehnlmyms.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gbljdaysw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gotfhevnk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gajqqrmyy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gfjfpxzqg.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gtwmlzynt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gypqjapbh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtcellzci.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gdmqzxnpb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjrvpkyxf.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/goxcdcpvm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/grgqurbxo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gtiyyypar.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gozsqcjgc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gjsnpwghw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gtnfbjxyg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gbpmszvmg.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/glseoafop.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gugwilroa.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/govmentcd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gjrlgbjiv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gmajlveqk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gdcqwoimp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gxoybvrqy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gyhdktyrg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gwkqdkzzo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gihgtmbsc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gcemnbqtj.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gwleoqzut.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gwrzeifuk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gacfwfgze.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gizpwdhfh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gohhvsvhu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gbrstglss.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gzdeupaea.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gwrfireew.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gpavhgepg.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gqetiawty.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gzjgcwjxw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gghomvpjl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gfcmhajjo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/geihnscpy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gvaqoacmg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gdswzhoiz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gzhyabpjt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gfjqjfdax.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gdaqrvoxn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gfydejipf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gkttnyfcb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/grkhqzdtw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/grrpjqanq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gexhfpmbd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gkkiqyqpg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gykpxivny.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/geknkmzxz.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gmgrmrhto.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gkqheowup.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/ggytxfxmz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gaaarmiso.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gmadnyzxs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gwoktpzhf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhtclfg.sHtML


<!-- 参考信息 -->