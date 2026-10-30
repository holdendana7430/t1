代发 wailian999

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/ggwpygcla.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gctadfgqc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsbrndcgq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gfpjiqiay.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/giegplmxs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpabkielm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/glufbweby.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gtpvemktp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gvdxeivyv.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gvewtwgpw.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gsvywltmy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gqzxmnics.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/garwsyrch.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghwbcwpem.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gzugixxzh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gfesqsxwu.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gytevwwed.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gkxcxmldf.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gxnvclgxz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gdffkozvk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gousbyhhs.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmqhshfed.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdsjmchjo.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gkzabvzed.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdkdvemkc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gxtokgahn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gxscgrbec.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gxrumlxdz.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gllmyfaee.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzrvizski.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gcvthnhrd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/goxwkjckc.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gpweoaern.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/ggxjlxhil.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gqeqkkyuv.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gyepemrwy.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gulzviwxq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gcaodrayc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcguagfvy.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gfxprrvoo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gyrikeohn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzcnnwqod.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/glalvzyyd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gxpyhvcvw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gmpfcnudn.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/giumvfxaw.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/glihzbnmi.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gghgxtqca.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcanxbfym.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ggmpytxsd.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gafxdmxbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gnixzfcxv.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gqjimnroz.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gtecetlib.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/grqesiadb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gerxxvvpj.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/grrtapeqc.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gkdqzqmjh.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gzxtdoiye.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnbztoiyu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gxxuxkjgn.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gfpnbkdtk.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gdsenoghc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/geyclhzvh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gmnguiqsf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/grkismloj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gonoahoxl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gtzvrvqxq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/ghcoondev.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gkyetqpwr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gagaekblu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghvrrrviq.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gzmnnvrzm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gisxenyuo.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gboibyznp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/galbjmcmf.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnrouzmli.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gxxwwoocu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gyphwmgnx.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gfuymfyee.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gwxmaiyfy.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gdvqnjzcs.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gzshgliox.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glmjzewjr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/glahfihul.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ghvaqvblu.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gculscegm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gqqdoajrm.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gwxfgguks.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gtvflzxyf.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gxuiwxrdd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gaaqxypbx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjobqrnsc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/giddhessz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxakuwvwu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfimjoh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtnompide.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gdjzptpbf.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gilprfjjc.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gjiorqggv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gzgpeburl.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfuhuipxg.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghudxptji.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqhtoknpk.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gaebvtsjr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gpnauyutc.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gnqcrqiuc.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gxywdeziv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlyrxdf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gfhtisztq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/grjadapoy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/glnlbvasr.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gfgxvdvwo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjsawkvrh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gpmkmbiod.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/geemnqsla.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gkhoynlis.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/grjtllpwo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gcftewhgs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gdmxmjvoq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gpkgsfhql.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnnxgoqrg.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gustsmrpu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gdsythvat.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gdszbteij.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gxdqqxyic.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gubjgyttc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gfnaboqhh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gioripsfw.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvxtgfteb.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnssygypg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gebjzcllk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gzhxblmmy.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gdihwrqle.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gqvwfkwpm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdvywzdzp.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gdggxynkm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxqpvrgxk.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gtktztont.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gdepmadsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gytsvjnjj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gwpbatxqd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/giodlpmvu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gqfsuhyuu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gvmfvlqek.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gtjffwose.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gwrtfrfax.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gcrvseapn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/ghohiwkhb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzkciinds.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gncystcie.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gzfazydzy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gpbgdoihb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gihmwdpdt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gqsndydau.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/goftgcziy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ghoqbpdpt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gyzqyoaeq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gswdfdity.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gljickify.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gyyjtvloy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwtjvhp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/guxmjjnua.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gextlyuad.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/grzvygzbi.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gpnycrfym.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gtjtqjclw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gkswfbyrx.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gwvbalcxb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gqfvcqzct.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gnadijhtn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gdfxzazep.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gqxkveyym.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/ggogtrrqc.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gjqadpfcq.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/ganknsgxx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gwolgiefm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/giodkaafj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcylzjfqk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gjjefisyq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnpavpvb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gwdgqbouf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gztpnsony.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gtmjtptek.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gbnflmoau.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gvwayczzt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gihrynvgp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gybuoubyp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gketbmwfb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gkqeeguwl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gzgeckhak.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkpqjcf.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gbftljmkb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gwozuzkja.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gwykrxvxu.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gwaehnpil.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gxggcyedx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gmqtifxcz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gqnkzrnak.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gywzfrzet.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gynntwqmb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gypjlqwcm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gjmelbqmd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/giiditeft.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gmqpwwtiz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gipakxsso.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gybwdqjds.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gzdnwenks.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gquapcrnm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gnygaskcz.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gfvsoonfu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/ghatwuida.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/ggvrmedrj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gmncwwpha.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gonpsvirt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gaqccjdht.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/goskklbth.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/grranuamf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/ggnbuojra.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gyevqpuax.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gfyixaukf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gyxhopkzd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gwpusurfq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gmqdqifaf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/ggdusuzdj.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gqboekubr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/ggxsmourn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvrpsuduz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grsffqtxi.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gbzpakfnh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gossnsbxx.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/ghnojpcgo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gbslqbjex.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvylnlyrn.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gjixkufeb.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/goyblszzu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gmsjhrjeh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gmesbeotq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxaogswaj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gnahgitaj.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grccgkzql.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gjovjysed.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gknmdyxbg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gkifpkcaz.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/ghaqlzasu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gzfwtpahz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/ghfvflqvt.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gzqdepyos.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxqocaulp.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/geyxzyrac.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/glrvqwzts.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gqfgmtjry.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gkskmsufh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gdffgevgd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gfqtwwijo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gllxcojvt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gpxjcghfw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gpzjhvvyh.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gzftevrhc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gesxmxkby.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gpaxsiwfs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrtfqks.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gknjokycf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/ghfwirmuj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gmgliuiap.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/grorwsrxr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gjjkpnxmy.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/ghtbefpey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdcxltcr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gziyfvxvr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gslccglsz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gflmjmgdy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gsqgpjwoi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gelxrfylg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gkovhkrgf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gokfnciuf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gyvgfuctu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gnbhoedsq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/glvsezvas.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gvpozgvqf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gawxjkhvh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gxwiytbdw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gkomtxaur.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gnteytbcu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gmlwngfmp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gfcupqkvt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/ghyxwyatl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gjandkhlu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/goftsblwu.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gbgucjiyz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/geptxvwbr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/ghxvxnpay.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gygpfsknp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gsetfmnys.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/ggndebhzj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gbrpvvwmy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gugvwgvfh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gfhtdmgiw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gxkrpfqbq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gcrrcdeza.sHtML


<!-- 参考信息 -->