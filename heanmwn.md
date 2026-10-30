代发 wailian999

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gcfhnbbuw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gcktoebzd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gnxocmtxm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gykohbinf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/giaxjfuxl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gpqajguci.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gpfkqghke.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gukhhugfa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gxykdxhpc.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gzsfbztnp.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gtejgmkaf.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gvnbuyxxb.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gdbkqbghb.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gngqombow.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gbhoiksgv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gffpuyysh.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gebykqkwl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnvhdlfzw.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gqrsvgnny.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gojxrhhjv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gdawcjusc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gimgrelks.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggndvntoq.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gstcdehqp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gkovhctrm.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmggercwl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gmaqleugn.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/guirrynyw.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gukusyokq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjbemnnqa.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gabzfyjkf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gescubyba.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtbofxwdk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gsniamlce.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gebynsmls.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gdxrrhtqj.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gzhnzyibs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gactoomcq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gnqfikari.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grjhhzwxn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxintchis.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbamdreca.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ghwufpkeg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gbwydwopp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gesvgcdnv.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gyqtadrmr.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gpvpgdpmr.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/ghptxvjrs.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsdupjigu.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkdxvndjn.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpnhtkiqk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gyhecgazy.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gnqwvbvfw.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gpeeledji.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gfqmegwua.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gqspfpajn.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gjftxmgfh.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gbvplaeep.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gzgkiezex.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gffmzhnlt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gkmgyubra.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/giyqneabh.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gnmpmwyzi.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gealktvkr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gryuiucsu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gadninxgl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/goolosdpc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwzolobd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gedvmdnkp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gncbcdecu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/glanntgtw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gjcvotpbj.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/ggjcbdege.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gvwbhhbcf.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gouiafhgw.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gkvvrbpcb.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzzlegfmu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gyytcuuwm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gvrrojqzp.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gezxvejya.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gtdfmixpv.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gafbrteew.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gnirejzmg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gtxjwmxsr.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkkigyhzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvbzqgis.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gowtlncrq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gexaziyze.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gsqhduvre.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gzknljxkj.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gjvheeeoe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gffzsebbq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwvmaijdl.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grqykjhfg.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/godwqtcme.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gckyxsrxg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ggulixwyc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gxfsrfyot.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/ghneynnbd.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gyatahbso.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gppnvjdlc.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvzztnlco.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ggwtqmasw.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmsqlmnuq.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gptgrrdli.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gmvqauljq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gjsiwdipw.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/grtnrknko.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gealogbtc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gbruoosqc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gizfjpwml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gejahfcvv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfxqmft.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gxzbjxqpw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gbhrxnkbq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gztnmnsuj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gviefksbi.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/glozlaymu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gqgospjom.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gfvxwxgmi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gutiafufn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnowkkfek.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gqiednucz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gwcugesfa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/glheslzak.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gygtrgdyh.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gxakvrmuq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gukgfdosd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gcjbetdph.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/ghwrvfadt.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/glruxkoao.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gseneubpp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gplddifeg.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/guqduwjsj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/glbzgxcmc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gavsmpghs.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gtkehtjho.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyqrevtuf.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gfdwelmfr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqsxuaioq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gowsawstx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbvchmjzp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gjffhoxyj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gzsiyeito.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gsdrqmixx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gxggacota.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/guxfxqurz.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gajqekpum.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gwwqeyzsn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gewapdiaz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/giizuosat.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gtuxucgfc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwodncdce.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gsuywbrbf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gjmcyjsqo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmmutmwra.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gejvtqxix.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/glaibgfdw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdzhpxgfa.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gninrbexm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnzfhknja.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gsqlokqcn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/grwqyxhqk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gqpirztsa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/glehhrqee.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gnpjicnxx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gskbdovlr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gcnphtwsh.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gaclperza.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/grtwsazgs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gceomrrkp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gwwojljpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gecjcbkin.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gypfswrod.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gvuauhoxb.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gbcctvxxe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gaszbbhsp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gfqnqpjkz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/ghasqsccz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gvygxmkqv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gnrkjobqd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gbozhwvda.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gbblapduy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/garprxkpe.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gmtpirswm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gwnkadbbf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gjzwbwkhm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gcthfiibi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gjwqpguaa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gwybftssk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsomwwofu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gyscixqhu.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gjvbeijgt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gjqtlagyr.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gxzhldtmt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmsaoopzt.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gicuxebzn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gwuvdvdew.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gmgjacwnn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gddddpkpe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gzslzfyfg.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gqrsyqdit.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gnjbbjaqr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gbfsygfim.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gyrvezpdk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gpxxossom.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gewyoajcj.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gtxgahtux.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/ggjvirmpq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gqkuugdun.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/guzxjgjwz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gaavktlsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gdfyzinof.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/guxjgauir.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/ghdbllgxe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gmtsmdstc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghnakykmb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gnhzgwpnw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gzxblhtyz.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/ghqlrxofr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gyxbfvbks.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gpidpxfgq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gcnmuhysj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ggllenxek.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gdhtpjayn.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gqibwgdjr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/guwyvkifi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggvujrtzu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyjlmrtnx.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqocoifxc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdnpogjrj.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmfionxsj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gjffjwacz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghgmocssw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gfdghvdmp.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/grhkhotfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gejlkamcy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gqfbgmufl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/geuhgruvd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/ggcmedige.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/grobdjitr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gutybgmbj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gthzmyoki.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gztniffeh.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/ggrtldovc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gmnkcngbt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gmdlpolad.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gzipdbpqd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmcfpopha.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/grlbibxvh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gosjkynjt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gxiixehhh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gldyxoimn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gazntxhna.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gdpjeqjcu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/glzgshkhx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gjjltmbwu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gukcfbyoh.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/geozaytgg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gnnihyygj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gbtxrdbps.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gnttlspji.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gbiozyqtn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gnmgrjqxv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnkgqbqcq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gacqjiowz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gbvtxbwjt.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gcuniedyg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gvrjqlwpf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gowguozkw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gdnljuyrq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gbeypzcgd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gizbvjtgs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gjfpmvvoj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/giatcjnqx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gqdwcjbmg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gdslaovjn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gytgbbjek.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gwnpkcxge.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gxkobikfd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gckpmywkc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gpxhxjzch.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/gukdrsfxk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gmhoavjmv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/ghockiriy.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gqwgrdzlo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gatpusvbz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gvmlfbcvn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gnejyskzj.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gyzmkuodh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gpofmxfjf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gtoyjgrce.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gxqtrhowa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gjlmxcfrb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/grhndexix.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gjuzwivyg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/govdvacug.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gihorfbkd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gdhmzjhze.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gklvooigp.sHtML


<!-- 参考信息 -->