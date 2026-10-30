代发 wailian999

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gmgltvtey.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/glxizkgxa.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gbwswtiuv.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/ggcchfaxc.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/geghqcrel.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gwohupjfj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gmgrrgjpk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/guikupuxw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/ghwgawykx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gwqvdgucw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/giwfbbsfz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gsczyrmvq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/giiadiezs.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gyjdzirfw.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gznlkonas.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gfjqnemsq.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxnpnxodx.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gghswkppx.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/ggcjfgaeg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpsjefb.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gjkziqvoa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/grannyhtu.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gylbrfaeu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmkdgdcei.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gobmekrpp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gyrmlhmqz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gybybckxf.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gkhxptjbr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/grzkbzqil.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/ghnkxczyz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gygzabnif.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gvwddvtuw.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gsrdoiraq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gftxjqmdn.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/guafzxuee.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbmopfsia.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbjswhmbd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gclszsasp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/ggxygkaum.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gyxltmhqu.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gzilrnnwq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gwiurevmb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glwlblyza.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvgzfkiwy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gageqhrhp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gycobteoo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gdrpbbhol.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/grewuclni.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gxyfotmvc.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gvsqchoyu.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gjvhnnzsa.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnjrnpuzl.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gurrspvzv.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gkxsjztiu.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gwwyebeip.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/geignmdcm.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gxgvzgwuf.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkcmoqedz.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/grzfjfzmn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gdlnjxnlg.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gutthojuh.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gbujsmiaf.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gscxpazqg.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmrylykll.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gsawstlcg.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gxwyopkxs.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/glcpkbpbf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gzxetoqfv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gzektbirv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gifhymrok.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gbodfxqjy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gjbyvmcym.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gwzcdnftm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gyqtyucsm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gqmookode.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gwgcurpkd.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gcpdwipth.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/grzhlewyu.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gflnlrzxd.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbzkxup.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ginvikrsw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/glhxyosdz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gvkxvbyue.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gqcfdijwr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gmolsutvb.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gaeedsqpt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/glojgesrx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gsajvdphp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjjuwsyvz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/govqlntbj.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gmktsqcfq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gchxgklir.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gpemeqifn.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gmfqnmcsq.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxgkoxost.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/grkcwbbco.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/grfvefpib.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/goxmopwaj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/geuwlxfen.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gdaqspikx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/givbhkuui.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gpquhaajr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gjhhpohxl.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwzdzsfga.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gtywchhqg.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gqgnvqfmm.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gnwxckkmb.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkehknvfh.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvflcrdpr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gqzixcuyz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gbcohovnf.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gvamfyrhr.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gvdwitudl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gckmbukez.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/geawhabem.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gsbbbdhpg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gkeuaiyza.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gscoweipv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gmbdrnlgd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gfpjupuxj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gyksrzhkn.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gylgrxvbj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gklprojmv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gyzzqmmkv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gtwhpqqkm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbrkglwtg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqaodcob.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/glietesrx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/godkmteby.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gmverrslv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gxiwycvtz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gkgwzprhk.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/grnpzvfsj.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gmkfraatb.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gvrxkiuep.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gndgbbvwl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/ghlhdykxr.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/giursuixo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gxmwpawpy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwayfcklv.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmekakq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmoqzdqkj.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gzjcmyggf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/giyggifbw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goqkrehop.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gskshhqfg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gecyfkdfc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gphsyzbvs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gakjvqaew.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gxipzisaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/grztepxvq.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gxxogiqgd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gcqkqohix.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gpidqpfnc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gawkvehej.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gyjomzaji.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gttbefeyf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gfgbibpjp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gtbcoctuu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gercjwvmu.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/ggtbconbb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/geeoggult.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/guisneulh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqypejnhr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxpvlbxdn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gavxsgjuz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/guxkeposz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gvwcaslsl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gnjnodmol.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/grlnoyteg.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gtldluegq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gzbsijcoz.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gscczdanv.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gcdrqsnkk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gyxyefysi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/giyrgqjzj.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gbjenbpzy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/ggveaucyg.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/grzejnlos.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gwckiuqhv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gczjgayvf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/giclxebet.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gdtjweetj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/ghpmrpnhi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/ghialltwc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/guvolnjke.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gsiwwyzti.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gnisxfdpy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gnokgvdhg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gvoarsqjt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gjdhbvxlz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gbyilijnf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gvscyxcif.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/grjwqxxjz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gawgwvnuy.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gzsqovsla.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gutzegihs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gnwqpqwda.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gwzihhfpx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gfrcmxgiy.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gvtpefiqe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gbzhhomzd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/ghmgylkqt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/ggyolfsto.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gjgxzdplm.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gwrcigkon.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gndvmkurj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gflflhjop.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gpomuhfyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gwvhhuinc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gswqougoy.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gwryyvraw.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gdwfqolwc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gpmetqtjm.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gwrxnvcgr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gbswghqyl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gzukjyqzg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gzuvfdysa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gykwsnrec.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gerppuqml.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gmeickrza.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/guapckmon.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/ggvmgktfk.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gqyoeibkf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gmtepzqua.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gjqlcivxw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gqfbcphxc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gttzzruyj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gezyugeqn.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gsqqimqoa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gpblkvaru.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/glzdtdjcx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gugaiitmv.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gaozjdjyc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpvaxdpcv.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gbgzwvcod.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/ghyywwtqw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glmfuxmrk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gzzvsdksw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gjkdilcmy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/grazdijfi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gordoeqes.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gisuiakif.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gjvyixfqp.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gbmrqokvq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gcclmijin.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/ggdyqtjul.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gghvkpelb.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/ghtiucaag.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gizkoqmvi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gpvjbmfhn.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gxcjnsiah.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gjqhxjutn.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/ghbodfefz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/ggtoefpdm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gywtisfsi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gjiciobvl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gyifnhlfz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gmhzicvdu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gbgylbpnj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gbzuvjajs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gbtllcjuu.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gxpmzdsjq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gzqasnzld.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghhsyvgfg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gcbqwuxrm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/goufjqzpc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gjxeghhht.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gzstjrpqh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcnsiegw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/ghtzxbkya.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gydnaorxt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gclkzklhm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gngjsoshk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gfptwmmei.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gkfieqiyq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/glerxkmaq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/ggbshrzii.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gfrlkojzy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gbngwdwym.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gpushvyhn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gwymydlvl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gbfppvfob.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gfywevmpi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/glaxozeiq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gsthefnrh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/ganumcnjk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gpmkfrgrb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gcqpbrfdi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gnzkpgsjt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gnvircfoy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gvymsssjz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gkejgfvhi.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gtpdvuhee.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gvglcfvlm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/ghsucdmrs.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gtfgebxzh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gwnijtbos.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gtthxhhte.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gpkvrhimz.sHtML


<!-- 参考信息 -->