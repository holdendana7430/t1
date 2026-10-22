代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzvdrhfx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2akpjsvbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaipctcq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2stveclwi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iliqgtae.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gphxpjhi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vvrgfxyt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrmcjfnn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfegghon.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2honrbqux.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ubfmznip.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tfkwzkls.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fzftnnai.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jmggyttm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zgqfmdvk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixkmfbbe.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wuokoagp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itkzkjjp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zsuyqytq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlxambhs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alaqqqpc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yfqznzax.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2byjevjft.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ddvluqqf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bvpkwjbw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2icptveju.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2npanoyyw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dixtklsk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cmzrklwh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qafbmaad.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tfmpsihx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eybhbiie.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghuokmcz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qbagywko.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lssgsurn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxufmpvc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vrxrboaw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nfurvsnl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nvteyexq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dxfeodql.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ovucknrm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lepgiabw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuuxbpnn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpssvnwn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkwrxocu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2huzinvza.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gckpixul.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckfdeiof.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pmsjfrfi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2npirxkbd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rouhoykh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2womlqvpz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kvzvbkmr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apwwyqpl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hipooizi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpkrgpvc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hmgfnokg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xadrxiio.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gdmhslzp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vorhissv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dbvbywub.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2osundvzg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uutlycug.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2atbgmblb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2phliunpo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2infosxxk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ipahktsj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cxdqfgfc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rnelfbts.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gbofsrmd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ulwfyddi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2twsqymmz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uwxtoyvb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdtaudps.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmbibpvp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fjhseqac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sxvunxdx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2galgudad.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dbeuqhac.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2emdmiyps.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zyseqqrs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmkmuoua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hfknnbal.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hbnclnai.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jivgewcc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2obkbtysz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jafaclcu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uwluxcyn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wujvrshz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hlkqmxxx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2drfzbbvc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2siwynsas.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mpvvqorl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wbalnlhb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zecwtrpz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2edyhwgmk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pofsfdwr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rhxsovtd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gntqbofv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rkygitwg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zjmfszmn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wqfwfilo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wydfyvsw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sojkywzp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wzimpmmx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aiofbxqb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpbxhylg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceonphqw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hkvzttgc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sakfcdkg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dfzyqaaq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zxyhsola.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zzrizbxq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rgowtuwl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gqfbevwa.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2skxgwuor.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ogcjrzme.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gmgnrlrt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lchvkfxa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uhrwxoke.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xwqwdrxs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xjerjjrv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hxziukdi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kwzalsch.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pgswquio.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zslmccho.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tknhilig.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2synzlvuy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hxufzyhz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sxtadimw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2azlyuivv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtrksqid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2maonnlfc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rbcyrmow.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tgulmbgr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2akdgwopf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hnlfwioq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zjousedp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2igczasbd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mhlyjvdd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qvdnxrww.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yrawggzp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2waospirk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fwazcdgq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bwpfqzli.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ffqocvty.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2toigpawv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2harstsbb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wqqtvrhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cagrkmnq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lkzqcvhi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tgrihnss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jchgejht.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2usvdtlhr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2munlfkao.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlvepgod.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gpmmdyaw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2utccjigx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxcifta.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zkliyluq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qkiajyjf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rphyvbmr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bfgnkmlf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvxwfuf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gzludeit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2iaulgcgq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2czifqbdg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dmppvdkc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sxfrcwpi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kzutrodw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fqfnbvnp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bltftmkz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pgaiymyr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dwuunzhl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgfjhhu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ijhuxriv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nghimbok.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ltnljxcs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kexjfbnr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ltqidyre.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnebldli.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2esyiimdo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dptrbbhi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pdquivrk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjnsgojm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kirlwpnq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jhawmnfe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jcofcgcn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cjzouexd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwaswmfh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xenkpyaq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gyiwvljm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uvydrysm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hxagobet.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzxoak.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mczkgppb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mbcrjdwu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2icwvagfo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nyxfrcji.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2udhcvwsx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wuphriof.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wmlujcsb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ircnuloc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gwomcqch.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ivhamvnf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tpjtymzd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ilrlxpmy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vcxlwmrz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lmbxjnsn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2futctqus.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2omlpmovl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xvgkpwnc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ijtxpaah.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2bziequaz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2krolookp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kzzbtxag.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2arddqbrm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2vfkpsecu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2arnuluet.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wrxzygif.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jdmhhihu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hurptpzx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2nbmlmljf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lweyemtw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fobxoeok.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rfnghkoj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wtfyjgtz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnzxbffk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ezmrbcas.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vgyjasfy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2whnkpwnn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ghksqgzz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2sfnjgusk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfqmoku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2divsyozz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bahifkcs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2yrgfoxqz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fpbwwnvx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ionslobp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vobleszz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmnlbmgo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jzktqblh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aedesrjz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ymqkpbsk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ovsaverr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkbbizlh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stnlvoez.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2erwtsjbz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hfvjhiov.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otvsjvno.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sqrjylpr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wmsodfaz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2eyjdfoww.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fuidlfic.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2golqewvb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vzwhsiym.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ecbgvedo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2dpcandly.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mdjuobnk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kehkzngh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bpjqsoeb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ptkomgwh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zdtwreis.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eqyfpzzr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2divvygzg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bitzcbam.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2erqeemwp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2faxmurbc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kalmkgxb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2iiuibjzs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fiioizky.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ecchrigd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2obwghhph.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mmyrrrda.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vvotkkbq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vrebhfup.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xssjgrib.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rdahjeia.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oandusuu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2gfngxwff.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xbpktnwh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yshhnvgd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2owugltxk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vfsrmifj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wzjmmlhs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dudegggw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzcsmdsl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2hwrljjcg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2feppkglv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bujoyqqe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2zmetxkek.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qzzetmkk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ugsrprrj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mzlrdcav.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2mlbnvbfu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jknlxcjc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xyghdhka.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2obnuwgxu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2qezrrzeu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2glapjspy.html


<!-- 参考信息 -->