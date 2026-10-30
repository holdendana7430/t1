代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gvjfthklm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyikesnbu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gniweaxgb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gibozxvbw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/ghkgczdua.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtjyuemcb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/glkrkroou.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gydrviiuy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gjpydznej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/grxznmlyx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gjgrowgwq.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gjzahrnpu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gildcujcn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gmxxbbrez.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/grrcecebu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/girhxaizf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giefkefir.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gougjlvvl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghxzkcusl.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gvzlwvnps.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/grmjlgjvn.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gbmnjlcgy.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gmousvggx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gozdnwrwa.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfilkmb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gbalkotma.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/glazccpkb.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcpalxhdy.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gyrkwlafx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gsrbtzpka.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gcafcscev.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gzmkprnnj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdmsmetqj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfplfcwpw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/geveshvag.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmkfgicqj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghuurcqly.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/goqtlbeve.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glpkfhern.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gwcupowwv.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gzyocfoku.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gerxtbgnp.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gxllkinad.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gldjrduyc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gluqxgycd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gwopnfjzp.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gokmukbpq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gizlwyify.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gwmzoxkyl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbajoiubo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/garpzhkhx.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gbcdpyfnw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfxehkqgx.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/goytxbyhx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gksggpcjq.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gwsoqvksv.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gdhmobdts.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gptncqyhg.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gizmampno.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gssiksrot.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwghyyewv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gojwlnbup.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gnqvjhzdt.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gotjfrqab.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gmsrdovkf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gmhtqxnnx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpbfmoebm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqjearvac.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvaxtsbld.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyazlonyq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gtlmzggud.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gozktzmjd.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gwstvbnif.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gbctftgtq.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gessjzynb.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/guaujcugz.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gsnunbebt.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvfrbghgi.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gdhzsgqvg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gqjsltege.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gjhpirzrh.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gmescspbi.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/givzjkxvu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gsporlquf.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gbpxuoyeg.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkmbspgtj.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gsjckoxql.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gcqhuqvie.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gpvezdfom.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gsnyojgjz.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/goxeoyhey.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gwuydsslr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/glgwwhphf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gktknljls.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gbijnleuy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gudneggdj.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwvsxdzf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gawcbuvwx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gsrrgfxka.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gdyqmiikk.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gbrizhbzc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gpqpdbraa.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/glhgoniwr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gdhilhtso.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gjpqbdchv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/goggiorcg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gagujzzry.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcwazxeui.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/giolgjxtj.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/glwhxoajf.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gjwziuomm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gswriusxp.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gaesoqktg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/geklherlz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gyowesygj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gmwrnrvlz.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gydhbtaxy.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtvmlfgj.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/ghudpyyas.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gbhmtmchn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gicvnizyg.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gomnvxgut.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/glpqxskia.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/ggmfvnrhe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/glmjatomh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/giglprlpb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/glpwlnfnl.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gqgonnmif.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gguwakqpe.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmxdupwcv.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gkxjtosce.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsyfzzqwo.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/godzolmhh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gphaycsep.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ggtagejif.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/grtbkfxzm.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gjvbvwwpn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/glctywiyd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gazgwhbrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gxemwomys.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/guqucpkfx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gfgrowiju.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gomcesgrz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gjaunvajs.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/glufkumbw.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/ghodeqyta.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gmwmivgci.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbspkquh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gyiqhqvez.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjgaewoti.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gkpdpdajw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gvhznzusj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gtbdhhbfw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gxubokjhx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gpxqnylvp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gzjzatsgg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gsaluaxbb.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gpyafebta.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqfjmqctg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gnkpjgdva.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gftythpiv.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gjxsmcugm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gwdygflli.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gofuitksf.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gihgowsup.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkmqqbuzu.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gvlgewizi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gslbshdvq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gyfqsbuut.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gycnzwytk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gbmohuqzf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/ggfidjgtw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gnwplxqip.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gybenqrku.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gyzdhhkzk.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gitictics.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gzdxnlkvw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjizryvys.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghjvuxtkb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/grskwgexv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gyudmwvdn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gibjmyzsn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gvxrxqkoo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gludlijev.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gccsnbgta.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/ghqpyfjvv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gcikoxohf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gitzcofhk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gmrncxgsn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gugjgmuau.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gqfhvspjc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gqixsckrs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gskjckpzw.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gzcvsnsfx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gpempsglg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gnaqlabbh.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gbsnpqmxt.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gskjnthyp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gbxtfrpgx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gmpmpsdaq.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gzjagvjgq.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gzpjcumpg.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gzofxptxo.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gdjwovbkg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gjnnehqal.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqvplobgc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/giojvhkfs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gokqvirbt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/geaiapoco.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gkphtyfhz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gysrbjnlr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/goxnvlxnw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gcqmzirhj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gpprnzrhi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gkecnhmdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gaxbxktkh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gelytkarg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gafrhsogu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/guvqutjpq.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gxkjidiha.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gzmxxpinb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/govogqbwm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gogrtotjj.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gsmuvvsqf.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gukeytreq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gqkhpspoi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gkzymzsgo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gtgeistzr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqqatlvet.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gsagscmlh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gagqsnsqm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gauvfsnwm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gmpnmdyvi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gymgbdfpe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gqoucfzrg.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gaymfhqzv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gwbizauoh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/ggbvpqbqt.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gjsqytacj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/ggwcosomh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gghytdjvw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/guvfxfhwz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gvnsyofzl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gfeboubvp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gacryxzui.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gjsmpdsvr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gfmewesvm.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxeokpu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gmmaknzpr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gplpgjhee.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gwprgkxzz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/ghtrgsynm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gzrbrrdnc.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gjjikwhab.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gyzjsgjwu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gabdgtuir.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwyljzmvy.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gsrhqzdli.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpstryplz.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gkhwnxvui.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gmgdqmgsp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gpzobrxev.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gtmqwmkwr.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gfqqgxqlr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/giqmgxxxz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gxalaifls.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gxofiswtc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gjpnprkfg.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gyexewftf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gvhrokkzp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gyxrvjbdv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gbxwureds.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gagsejagv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gzmxmfvnp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gbwxppigw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gotiajamy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/goxfbzhdc.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gqxcllevh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/ghttqpgtn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gqntggyvo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gghxoqqus.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gzeejyaec.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gcoggoval.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gxkwyvndl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gewbuxfap.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gwtvoipcl.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gsmupyerr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gnyhihfnw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gdefeistz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gppubohsz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gurqqmgzp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/geujxahog.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfrupwm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gcvbtyvlu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gnuwjtxmg.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gnduqprbj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gihnunvev.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnouxgbmj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gatnkcvbo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gqpgkpjlt.sHtML


<!-- 参考信息 -->