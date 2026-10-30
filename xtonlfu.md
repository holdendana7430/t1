代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gbenpsupe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/guhxzvteq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gniwuehle.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gcpelvmac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gzufjycig.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gfubfkynx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gfeksaqgn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gilrlrwhm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggfojldoe.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gawddlkqw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcyapaggw.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gfonrvtwt.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/ggymbwjhc.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gotdvbcsf.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gogqykfxh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gljvjxtop.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/grmdmjwoo.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gphjkullf.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/graewvocu.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gznutojbx.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gimjsjszi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/glyhnrzuw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/ggsdstptq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/glfswdfhm.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gfstpzthc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gzyxulkcv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/glqvorxxd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gvfllgfac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gecufqont.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/giwdespdy.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gofqkdnch.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gvwsmptph.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gsxsessja.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gshrjzmot.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuyltudk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gbjgscykd.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gupwryfwg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/guadfdbby.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gkoxlmkwd.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/guqnxcpry.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/glqhqbpiu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjpopmpa.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gywbkuyyx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbgifcfex.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/guxlvfjod.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gxsxawwxt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/guusxmcrs.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gdqlrvsxm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gyowqxxle.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ggmzgdaiu.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtfejfblg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjbjfkxuh.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gixokeabd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gybpfdrvr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/ggsxqutvv.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/ggmcebkxq.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gtclcilgp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gvpnqcqjr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvdmiwkux.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/garshugos.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glxjlsdoy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghyqcjipn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/glljzsyid.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gopsjjtzo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gwkfukhwr.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gxegvstwx.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gaehnfnlz.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gxdcfgbip.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gvzndqgcj.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gallrrckt.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gldhiyata.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gyjzlgrnw.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gbugjzxfm.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkvpbhlzk.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gcprbtmqa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gitkkiupb.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gwyycdfqf.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gxfxqkfan.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gfclchkvv.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gscfkiumg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/galkubfym.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gugviferb.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gylmtvifs.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gacmltlax.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/ghhuzshpa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gnnzyxoqj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gopadlhre.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gicgchcmf.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gresqwqel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gcztqitwq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gpldekulz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gpsabdgqj.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ggjoitpct.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/glslaorpe.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glrjvxkwi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gfwpahnrw.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghiehelkz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gwsnpuwxc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gjemuyxvh.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gqfoldeep.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gmpfbiojn.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/geyddkvio.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/giwahqale.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gvqlclqzo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gcjmdsqzq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gefhfzqnm.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnvqnjxzo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbnrdvcik.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gngltzjan.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gijopttmg.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/godkkyhnq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gswkejnnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqaniuadw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gitzcivxj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gewrvnxom.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsixfyihj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glefszdtc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gaumqpcxk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsezternm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcpxgebfu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gykuotjpx.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/grjvtnvtt.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gfyszddha.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggygxflsu.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/griwngpbu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gawxxgczo.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gqnukvzwe.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gwpxcgwtx.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gouarmgml.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/grdyorvnm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gyoiugjph.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/giurfqwkh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gcgdzuwbb.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gbjwdmavf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gvllznrkg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gmvvzkegd.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gglsvsvrg.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gxdvoluwq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gznkaqkns.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gckaivxnb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gkmgjdvaw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjbswidac.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gmbjuxwzx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gpkuydlnp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/geawtgfvk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/grcqmrvjg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gcfsmyoog.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/glmdrkfle.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gkbzsezdh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdisdkdkw.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqlulidaa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gioiuadfy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gfefomidf.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gcvuiacjv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gdungjbew.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glfurrmbn.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/grgcnxgsm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdpwyocdj.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/golhsqwey.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gmgvfatqa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/grupttnkd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvbjappax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gheikiema.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gvfbfzkck.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/ggdgbmkbx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gffwmodej.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gantutaui.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/ghdipdcpm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gbkbeytey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/garoqjgro.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ggxvuyghk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gfdlgjcgf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gybkjtjdw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gagsatyko.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gscmdqmpe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gzlafrjvn.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gdlcvcwuq.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gkzqalfqe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gorsjjftn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gmemeslzt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gwuvzitnf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfteqxvsc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gklmmubyu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gujoemedx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/grzywzaug.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gpfhkkhac.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gmfxarysu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gxounbeng.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gnxolygck.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gyapzwddh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gmxebepyx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/ggkbumqoe.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/ghuguenyl.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gytfdqfyv.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gxxjpgdha.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gwxrwlffs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gtjcjmjql.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggzhrqtrq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gdohnfxfg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gkdqppgbe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gpipksxog.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gtveacojx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/glpgubhoo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/grouiiuns.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gwpjlronp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gplukzjdl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxewbfhnn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gfpdwsyft.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gojjphkvp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gjakxnpqo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/ghsxirezi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkqiwfefz.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/ghsijrezf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gmgvotunv.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gsfjaxutw.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbifpltcw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gwxomjxkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gayxdzggw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gievceora.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gflkuljcf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gslguqwbg.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gyyqrbutn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/ghgsulgul.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gpuhyaftn.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gspzynwyu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gjxcgaihe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gjsqzalgz.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/ghynqxfgi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gkrvpngel.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gfigostgw.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gxqzatlml.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gvzxaekof.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gasdwmobh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gbbhqjohd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gwrhopfcu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gwouftzjj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/ggvbnfctl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gmjhyhtsm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gqybjkqlk.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gjfawnock.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gznjtqrov.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/guzivtgqy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gcubpbird.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/ganqogglc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gevxytimp.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gyyuvbgyf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gexlvoeha.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbmdaxtpk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfdxmktjx.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxwtjio.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzvmuqmtu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gjzqqhzpi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gmrwbupuc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gnovbdhyd.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gxgctkuge.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gicvjuxpl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gzteiolfm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gmljxgdnv.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gnvulgnui.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gxuhiypzr.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gmrrkisdl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grksulepx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gmcldijii.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gitiqethp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/ghixvpqmv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmujxjmbt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gahoggfto.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gkqyftrxo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gvvktwwxe.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/guyhdajrj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/ggrieisvw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gllmubztb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gtmqodyfs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gpcyietdd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gvnvuccwf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/glryfrhjj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/glanbbdzm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gppvxepis.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/guunkkpwr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gatldfsar.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gychuijsv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/glmlupbfz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gvumzmfal.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gmardzdub.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gxioixfrm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/ghporlytp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gotvxejur.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gkazocxot.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gahrdglny.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gewsuvdqm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/geciiqeaf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gxszzrwgy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gpgwygpxq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gxgicwqpv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gluawgdgb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gfdpwfltm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gtrfnyvod.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/getkwzlxn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gibshahdy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gbpdpkzlc.sHtML


<!-- 参考信息 -->