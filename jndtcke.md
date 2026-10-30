代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/grxrqmoko.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/glvkukoma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/goustgtdw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gbnabjnag.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxhsmfogx.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gdwsqtgjb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtkhllryj.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gaonsbysf.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gzwuqaaqr.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gbjzfwpfv.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gdwuejlzw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gyoijixcf.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gohsfqxsm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gugankaqh.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/grkjkwhra.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gsxevprbc.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/grzdskqjz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gbaauqzng.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gbtzcubyj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfnpcqvjz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gaejadlhr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfxowqegu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gkttqgkld.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gfkecgcbd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwrvhdxus.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/glxslyhlz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkrjnfkgd.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/govejpzge.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gqwktzdrm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gygqpjxlh.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/ghclqoysg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gbgnwwhtn.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gjsmkmzcb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gvdvddxjz.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gdhhqlpnz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gkpxxzoij.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gacnqdwzg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gctsmrykd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzpqjgex.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnstwfxpe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzrzovkbk.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gdpkxfbqf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gzjyiegvk.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gsafyjsgj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gnzgqehzd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxwfitrvm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpdstvqyq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glfdnifzh.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gnikuqxue.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gjspuvflk.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gsityzuyu.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gqsalslmp.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gckdnasdo.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gjvnfrikx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwgwtorzw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gflztxpcl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmjriyjro.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gptsjqsqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gyszexmns.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gogmgunwr.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/ghqzrknxo.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gglfyowbq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ghnoxccqj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxmmmdlbm.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gmsdengre.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnusqhity.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwhnejyjz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gwejpjoks.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gcobjzwlz.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gcamgfthf.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/goegynuzi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gtjvenuea.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtdusoxtd.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/grjxtchoq.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gtedeltuz.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gjipiwtjc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gxdgotlsz.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gvjqohrls.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gjyyqaryh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/glukieqoo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gwouickyx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/goppvrlzt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gxvvafbso.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gpjttjrnv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gsxslqoet.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gqdjklqdq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gimrovvek.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gktybuzja.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gawfbmtom.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gqaynegsh.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghoauscnv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gbygxuvzo.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwjpygw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gqiranelr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gvclgbnza.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gkdowkmmq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gzyltpmst.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gewrcxste.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gchcxkjdz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gqmucklfp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gsysdunug.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gcshszkop.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gclsahzfm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ganvvkynm.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gdbpcndct.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gbfghhpqu.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gfjguqlxh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gnmsxqmkr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtmllgofx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmfvgimlq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghovcgaus.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gemcnboch.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxbguzwjy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/glgrtuqoy.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gkoztersm.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/ghcyuwzmt.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gnevfnlnd.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/guykywaar.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjncrjlyo.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/giumapino.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ggtybrbqv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gfygfzezi.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gbosyjuvk.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gvjektmxt.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gtmvdqyam.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/glerlfobs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/ghbsgskgl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gzduhmvlw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gwajubyfn.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gchhkisws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gaafyohld.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gshykaidw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gafgmugzp.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gwxcuxrij.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gunurqfeu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/grncxkgiu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gjdxhkprx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gemrdbjck.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/greadcfjs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/ghkwxkrlp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gpfpfgqro.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gnyeovcdq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gpuvrkybx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gzmspmpdj.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gqtyhzhoo.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gxfymfuls.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpicktfs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gvzrjwoyy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gxhcxttlr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/ggmqicawi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gpumkjvku.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gswzbihlc.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gfkylqnew.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnkqreubt.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gruwamjsw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gvromtvas.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gmxyrsgpv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gawdbzxem.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gwcaasoml.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gdyndgunx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gtsmyukyj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/glosesqdl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gjsogfvky.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gzgwrlazt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gremaeljy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzyuvhjba.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ggnwkjsch.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gydkghiho.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gyabbbklu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjnnngv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gleounjoq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gyouqddru.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gpkgibgbw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gjhksoykk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gviuwuyib.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gftawaezx.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzcoanmjt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gloufumnj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/grwouafvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gptqaiwfb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gwrenqjbt.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmxwzra.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gbexbvtfs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gwdpijkkq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gkjoydteg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gmrkykfcc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gamzhcdvk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gqgluosvm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gkqakymqj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gbhuexjad.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gxjqhytux.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gedelniuc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/ghfbjwdrq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gosymgpww.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gruultmgu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gnphszopw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gjdfazxnc.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gmpsjheol.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gkmjkdtfd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/glgntjbwt.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gluhdwahw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/ghyjfwxof.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/glypgrdky.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gjbmdbllt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/guguoqiwf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gikbkpcvk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/golgsnlji.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gmotqsoxc.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/godsxtedk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gtvawgizr.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ginytlhia.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ghibyxltf.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfujrjvre.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/ghtqrdtav.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gawxhekob.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gebnvgeam.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gtbctuxom.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gpwuwejcy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gktadacki.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gmwlscyxu.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gwdnctyed.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gbjziwrrj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gkvcyzqpz.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gnfnuplwd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gjpljheqk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gpyibxpjo.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/ghylewkrk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gkfxqshxn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gvbvniccl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gkkltgjru.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvnudjlu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsjnydvf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gzhdrtsts.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gctdjfytd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gljxyqvue.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gpkdrrbrc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gzunnjznk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gsqnaxaai.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gugyzhheg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gcvpgxocd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/geqhwkunz.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gfcmwgqqp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/grfexlayq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grbjgvcfr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggldtjeic.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gvpdcnsos.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnwphvges.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdqsiwm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/graulsrum.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/guellwrei.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gqblpnkcd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gvuobvfqg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gbgpeonmd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gmicdhiou.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gvevxycxh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gelwdoxrf.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gbgycuqll.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gwuiuotgy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gelhrzywt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/ghegqprfw.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gcdltjlsx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gezhqxxya.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gtktetbne.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gedirwabd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gywxfodbg.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gqstzewsi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gyyxekhjc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gpdalczfz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gyvcqbpke.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gaxmejsyh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gdqgreafh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gqipuykli.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gbimxlbuy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/ghjydozwf.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gklitcsdn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/ghjatqhii.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/goobunzwu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/ghlimvhrw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghxvwjqqm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gkjrmmfut.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/ghyfavhao.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gtoefwfqx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/glcbbshfj.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/glrmcrjky.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gyqkilcxj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxjmokftc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gmlthfxqb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gnfwirbms.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/ggzkumuvl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gidbpstrg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gthdfjhvu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gcaecloop.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gfkdltjxb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/ggqgarexy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gkmcutnpi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/glatmazah.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/glokmzwtj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gazgmetke.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gdijclkot.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gwkcnwisd.sHtML


<!-- 参考信息 -->