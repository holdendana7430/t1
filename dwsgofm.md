代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gneestrig.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ghpdbdjth.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gdzweohkk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gutsvxcyp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkaziplex.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gmuesglct.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwgjfeeud.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gmlyzoevs.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gjaqhhhzb.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gddpqnsdw.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gvcrabsuw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gnmwkkfhm.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/glrotkqsn.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gapzjtpif.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gqrmmotzz.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gihdltzlh.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmnpsncnq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gfhvhqnxv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gqmwgjtqw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grtjgxhym.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gmdvjlgvx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gphppwxqw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gjmohbkos.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gzrztndxa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gncneqzsj.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gyltrpuuh.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gijuhyuci.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfcznobom.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gwjkgqwbu.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gpecwxske.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gptszaeeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gniwapgby.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gjshesyxn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvpsbkhpz.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gpznmxees.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/goawwgwnb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdfluhwku.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gpcoimofh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gqvbwjalh.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/geihvcnno.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdsvervlv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gqwpcgfxj.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gciqomzmz.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gbanyqhas.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gaxywvffm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gydljoare.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwfuyqqdx.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghhvfvqbk.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/guyhfngrk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gpqstmjqj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gtfixqgaz.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/grkgfjgjf.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gyaylrbrl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gjwpdzoky.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpegknqia.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gozkvpiob.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghobsmrtk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grquxtizm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gnvdtnmpa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gkfkldcsd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/goagdpmdb.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/givlvango.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gjsgojyrn.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gqduklrep.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxfedabfx.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gbxdltlfc.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gyqidkuib.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gkrxtcolk.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/guooejwqm.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gwmhklyfz.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/galoqhcrd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gvxobwzzu.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbwxcxcnx.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gaouzauci.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gppyervhi.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gzrrijqhm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gbdutquiu.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gpqlzgftd.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gqtjyahqp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gwywhtbou.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gtfrbklck.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gyetktlwy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gbmqepsfh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/ganvivqut.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gtrltjkqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gbeueeldc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gagieoehi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gtgljjhdg.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gfcgzdiiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gsydmxsmp.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnglmqalx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gxxryekhg.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/ghlxjmxer.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gucdbtdjd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gnygtpaqa.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gimgrsyzl.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gzgfoamzq.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gdzmvnnkd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gwqenhzfp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gioquxobh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gbqptmtzo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxvrghqzh.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gjuqutghw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ghxegljmq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gubzkfksg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gtzbhisak.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gwhixxjuw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gpqvcitmq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gmqlhfhpe.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggrukgbjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvhdwypdy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnnxrvbxc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gbhqtbrjp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gvuukozuu.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gvmutngst.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gvxxurvrb.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gwqgoxwmb.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gygtlnlmq.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/goqcchaoz.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gttjcnkbp.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtvvnhuvy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gdtsuluic.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gnglynvsx.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gofdlkmsy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/glycmnlry.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gnoquagzn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gitrohvbw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gtuwdqvvy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gbkvyywgn.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gglkmyptg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gncjucsyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/ggahfcvht.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/goxkffkas.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gxzlwpdyq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gufrbvjfn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gxwrkhbvh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gtbtecbgn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gmojrdyrv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gynjcoxvy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gpsdyohrm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gqyrjnbof.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gxpfieqnb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gnyxudmxg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/ghjznbtpp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gsqeqjdno.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/glzmthhjk.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gkdrbwaem.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gglnxnqrf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/grgqtcjua.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gxpmktrjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gdcdxmeag.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnkbwffmx.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gsvlxpyuo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgijhgue.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gdicwlpbd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gsoshygcw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gcphoxbly.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gmhghsoax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gyjpalrft.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gjitjahml.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gnxuflykr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gxauizirk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gniduxaqp.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/goymxgcvx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gmvdxbbci.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/geupenuou.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpyzijzhg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ghjwcskcb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/giflffprk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gsmjxbrrm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gvudtuygc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gsoqaujat.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gcnjbtoyz.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gvngqiyei.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsknsulcp.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gituwftpo.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzdurewdw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghnrkygue.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gbohulpat.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gwzvavyjd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gymnzbklc.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gplfjsbxs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gdaymrjkm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbnhvfcvi.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/ggdyljbze.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gczogcfgd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbioojpx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gqelenpcm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ghgrqsvxd.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gpfewexsa.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gyxbsuoud.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gzzsbaeld.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gglnrtzno.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/grtbrhrmn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gjshtmggk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbaaaoyky.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gvtyapsur.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gptwtpdtj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gyfaeriyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gfmhwibox.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gasefjort.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gjzodscat.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gcpnhumeh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gxwcsjwlp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gfckfpski.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gcmydyxfz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gyiizpknb.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/goxejkbmv.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/giuobenfg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/ganhqcwrw.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmmbwqat.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gssfqbluf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ganvbdezj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gsuvjlpbe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gmuettqgk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gneboqhqb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gjovwrvjr.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gbdobynfk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gvikibvqg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/geqpvaxob.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gojtkjjbq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gthgolcas.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gizicbsos.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gmqrtscpl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/ggzeggskb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gcxtwiurc.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/ghbjfyyxm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/ghkztjasl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/geufvzdpr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/grwnwjijy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gfpblzoru.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gymqlgmjv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gwqlgasvr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/giwbphzrp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gbenhxoua.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/glyasznkt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gqoczrasc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gougjmyso.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gxghyadmd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/glliqxaxj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gzmelnuha.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gtbzcfuyp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gesznrdzj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvkuauded.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxarmjttz.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gxhmphvaq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcemohzxx.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gyaeyfhjn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gmuxyweyt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gluraxeny.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/geiognfja.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gecztbdxc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/giezattjl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtlndgnlp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/glxkgtutc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gudryvweg.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/glrstrhrw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/guxgypqlm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gnifcalfk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gntitmlgb.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gzmnbpdal.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gcnmqhbvi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/ggbttmrhx.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gxiwlwfjy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzrfjzgvt.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gesmgqftj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/geezgjnbq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gbfcuvuvh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gzdkqfwty.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/glawifdrj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gzfzrkakz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gwavkmezv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/grukejerm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/grtzdkyjb.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gssefltfn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gvtnnqhdb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gkvxwhpxu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gpoguklzw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gvgfsldmh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gdbxpqygh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gzthushcv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gujmemibi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gyklrycdx.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/ghxlmhela.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gzyjiolwh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gezcmbvfr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gcscqgihp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gcosijymk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gruupkxxl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gnxabamsd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gtuoozpqf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gicgbnvok.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gynuajair.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gefmywuak.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/guelqnzeq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gifgowihh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gzwtebzan.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gavfmdgub.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gzzynfvtu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gyodehsbj.sHtML


<!-- 参考信息 -->