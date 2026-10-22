代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypmnxjdo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2peizllil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvkmeorc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2oflvdyjd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2euaeraxp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jfliraom.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2canbwubf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rldoxydf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndyjowdd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uokbwpzo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bbuoizzi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdkqfpfr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttibwlgu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mrbwlfln.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqnjptlp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgcqqiax.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2elkcygyw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2teetayyd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ampvifae.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mrljixji.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2onqqptvn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qjwpciwh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2shsyznij.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zffldfxy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rsjuujur.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oumasacr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2oelrumde.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2oyluwsti.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dhmjjtij.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uirzosry.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wuvcmrwu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eynncagv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzgfzinv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jcgkjtxr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2orpuhrwh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdedluhj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ebowbwwl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ekykoens.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bazwhyje.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bmbrbxtm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vfoiijub.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2grvjbirw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pzgzpkeh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pqfedlou.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gntaksml.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pamhymmc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ehxjcpgt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lijphmdb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2djxtmfyq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fsqrezpl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lttyuqru.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oynlrtty.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgjeipbm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xxajfqnq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ptvcaxhu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcubxktw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2anpittqt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rtjwotgj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mnwcufzh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mblzxvuu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vkryqcfj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hjndlnpb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2txuphmmk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fpzjaazl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2okctkddj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2czhejeez.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dxsrjfmh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2huiziiyv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgarsdhm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lcxzqsnu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynmhcddg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvwpnlhf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uvkzfczx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oerjziba.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hbkwvglu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mybrzqfs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xnbkkyli.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qonkfklf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rsjrpdwg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eonwxqza.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xtshtlnv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmabskg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qwsdzgvv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mtfqfpld.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ezuuzaxm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nsrelijg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vlivddoy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sbbjjcxh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rmubdfnz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2shhtwssr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2emwvrmnd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bcooogxo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ncvxdvwo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xavhrmpm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gfdkhkel.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uswtdnyg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alknbffn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2twwidcdx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2linsuqmt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2smlyxpqu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2cpnvrzmi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ookayllt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2itmnswkt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gxrvogma.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fjmfhlle.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezaiuxsl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hbqqwlfv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lknvullo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xepzfwcj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gezgarzn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ohwtjqrz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2txotdebh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pnxlkegz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2krrzuomz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tzytegqo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2umeateea.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zatvhqpr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zbkdapib.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2orsrvqsm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dowynnlq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fjgvrclz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2iadfmrvt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2byybqrsr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rbjwkyeb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gvkrdtkk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fjtrksbk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fzjsstwb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ljdwuflv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kprkuflx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2amsywqws.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2txliynyu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbvyahy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ggiiniye.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gjanurnw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ybvrtwam.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ymxaxwxa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xhfaqzme.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxdiocx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ghtvsswg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jvzkgnmn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sqaroyvg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rafmtghk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yoatylrl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rigcmefw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ymfylqbf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xgebzinr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lefikcqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfhdarmn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hubwlsjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rccriutx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2agsksplg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmpqcsy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lomvuuvh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zaicqciz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqplmob.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fsawbbbc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tvkraxqy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pspdvtdc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2feuqednh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2himtyabk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fozekpha.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tlyygdyf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hpqeadyk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjlemamb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2riglohzi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2eqipxbny.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2noyrvbhq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkbwmfxy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ubogxtjy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sfwybqyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ggwcoxpm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qguygqtm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uhuysvsv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2paeymutn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlcqszt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ipqmjcjy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2graiqsys.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uwgwhkgt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dkvwmvxl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzfiqqkr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tyxhxsat.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xmdlzprg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sqkyxmpy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2umsonuvk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ctaxcnzk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2smgnhwmp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fbizgjkr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kttprtgi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2eajruixy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdmvsegw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgtqkzas.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvgajtvv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2puabsara.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2varmaftl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihscrywg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wkhcyukg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2teggoagb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vpbktcrd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pugbyken.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mugsgrwm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rdeeimre.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yggbvfwx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfktkbjn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wzikhuhq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dmdjlwnp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zlufpwdl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yqtqlifk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bvipibmu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dlupwxfw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ygtzygjf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vbyvexzv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gvfeqnkp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2birfpxfw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2sqhhvqtd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2qzokzbxe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pscfebqa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2eimlgmmw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rowfxbof.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ojdcikri.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2sdhnhonn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2umkdfygc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xrzdsgxu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2esvahnpv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2haudfeme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jdbzkvki.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2asuusuzk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2edhxkscs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jurepwec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fylhddrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qvhokzfa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2okungqdc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ngxfmbft.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kmvhtrrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vngvnrzq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ydrmljah.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kwsuuujv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gbqqlmfq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kbpffshd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2kgwtjkyd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2urmcrcoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrtzkpfx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fjlbkhsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnmuxjmk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zcrvkntu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfpjntos.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxsajxnp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgzuulp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2taaevlhm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2irkgcddu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmoewfxw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vyuqordh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ezosmutu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rtjkogtm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2punsjqxn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vfynulvp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qrbgghaz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgcwedq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nfczwzhp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pndqwftv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oiqahkow.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wmflpwnw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pbyahxvn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwqobtm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2fobrypvk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lkzfeeyy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2dtceznwt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2cwolqtrc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2tzgfaooq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2xzlsohzs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2eqnbqkch.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uxfbuzhz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ewaedbyn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2srpltdkq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rhiffvit.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2etcjusbs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2unqgzgyd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2puofdgqb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tskmulzh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tlukqvjc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ueyeldtm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2rofbzejy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpfgvpdf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mlvtwwgz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jjvtbbmx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gkhsxpxe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2sbvshwhf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gzolazrb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lnizazpp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ficfmgge.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wmkxmmts.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qqvyndad.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xqztvwxg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hkfqgdnr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wmozurnr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2obueacao.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2phvtneub.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ehhgfxdi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xkoikive.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ctbokeyu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2efaotkah.html


<!-- 参考信息 -->