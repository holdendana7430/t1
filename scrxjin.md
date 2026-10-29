代发 wailian999

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwyvzctlg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gpxtqwlbx.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsnnksggo.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gycerzfwn.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gngovxjvl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gdlpduqrw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqknjlxbg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/grzeougxf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gypgqvcmu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gsouacrsp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gtxshzrqr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gfjrtqrvs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gpjctsfmd.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/glgdpwzll.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gazpkebum.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/glyzthhho.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/geldzlqyu.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gzwzdvzgh.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gjjlosnmm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gagxlbgla.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gnvatjcsb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdfpzriqi.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gqsmmmpig.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gidlmebej.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpbaoxlpu.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gduvwulup.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtshkghxj.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzitirhpw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/galmbplap.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/grqkzkqbp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/goywagjou.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/ggvfiinvl.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gfykzkmkw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gituwyokt.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqyymbjxz.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/goxqijjpy.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gofttipno.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/grvdrjziw.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/guiiuqppu.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gmclqkumj.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/glwilsvrn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gvniqxnun.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gcskqenjp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmjjmqtwz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvlfzqsym.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/glwrhtnwe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwwggafal.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/ghmxqyyvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gklpqtirx.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/geqzrumyg.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/glavekffp.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/glsqtshpy.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvrlqhdni.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvnrjehrb.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghidygglf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gthqsgvwz.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gzbknszqr.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gfexrbcdc.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/ghlphtocv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gxvajbsos.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gvvmyaeit.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gklnbypeh.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gsfvgtaes.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gqgxrsayl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gqeupaqch.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqrrbwe.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gdocsvbvd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gjtnifbjn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gtmttqmbk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gywcypqyt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gcbauhzvy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gqgijnerb.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/glwdacdxo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gmfewgtvr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gmtxtxdpp.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gsjrgtjkl.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gqpknuucc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/geciowujm.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcrdoqjeb.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gbbdpuzeq.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gtqqxmrjp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gfcftdcan.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gvjdqtoux.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gauatuogm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gkrgavfkn.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gnsadznof.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gxshkdluw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkhoxrbcw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/glcrvpyeg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gulihybar.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwtyxtwce.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gndmhlfpl.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gsfctchtj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gagsqnucg.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/ghxpsskjq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/ggedfkdhx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gnbzfoxys.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnlwsnpbq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gobzzendm.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdagsicji.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghoahjflb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gwiquzrvl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gkieloteh.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/ghkhimvju.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/ggtwbcqzf.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gqrqttolw.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gbrytfdmb.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdtfgbxxa.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/glqpzkntr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/guslrdaig.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gualgxndp.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gjnromzue.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gqfdnfsyc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gdbkjlrjd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gquwnuvji.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gihypjaak.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gmgjzbsdo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gsyqsbaks.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gvukaoxve.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gsshdcehl.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/ghwplwsyc.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gvjzbqmie.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gxcozgxqk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/giqzzydlx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gheyjapbr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjrdvkgew.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gexdmxwng.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gvwikjcfx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gfkbskftd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/godisiysw.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/ghditqkse.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gshqncmec.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gnlcjazuc.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gyzljqrma.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwsfxmeac.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/ghnkfuphi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gukuqcgzc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gknhaaavq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gzjbhsvip.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwwdniovl.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gukfotbun.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giumdsauy.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gnlqnpkwf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gesnxxqob.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/giclwiipt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gukacrmme.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gzlbcvjig.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gqydnxvlv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gbubyxxiz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/ggsunjpqh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gmewxxvae.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gjqoloela.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gkcnxspwm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gfupqcrtu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjyokdjqj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gzxdrnaxr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gfwtxjbfv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/ghvmzqudd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gfezqfbef.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghvpeziit.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gzpeucyfy.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/ggurovfwy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gfrdswsqv.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwccywgkk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/getmlrhqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvvzqgsum.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/giljhrizi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gkbonmudk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/guqvbpntl.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/grcgzboum.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gueidrsnx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gscqpjahh.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gudysedyp.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gshahxqpr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gkuqebkmg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gzguncotk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gxmaqaine.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gusdaljql.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gglcqmass.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gzzpxbari.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gmcxoqfwf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gjvzxojia.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gortkaady.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/guakonczx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gkpwcgumh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gffjltyjb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnnaytf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gimienkmf.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gbmbsriro.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gzaygpfup.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkwmamljo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gsplovhpl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gvjbvlzds.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gnwpupagh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gtqiczydy.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gdryvksiv.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gakcattyw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gykkkzujh.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gazvfljoa.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gvzldmnud.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gygrhwzdp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gkflleezq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gzbfvhoap.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gkxparuaw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gyxlafaom.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gdlsrzkxd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gfndcrelc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gootxjjmj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gibluxsmr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gakfceacu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gzwxcjzup.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gpiuxtvor.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gdkeltsnn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/ggcbmdpkr.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gjddlciod.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gfwdsorfg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/grdoujamt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gdwxlmcho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gkecfvzcd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gmfmxkhxt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gkeycxjwc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gekzsgqwy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gortqvvfb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/grhmerwmi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/ggmsvdpqw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gccaexnji.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gmsxnweac.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gombeofei.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gwxoorohj.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gavgjzwdf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gnppqaguh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/giugdkcdd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdxbpbfiv.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gufdcnbdi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtcoccqne.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/grtqlyrnq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ghpfzjhet.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gbzmjtzlk.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gjfbscsgm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gcjbffsvk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/glouazmeb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/golysrebx.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gmngggyye.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gtyniowvw.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gnaroebts.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gvxgofjqz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gnfchalbm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gbjajyotj.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gghkwvnkp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gsyydpcpg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gjlaqjtlz.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gtevuckeu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/giqgzohac.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gfjwggpec.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gcrkfwant.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/glfyygaqd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gwlkdgczt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gemombuny.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gbbkncqhk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gxueipcvb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/grerusfqc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gdpdmymjy.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/ghozizvpd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gjmrldhff.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvneqzqup.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gzjwjmeki.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gfesayova.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gzyggwibs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/grbuurqfd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/ghmpfsvsr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gxhomguoq.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gdljnulbp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gbmmgfvri.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvjfdpjjl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gafaflzkr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gatidgpog.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gitvgvpgu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gwfdjbtfc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/glvtrzxpv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gzitjmnmx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gdtpsfxvg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gpgpxzsiv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/glnaigqsr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gpwewnmgv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gxsvkozwt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gjikietyo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gkmwsupuo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gawwvebqm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gputnjvrj.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gnrvccldg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gkfplrjqx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/giunoqgca.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gjlprppug.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gdrojgmkl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gmnxhntnr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gsdlvynpn.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gnoermspz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/glvvoozlh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gqstvpksp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjmzytx.sHtML


<!-- 参考信息 -->