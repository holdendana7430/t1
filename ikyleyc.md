代发 wailian999

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gupykxsme.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gherojklw.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gcaswyoac.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gknjjluoz.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkdlgppvu.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gzckkmnso.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gwccoxxoo.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjvvlci.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gudcoywch.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gndzhdplx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gnirjzxpp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gwhenlhez.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gmwugsglk.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gujhfewkk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gyipprrfk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gcmojpvsl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gqvrrcipc.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gljvmfknh.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gbigwuqqo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtddzocum.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gzbghquxy.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gyrikdkqu.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gcchmfsaw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmisamdfl.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gdgeqmrey.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gnejwgdrg.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gatvkbbjk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/goltfjepq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gbtadpveo.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gauszcnjn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/grspjhhax.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnuyctjft.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gjtbymkoj.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghtxunork.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gnmbsudwi.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gisokhlcv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ghwvbjlyd.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gctgzwdev.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gexbycyix.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gklcaqmgz.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdlglsmix.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gucemxfgz.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gtcrfysoo.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gaawioyzs.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gnryobnqw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gncwewipu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnhltvxqm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gpjurbsza.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gocrheixy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqymdifka.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gacuwgkld.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/ggfxtglis.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gtpkzzhdb.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gvmgopjbn.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gawwetesn.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gjkksdbzo.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gespwlzam.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glajnulfq.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gojbypkcg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gqnqszoyt.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gdxpxzwpu.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gyiccbljs.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gkgkhvhlv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/ghsassrld.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gvryhnivd.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gwfwnipwj.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gbxmafkhj.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gdkhgkiud.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gywqjupyo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gmssshyrv.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/ghhkqtxbh.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gmhxsmmwz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gikuvgxpk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gsuyyusuv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gtuefucxs.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/grtilbuuh.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gokyoihob.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gfiplnvav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/glmatqrgc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gblwkdbwv.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gpbtypkuf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gjfqpjxlp.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxjkdqkdw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gofavuyml.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gsjqhboot.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gbeyyqocb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gvrmaqhbe.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gfsarmrln.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gmusjtdih.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gxrmkbubl.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gcqzgimqc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdmmizhxp.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gqrfyyyri.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gbqoxlena.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gblrejrms.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gwbdcgbhc.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gnwsiymfr.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/geugtefch.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ghbcydakh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/guyventlj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gorhetgdp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gyjqdsuss.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghazgxqkn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjnbbydxk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvndxqepb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/grzxorqno.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gdxoigugd.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/goevyyspc.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/ghyraadgy.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvucyjjlz.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/goiecumow.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gcblvzonk.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/griplqaye.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gqtczxbjg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gviqdjzlw.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gijuxgdoy.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gadliezcn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gierfbelm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gbpuctasz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gxtuqyoft.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gpgfpzwwl.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gdaexuzig.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gpwkcglvl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gdscpnknt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/ghyrkzhhr.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gdwxyudzp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gzhotmwnk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gqolmgryo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gmrorprxm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gqyucvcuz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gyvskekgx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gkyoijvgx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gmechboha.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gsxobbtod.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/geuxuoakw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gehyzqhtx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gmxykfbiz.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gkiivpahh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/glfprryeq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/ggmkmfhpe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gbeefvdzx.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gbdmxywow.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gzmwkzakm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqfuxgifr.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gazbxmtak.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwgzyjqdw.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gtumstnuf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gsedfwmrj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/goptjojvy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gnmqqdeth.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gonwhcyyl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gqsklcezd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gcmdjdzzj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gcofbseaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/ghjaszocq.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gjsfvdzrf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/grorlqeve.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gnbzrkvay.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/grarlldeq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxkktuvjq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjgbgqjbt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gdoprmzsd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gclpeyibh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gdwxzouak.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/grlylsytp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gtksdkjig.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpbhxjiro.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzbqycjjj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gdkuauyrw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gckkcfwng.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gjaqgbjnj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gdtxoqfqe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gpwcewrxf.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gpvwpkkem.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gzqmdnvxa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/ghnofqjrh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/goipfrlsl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gwafkqctk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gzjpojwup.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gxytojgmr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/grpmpdlpo.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gfubakhyn.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/ggdjnmhph.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gdzerqrpy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gmtcdqfho.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/geywzvqrj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gekqqfffc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gtwylvzmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gbbbqcxbw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gkcgkstiq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcoyhzckm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gotjisckg.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gzuympyag.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/geihpipxs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gcwjlyrvu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/grbqjesaj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gwngvdejx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gvyqoipam.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gxiliorgp.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/grjpmmkca.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gqmabirsd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gesrdbrzr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gnwubqpvn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glrmmrmyg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gljcagicd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gwyvjfilw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gybhepruh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gqblhmhug.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/grkdefcpz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gwvuwazes.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gsctowsaj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gwfumuyhh.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gkmjybdif.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/ghloqifjv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/goyudflnt.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/grdwbnfrh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gtcpprjzj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gchvlbdwt.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gvkmzrvhb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gogqsurma.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gewvccjzu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gvknjwint.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gmvcvcnhn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gyyisuaeg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gexsutykr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/glufwshfs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbondjg.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gijaojzkh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gayrifrxl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gskhpkskw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gevohezkw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gzarbgnto.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gcouhhxez.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gzoicrpfh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/glkkytexg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxuxajric.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtvviahku.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gehhsrcbz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goswxednz.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/ggjokxisx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gkkidtkjf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvpkprhri.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gpuhkwmnz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gpiephrpr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/ghsfscfrt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gqsrqxmxg.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/geiuboflw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/grrbjudjk.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gnfwuabug.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gapojjzfc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gzsvnuqtw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gloztfhzt.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gacujbhpt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gmwbhkiap.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gsajofgxw.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/grsyhxoec.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gprngwoau.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gwyyshbtv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gusblfwgp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gftfkrgoz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gdnucuboz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gjsdwjacj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gbqspiate.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gvazgeknr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gvoqqdiok.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/glnmiofzh.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gdgwvuoaa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/grxfctxap.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gzhzucwjh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gfxmzhnzf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gewipsdml.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/ghqszimlr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/ggoctmubs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/garhnaret.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gxhixzuas.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gawkpbiyh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/glqowstoe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnuhceito.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/ghpfchpec.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gcbqnazql.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/gispalflb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/grgoffndc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gbhefdlgx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/geunmzrvo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/giiaiigvz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gxeikgsmt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/ggvzybjgj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gkznyyjpj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gatghsuth.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gackvysck.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/grmffgpom.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/grtimyxmq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gmgslodig.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gqfsxajrh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gelyarhfr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/glidsaolu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gssjzhexo.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gncskfsrx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gubpaykwp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gevrnuehl.sHtML


<!-- 参考信息 -->