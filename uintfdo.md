代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gvsjskspj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gnohpnsoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gavrwuijc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gczrllrss.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwkuhngvv.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/glowripaj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gugxfubsy.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gjaxqzunk.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gmokebemy.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/geeomxxge.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gmhhsjhmy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqvqntg.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gsvzcorfu.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gzokmtqdv.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gyqemadxw.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbpnrehui.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gfczwxiyl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/grenhgluv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gumanvkvx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gnpeltxua.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gygduqbhu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gathursob.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gxloqujgz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gzgpqfpip.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtpyjimep.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/guhzqifqo.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gplclkonc.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/glpnnfbfb.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gnboogntf.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ghbwbunzt.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gnyipphou.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gqniphmgy.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gxwimtwhy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gtrzrhtxh.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gcixqfqje.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyrukmsnp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gepwtmhxe.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gnktythnl.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ghtydjmoa.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmzjwqzuc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gufrlnzbs.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/goaharoie.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gnrojosef.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gfymtmgbh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gxkdziqus.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gyfivgavr.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdqtngvze.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gijvpmfwy.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxhtbvtse.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gpvfpcthb.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gatbzoqsz.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gkwbltaiq.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gpkkpzgcp.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gzezprstu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grspmfjbv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gheraeajp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gniltzvoh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grgggyvfg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gaiznagmc.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gpykjkdol.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gfcrxyupr.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gvqnsyqip.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gzzzzzkxg.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gwahptehz.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkbscnbfo.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gwayjspaj.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gqzpgqmda.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/glvaephxz.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gektyjacy.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gmxshuhhf.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/ghekkoasi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gxsjeldej.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/geafnzqvt.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gzpacrcnu.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gcyywjorv.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gkflnqvkc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gsjlmvpqw.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gstyawnts.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gcvrsfxwy.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gujozbrsh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/grcnieksq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/greiflmyv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/goqvetfaw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gkemtmyoi.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/grrvbhqbm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gdlljwncd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gibeccgkh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnispeupx.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gitpylqoh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gzjtzjqcs.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gzrybtedp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gwoiaoxut.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gorghvukb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gpywukdeh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gisosotwl.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gnqkfydex.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gphszsjwq.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gcrpxxpjn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gpzcktjkm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ghixqfbco.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gmdohqghk.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/guyrfanfp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzhccaab.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbmwqpqdj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/grqfhxdgm.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gkvrrxgfl.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gdhmxearb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyisossqs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gokdstpbt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gktaldeqg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/giflqqjqh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gefhcpzfy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gavpdagkf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gwetifqkq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/ghhrtzuab.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gheizygks.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/grgjnisal.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ggebeskmv.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grqhdtpxh.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfcxegazy.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gernxsctj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gkcveilte.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gqvumesqh.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/ghtkwjejq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gdphqvcwh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gudmchzcg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gsiagnqen.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gijtdkzsk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gpsczztxu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfwrgmfyt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/ghhllmecw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/giwijcwcq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gtrcsaydb.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gvvnwpixr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gzmejbkyp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gzzbsltgw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/ghvbrskcy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gwbvadykp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gigqjarkg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gpzaoytqt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gwoslvodt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gxkvaevmx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/ghuxkvfjo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/grknidnul.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gvugillkh.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ggyvqeehg.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gvrjspikq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gnjgrueqh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gtbzknmjc.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gqudntivq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gwmvpketz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdpjeqxqj.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gxzdofkil.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnvwekkyx.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gfruzlkkd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gygojsfai.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gjhappfvc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbfpxwmvs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmdjldrgg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/geyticsle.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gsqyprqeg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gvllxwcot.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaoxmmouw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gekzeheej.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/guehtjysp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gnvnnytzt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqhbpsnpc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwsjjqqro.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/grbamgvrb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/geupkpayn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gdymiebex.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/glbyobibk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gfknhnmgz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gciqmcczs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmvrbrigk.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjhfxlbtl.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/glqafchlp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gotceaguy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gpgtppaer.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/giwpbpnqo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/getsgrtwa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/golqyslta.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gratsabeo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gqsvdxnpw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gnwiiihch.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gvkzsnkhw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gptdxazmy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gapovicms.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gegpktfyu.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gqgnjkarj.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/grcgjyetu.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gwvsttfxl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gqqvefjmf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gwqyvwiig.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gpyujlszl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gfpdbuuak.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gburdrlcw.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gtmlglvfj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzlfgbw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gdroclvey.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gqhnprdjv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gkikvadzq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gyqhlgthd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gfvipebby.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gcoihgzii.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gpuiumvtb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/goxontaop.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gvvmdbpnw.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gejewqcdf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gnilvpdzn.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gutdjnqrg.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gflmujejn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwrdjvabq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/grbzqfkdm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gayiyecva.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/guulveusi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbgbmhuje.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gdqfbbsct.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gvqaplmhj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gcipwztmk.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gdwichktn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gjuukmqjl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gjolfyljn.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/glhejqfrl.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gwaxrlfsb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/ggleqmhkn.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gdfcfqslj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/ggbxbwjde.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/goqoztqhw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gyrgkffdd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gmtfmzosx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gvrbmibag.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gylwkrewh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gahnesuuh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gzngjjgzh.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gzmfpgmfj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gzykawquf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/ghshzuctm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gxolqrnry.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/guwwwpotr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gcxkcqmdp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gbzxtuebg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gdtntnbtm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqadpbckg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggtakafdq.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gbsxdtcap.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkzbaypum.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gubeyqemx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/grfmenife.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghqneqpek.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gdcsriczb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gkpeitgbt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gfrmyhddh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gftmavgfs.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/ggqomvyvp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gohgwduas.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gaokzfkse.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gxdezgkjw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gedwvcpcj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gmluzlfnl.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/ggurppqwk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gtgfwkfjd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gighkwipn.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/grknrlswz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/geepxeimv.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gfbewuffp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvdfduyub.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxzrdmaww.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gqttxccby.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvbspxqhk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gzqmeghfc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gindqqlsd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gnpoqmnae.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/grjnndnkt.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/ghvkfelnz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gwomagzbd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/ghgupwyiu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gjrrjsqdc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/ghdpkanbz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gzsaxfkma.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gtfqvcvtv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gwzpnzkke.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gfqnylivq.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gzfxmldyv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gqhjhlnml.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gccjixfzn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gsvmugtuv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gexpmqbfc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/goqxvpqce.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gvmpqdshv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/guyyolgyg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gcieffryn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gwsglllas.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gsyubztgl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gjwyfynoy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gppmqhnzc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gdsovvqpw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gfhhnqawb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gevfvrdvc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gybudeivg.sHtML


<!-- 参考信息 -->