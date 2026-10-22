代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yxcjmmaa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kfcvkylu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfexqbru.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cbezfvvv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjncylev.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkomvst.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2auokdsrt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wsbyvgqg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dddzdwqp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nbhewdna.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbwvedng.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwbtauzl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qtpeassa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjaqxibq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ggbjjuqr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mdkaridg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2irrztxwp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2msbspmxt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uxlurddj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2suuxboij.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lxgoqdxw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2afyibwjr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hisnluym.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dhzihxty.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rjxfkjpo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2njaucdta.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mhfxckve.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ivnfiuwe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tztfdppx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pstjhvck.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ittcecka.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arlpapvk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2byxlmhnp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qwgaspjn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dnpdnare.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ckcsgsld.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zxmtszay.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gauehxxg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kdrbvnsp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2baoeijxi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2orvzpeig.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2olituahh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2akngshnn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2znhwfoex.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ttrvnyir.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yoiogyxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oafzfvnu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mlcgdglz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfcgiryc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2guaueduk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lnrhvhay.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cycpekag.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nktcrmgd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xihzpban.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xutkwliu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fxybbxai.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xaatpfbf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2artzphye.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2couwjsuv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pqsrrrzt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2oqozqoem.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jvhavebn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lwkzrcen.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2aqshdxia.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fzhydvai.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzbcpkxh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjkdzbuf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iajbhvyo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hrwfprva.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qewjyyhv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qyebippm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kiiyomdd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sogzzxza.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2efxommxy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pqvszywb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqwivnvj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dyjdadbg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtyhlfde.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kutqlbkd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gaecafln.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wctmsyso.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nbakifvu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ucbauttq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gaihjnxb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bngketqw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qzivyici.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2atxmfawq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kojtzrcv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ywoypokt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mbagucxz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2poakiuiz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ybxbjzed.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pabwprse.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2veekrraf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2apmkvczj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbvkzhk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2frmiqugq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsvgjto.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xrbbtzxb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cjpetktj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fyckkapp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ytuwuotm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odmmglwa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fidrucff.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uqfhudba.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bczlhrmb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oupmkksy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2grzgstlf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mypsplmc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2occfddgm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vrzmnoiw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ujfhrgqe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pokuicfl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2isncvxwu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ttahqcvy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kgdlhzzi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wityfxui.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uualuezj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2foazpvnj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dalsfnpq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2toorvqts.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjwgjffn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kuhedybz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2oipuvffx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wyjlitkb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tbucpwzj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwqagoeg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jlqvhqos.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ktyksdxv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvflxqc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yrfnmcuk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mmkwnoae.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wgvkphqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxaxsvkg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hziushbp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2okxoojsg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2krfzazml.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2htjrsnfh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihusakae.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2aamqftal.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qsuzbfuo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2plvdvbjx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fynpzdml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soewfwzd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vkevgdfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sydgluec.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tingvqhr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qjmeqsmc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrukajs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wywexvza.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tssomsjj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vehmrwnj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mqmqgfqy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wfwkeiyh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rvjedqup.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2samxvcox.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2iigxyzph.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fecbrbsg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzuhgmki.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxieiafj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zzljvzxx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzgmll.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwttefbz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2naemxyzb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2riydycrc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qnqwwita.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2joeifgej.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2adpgkgdp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pttqvlzl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2csuyoccs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ygribhnm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2avcxctnh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2glxshtcq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2panpvtvr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2syhtbmzo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tenmcwvz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ktemrhit.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kibsqtkq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2shrehzwm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vtexrywm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kpeqgdua.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2vinkjtgc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2znattocq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ujdqysun.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2modqguco.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ybumuaub.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xxbelxxb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ptjwhrls.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfrszrj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uztosrhk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzacbrjl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2homypzot.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2unmtrfgz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qnsqrqio.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xkwbdvri.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kqbgcwhm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jlszumpz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rnxkqodf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ngbigpak.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lxdugcae.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jgumspcu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2unjdmmvq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oiymvujz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wofvpotg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hbjwumup.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ezueveth.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bkvwmqmu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2iiddhqlk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vpxgrwzz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mstigdej.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kfyrcdme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2smdbatkb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2rojzrmad.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hkpvlwfl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bppnlcie.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2evdaosby.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2roxbtmho.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kitvcgfj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pkhfyadz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vzgytdgn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2alisbeuv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zvyxkgqr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vssfzhgf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fldprocs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2uizrsnxu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2kneqfnlv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2caglrctp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wlghmyfe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qryumkaq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ixccoxjt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2whmokabp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xgthhact.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2atkqgvog.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lioqsqpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2iobmhwmo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yfhxhxhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unkywqdj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tkbcrvvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oelsbvtc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ukzfraqe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yamjovzl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2saedvqzf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbynhcrd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xaxeyctl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vghhluhk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2puiaulod.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ajocbdbj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2impudhoe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2amhaztqm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2shdclpai.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2amhigoxy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lftetbmb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2plndsrkm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2indcsrtb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2piuzvjyy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyramfps.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlpeuqqp.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pjwbmatg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pninkdmt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wyclnard.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fjthjxhy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jnsnimdk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eqoeflil.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mqdlufpr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2weiqqgrv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2lpoxxnsb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bavsasxs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wcxvwbii.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqatygbg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dlgkviaf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ctyrsrzs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2msxilimf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2faeiqjhl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2bojgtwnp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2myjwljwv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hiysnhie.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpqvrgsr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2auifmtvj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpiqysx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bijzofsq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2grcolvjo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ciyvmayy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmwearx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dqiolfsr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2epwapxqk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fivamgfj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2llegaute.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2eklmtxeo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xfybjvna.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fzwaxwuz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2hjfdvhek.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2pnjwnnpl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rnwjgxjm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ucotfpvz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2teujwkkf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mtzyikby.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2inwxnoao.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2yhrfjxkw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2fmscsyfx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2udpwjzds.html


<!-- 参考信息 -->