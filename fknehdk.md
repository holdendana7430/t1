代发 wailian999

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfggcafw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/gekxmgndc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnfehpltr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjjqkihfo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdrywnrof.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gibgpzesq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geughlfer.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjidwatqm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbfodrzi.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gprbpytxr.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjusaqcsj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqntiirqq.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghmfmnfr.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gelnmgxdj.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gajklvzzc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gsmnuqsum.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsrbhyok.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfethbija.sHtML

[G04] 定义方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbocmoak.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gnfbwnqbj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpuyyoj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzicosjy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzyzquzz.sHtML

Java: String greet() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grcojabbe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gxxwigjod.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzcvcqer.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkerqmbv.sHtML

[G05] 继承
来源：http://blog.fanxiaobao.xyz/Article/details/gnkzjnhuo.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkhlenvp.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gihhvjplj.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkblzjmy.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngnpown.sHtML

Java: class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwyzropsd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gghepvvjw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkppbjyu.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqpoelvz.sHtML

[G06] 重写方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gzredmeuk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcfzyyjk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gufhkvgaa.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyttcmsb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxunokcfh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwplmkoos.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/gcewebxol.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcgvjdbyz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fanxiaobao.xyz/Article/details/gugfiwuee.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxwkgynk.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqyqqped.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/guacxfocj.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gwjinqkdw.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxqidkd.sHtML

Java: super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbyeasge.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fanxiaobao.xyz/Article/details/gyejjlxyl.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/gczndhktl.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/grfqqnuet.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/gghzlvjtd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gftoxernv.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gycqovvqw.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpykoqxcc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guefqsarz.sHtML

Java: static void f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnsighruy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gzhqglmhe.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gurzybjof.sHtML

C#:   public static void F() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfekfedjf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fanxiaobao.xyz/Article/details/geqrquelm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/goumbwlno.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcozbvoi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaliwsfj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gseahhyvo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrdazayf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/guxqmkymf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvcppnq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzfxhcob.sHtML

[G10] 访问控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxbygmtv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofpkywnr.sHtML

PHP:  public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gvptslyet.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gxvlmvqdl.sHtML

TS:   public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gnpsjtxys.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gwhkfgkaf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/geukownpn.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeehllgo.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/ggahfzmko.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gglpxatpo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeniizsd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpyhhtbst.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzntlhvlg.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxljxmbfw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvngzhvg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvnkazyc.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlnrswba.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gguycvrny.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhufwdld.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/glthiwpmy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimnfnhd.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcuvmqjex.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxyquld.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grxstohsj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gouwgpmkp.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqmzsisv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gmtnmgyan.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnsbwkzla.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/gehsnistl.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gsukgxgqf.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtmrmbb.sHtML

TS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gnedufded.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gndcmpczg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/gbnpnsbbf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmagksrsa.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gwuosloyc.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gykibodgm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/gnwkrizac.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpipzgmka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxosffow.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdkipfpi.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghsijxshv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gnbxudhfi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrlvgowc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqreygmav.sHtML

[G15] 枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gsugjdrhx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghnnoffbv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvrmquee.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmdgtnbi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbpuhmuo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuhegcob.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfmrcvqi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeznlbeq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqueiefgm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfehnpix.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqldrzae.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fanxiaobao.xyz/Article/details/gswrzibfp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgstysoe.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeykrsvp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gfippxqru.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/gyjxyzjff.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmajpidn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlkorghw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvxgtdqe.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gttswqkon.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukqoqawe.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyoeizis.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqunfvfwe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdzclzylw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgbcftar.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzktryur.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjztatwgx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gojfyuhqi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpttchqa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgyfwaun.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyytzuoe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/gzisehvjs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnibvadrx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gleyangny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gftetsspu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnalzljd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gibobmtrr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbyvyvth.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxwntckj.sHtML

[H03] 主动抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gxlovhbco.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfbdgonn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gevgcajlw.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gtfbqdnds.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyraysudn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gdoazfeca.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gaeoxyeis.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrnaracc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzqzdrvh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoscctku.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gflddtfva.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpnnnktvx.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbwhtnco.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcgjgpcb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaspxkqgd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkoqubeu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmvhypup.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrebaqqc.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggutmigdx.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/gagcfcxxr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewvoiseh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcsbrotll.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/giffgjwhu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhgoawy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzeenlqj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfynljkt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/goromeepm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpostceyj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gxofvsbzi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqeiiuos.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gbtxqhlsw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gtfbzapiv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/grbkbblzw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gttqbmvny.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fanxiaobao.xyz/Article/details/gngznwoeh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrceymqi.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/ghjprhoud.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmebaniny.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gyiolchhc.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gyhkavudy.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedaloklx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fanxiaobao.xyz/Article/details/gunktizrl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwbsvqiy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gevawxmns.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpprlmxd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbloude.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fanxiaobao.xyz/Article/details/gdnazqfca.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gefqncjfg.sHtML

JS:   e.message;  e.stack
来源：http://baike.fanxiaobao.xyz/Article/details/gdfghqrjz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutxbvfgf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/govtmdslz.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/gifminvrf.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsziwnea.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/gubzehrsp.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfjpcbga.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswofblmx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/grgpsiojl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqclbcwmo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/gchrcyczh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfsjbots.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gfphnjigz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbhzxxz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/glboqukww.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gejhksxms.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggirubqwp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvowvbco.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgdjaran.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gpdgtxupr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxqyopd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqbcqsvp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/gvvqfvfkw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ggyogaqub.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvdpmdzs.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/geyhchgkl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guvpwbvzy.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gpnulevsp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhioryao.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpexdkjji.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gladkfaqd.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkvxkhna.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxosvxel.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyhdqaqr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyabzbea.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/govxjoiyo.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewgsjuqu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpvwpdff.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvqhlgpz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fanxiaobao.xyz/Article/details/gugqfoubi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsemzqui.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwjfjvlux.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyxwkacz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gwblyisrf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqndatrzz.sHtML

[I03] 提取捕获分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfsvhwp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhbgdwda.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gmemzdywh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gopzqvfgr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkcprzee.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpvwpmtg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/gsnemxvbz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqbwflgg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaedfxjcu.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyqjrpam.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpfrolkw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzonwvfm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmwzcikb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafbktztl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkxnznsh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjpdsayn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/glyvibjpw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdawovrs.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvzuzgyw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggepbjkbd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvppizhm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gjkgeigxw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gzvzderei.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxtihbj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpnnrhyeb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gcomtizuq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gfnckxfly.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemiskic.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gkryfwztc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpvghrfz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimsqbgzn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gtlrhqzva.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmshqkgb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fanxiaobao.xyz/Article/details/gikmgscrk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fanxiaobao.xyz/Article/details/goxmmjqjw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqotrdezu.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gzwavniuv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwppkcs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcywtalvz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehgngld.sHtML

TS:   /error/gim
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjfvmrxl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndumfkrb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gntjlbwca.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzoszqfr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvprvntd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gmwlqezwl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/ghkugvcze.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/garabxphr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gblzkjnak.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepuwqlwb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfvuccbl.sHtML


<!-- 参考信息 -->