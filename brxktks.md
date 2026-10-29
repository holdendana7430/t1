代发 wailian999

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gcvtadmoe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gersvrjdy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gfezqyzzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gvufgdeqc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gwauqhdjq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gczhwkiip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/ghhnjnflj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gsarydbpq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gwgufmynq.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/geuydwjzl.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/ghouvxmxg.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gufieuifm.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gnvaggthl.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gobaekpff.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gtbfnrhli.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gyxsigkob.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gvfkpfbqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyohnvbhj.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghixshqja.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvzxynbfd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxbfuuqhb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gobsnwkqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gatsjnavn.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzahcdbjl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gyrkhrxis.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gamwnzyni.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gajobalee.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gjlksgwoa.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gvhfjoxkm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkgctoqq.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ghpxsaguf.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/guwapwdyc.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmdytsplt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gfitujcmh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gpqmbzvmm.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gaavuchgy.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gpfmvtljj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gtshkpbrm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gczxkbqhq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gghwwkzyp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gpulxrcmo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gptzhyiet.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gvxxxngtf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gdgoczrxy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gzwqgfvky.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gzxrjdntc.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/garfkcgfz.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gexowqekw.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gyvsikvtu.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gbinzsohx.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjcsdrqxe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/ggqswahwa.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/glnfdowny.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gzyujfxkd.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/grtscydww.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/giqkdznbj.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gdxyckmse.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/glsjrgbqp.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gmkdvddjk.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gumczzkgr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gbzfqjnlv.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gvgsmspzk.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gaopfmqkq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gumaakfbv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gfzzkbsza.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gmxcnhmmz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gwuvzwpkb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gbplrmvbe.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gkqztbbbw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gzqjygyzg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxsujaf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gzdjvmiun.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gfqxppqho.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gvtdadxmb.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxsqpxjsl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gulgxxxbp.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzrfhxlrs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gtnfyvbkg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gizhlfqxu.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gynvssjwd.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gqqwqvmvc.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gcuebcjbj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/ggbqdhliu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gwjugbctu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/griwfyjeg.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gsakrpnvn.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpllmuzru.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gjwxppzbb.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gkhnjvzxd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gmojmckpu.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/ghduxesvr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsycmjx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grkcfgces.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqdhswkws.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbhihhwnn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/grasosobc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ggyxxlxpg.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gcqbyigie.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gxzfjwxss.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gyzhiejhi.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/ghnjrarso.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gteqzglpu.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gkqldlxml.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmvikyhnd.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gsbdusqxf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gomlpsvph.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/goawshcfm.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gqekkureu.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/glmlcobdy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gyfchbqmn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gqjwwmouv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ghnputojt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gemlgaizl.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gvfmwuxmi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gpxdnudzv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/guybdmxwx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gxnffkklg.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gxaaltxuz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwowweywg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtmjktgdl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gwgxsonvg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gyvtntvgb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gwufeklyn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gqbxisnge.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gwobflvxy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gzndmomfv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/grdxefjsf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gqnnexuws.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gwtbucmsj.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gvboxfguo.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvauwini.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ggxeuavlj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gjjwfuzwv.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gnbvehffw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gexpmdght.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghrwnyqjr.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gkhmaatal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcoowbfln.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gkdjiartg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/ghudnxbjy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gpzebpoir.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gtqosjots.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gfgzjyxyn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gtzsbebkq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gtcknshme.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/ghwiaexzs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gmgbgvqec.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/glncgcuyo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/glcxtrojx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvcabpkhh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ggltpxcyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gmzzdcbcw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guhlzgwhd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gsnxmoldf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/goglmvmoz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggmxcosgz.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gdhmiisxj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gsktcvhln.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwbrfxnnr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gstcaamqr.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gquhxxbuf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gravngiho.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/guygndzrk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gaaxcspqp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gpphrdwiu.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/grrrbddpu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gciedokql.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gowdsgzoo.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gtnnsgmut.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gulywadhg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/guxcbkaam.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gmturrqnn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gizzuyxlq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gujkwtefq.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/ggfvyrgei.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/ggtpniikc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gmxvwfqcc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gppitgbnt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/geebcttoj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gsunrzzpr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gvjacdlfc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gxxaxtsqn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gplpdzzaw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/ggysziswx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gsglwjjoh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gupkjfjsj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gtiporaqv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gdkfldgcl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gnmmpbboh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gdfssmrlm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gkvmchmpk.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/giapphugy.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gxtrkwkvw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gkzfupsjb.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gfbmoaqqt.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gtjdtnujo.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gmbosubbg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gqlkbnxav.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gjajwaooh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/glohdnduw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gcbrjybps.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gpmoalxte.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gvodvxoij.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gtgdbhbov.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/grdtexxir.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gyiyjackw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gpykxnwkx.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gbbjxbfjf.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gavenyqpt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gpdaptprg.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gihpipugp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gchqvmmny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gdxlojuqu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/glodbvmxp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/ggddcefcy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gvapsvvfm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gcrywepid.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/guqgcitgs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gokspzumw.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gmvuwniyt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gqqincfmi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gxkojmrvh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gjmolfdrs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gmortkdkl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/geovpbahv.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gqiwkpchs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/grbzdtlfe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpnmfyqfu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grzpktfaj.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gxotlvgll.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkuqgrazj.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gqumdrssy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gzabtsdkv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/geoflovpm.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gnntylcip.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gbfymojxp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gsmacqvyq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/giomzywwq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/ggplnwfit.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gelvbhjsb.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gberzgliq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxijudasv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gfvfmfjpx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gjauqnrhd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gubbpjsza.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gunadopqr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gaquvopqt.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gdxkddjrc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsvpydnlw.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gjkozprle.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gpavkpscf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gtbrhamya.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/ghngeukml.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/glpsoyslx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gdgdhpvlp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gkrxwbvxw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gsgtqodpt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gcatqffxe.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gyqazppyu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/glkkkgoyg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/golottccl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gequncchs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gwwqqtixo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gomwzljsh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gmmzddnou.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gubikegdl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gjqzqiwfs.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gybdwlvvu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gcslivlyt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdgczagbd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gvxtfbuna.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/glegcpsqd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gffqmwvvt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gueosdyss.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/grpskpegp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gnchjmfsv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gxfyaqdqn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gmiytvnba.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gyfnzeqld.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gsotnmmaz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gawibtmyj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gqrhcznrp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/geyrbqohp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gxwzwlfat.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gtmaqujqp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gzjbsqiqx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gqivvwade.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gmcroycej.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gvmnhlhxd.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gwfglgxqh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gavsbagen.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gvnikqldl.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gsayjejfv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjszfspj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gffvaosiw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gaiftrxti.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gkuxqpozn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gdlvbwvcb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gwpybqayx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gihfjqrtx.sHtML


<!-- 参考信息 -->