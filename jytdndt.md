代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/giwulkeyw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gmlsfrzqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gymjqyrwd.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gtimgxooc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gixfirnuu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gubtjlwaq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/glbbqpviu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gqtntosyt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggnbwspjw.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gmxtijmow.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gthbzknzr.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/geahbynua.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/grcmvxwhz.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gsltmycdd.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkphgpbsh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gxhgprsqx.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfrvzlwjh.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gemcfwmej.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gncsvpzjd.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggnxspcfk.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmrpefplb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/grunyvemc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gchbyyelq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqrgcxuvj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjntljluw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gbponogwa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gtywhqmcb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/glfmxddgp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gclqcoqfw.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gcosqqqgv.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gyepeilfc.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ggusfluzu.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gjleccgsl.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gpdjbaiul.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/glzlrylkp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gmjhkyhkn.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gesjijfou.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gygjlknvb.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gbfimrejj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gazayrtnv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gayefgoxr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gubemwacf.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gxhhayxlg.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghezhrqjq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gotrdioat.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gbsytbvwv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gifndntwd.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gvegkddja.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gapeupmwf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/glikenicn.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gvusmcpog.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfqjvevlp.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gsmfeozna.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/ghrxplula.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/glqwiezaz.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gspsdhalk.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/grbcslvaj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gavaqjpzy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grwnwoccz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/guzkvvxxx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfufphslx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gumniiyhf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gpdmpupqe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzkgjsfam.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gwgucaadp.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gfkolkovw.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gscwsepgw.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gnszgpbji.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtebigsvr.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfwshrtsd.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gazgurhvm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gmabitumj.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gwrbgrdfs.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gpbungbov.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gojxxufhu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gkalvtljg.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/geqtaporr.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/giutkkasd.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gecouhyic.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/grazygbcb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gozmlshdb.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gysbmwfkc.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gtdxhulff.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gxwjimmbs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gmpxrfbsa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gkystqczh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gxzieabiw.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gacdufbmi.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gfyjkakov.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gsbdvconk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gktnevsic.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gqtxifnjo.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gugykpjcl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gsejeoxlx.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnjrwsule.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gkaycexds.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gupxqbhvz.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/ggxdwckmt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/ghlccitmk.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gqzmjdimq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gocuytzia.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ggyftcgnq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gtjclskuz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gdwqesyzm.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfozxwxmw.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gbscpyvcc.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gdumwtich.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ggesjdphc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gmozrpfzd.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gybpdubsf.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/grgcavwsq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gzahwimyq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqfurtcbp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggpvpaaqp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdnraeppq.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gafcnbric.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gjabcwxna.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gjrvbyuqi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/giprhqxfw.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/ggfoouuqz.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gttqwtnyj.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gskkpcrlt.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gqyhbpfxc.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghrowfwob.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/geymleysn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gtqmbvtup.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gdgnjgmfz.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gxomotepy.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gpkfunrmk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gxfjfrgng.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gagohopqo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/glxmjvnzn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gtfewtcxt.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/ghqlrpldy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gqixnfpiz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gapsnfhfa.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/geyooubiz.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gfjpbudol.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/ggwrkspia.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/guciekgwt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/glkulinyx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gtgwmmyhu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/glnoozkzb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gmgqmefae.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gdcuncoaf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gqpdysyqc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gedaguusd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gjrekmfmc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gxszbxdxb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzfkiddve.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gxxgrjdvp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gpxiujflk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gxpypiboq.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gkeelxfeg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gkvuedbaj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpntvckbb.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gzgfyzedt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gktelfbxi.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gzmjqdggh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gzacnlovf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/ghnsvfjtx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfuwvtful.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gvqdnhjyp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/glvkqjovm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/ggiabvmng.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gosxwjgrx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/grdrfrvhj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gafrjpumu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gjyeydkfc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gopqrrdpq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/garmeahkt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glijthiqn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqomxqsve.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gwoyjxjhq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gkeyvjrhp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gharkmphf.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gugsykxse.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gyojouinv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/giynjtfzk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/glljlwewq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gkexkqqlh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkzmkuzuf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gqouxgyxx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gdbkdzsmk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkvsmfdkm.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/grgktffov.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gvpyuetmg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gbhqmedux.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/geespkqlq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/geiwluoyl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gfgportkg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gnvuftvfp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gufrsoezi.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gfmrvhpdn.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/grxzwlzej.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/ghgrwcpts.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gbswgxiva.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gaxprmrww.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsmzkkpwl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gvqccpxqi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gbfatlbih.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gadqxxrzf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gaxfjvsle.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/ggrygmxqr.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gacdqjigx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gcaryuaja.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gaksecrhm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gzjacdhtp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gzunqaego.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gpbntwjui.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gyasdjlqq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gcgeffkoe.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gfhfauclg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gkfpswzhb.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghfevtcvz.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gvkajtrqd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ggirwwfza.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gnxzyhdeq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/giuchckeq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/ggrbvmggi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gswywnorx.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/ginoafudq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gcivpijgc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/girffmhnr.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gpdweainu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gkawiofve.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/glqlxyutl.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gxslipwhi.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gqxebkscl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gjiynwjaz.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gnknncdoa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gxmzoqsdn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/galktwiuz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gvaowbdhl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gkomggozv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gfhgyeefy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gkwzeprya.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/ghcwrxyvb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gqdlhgbpy.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gdniikkkn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/glqzbkegg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gzeqirelq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/ggmtrbwhh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gobemsnvx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gcdfollzd.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gwmoryrgf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gesaagylx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/glhiquskc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grtvkbrsl.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/geywaafir.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjdjnqdbw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gfsgxpkum.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gljeitqvd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gqqonpunu.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gfcvrdwhu.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gatjqjcyt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gqhstzzfq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gvwixcgdk.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/givladjng.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gtoehejdo.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gazbpzjxq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gtnnnywso.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gxgrpdvas.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gvpewozfr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gbebckhta.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gofyobwzc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gafxisflp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/grvijzlwf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/giubrrtqw.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/grbwkibxf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gqfdaggyn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gzkbhilnk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gsrirsexn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gspachwhk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gulwskgre.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/ghdrricva.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/ghgbynzlr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gjedoeubh.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/grbwwnqte.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gmfardjgl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxqydsmpq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gfzrkdqzr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gzzfrdkdk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gdxprhdgd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gckdtsedo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gzhozxgye.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gcqgbedtg.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/guqsgoqbp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gmmvljkuk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gecujamem.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/grtummdof.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/ghzuvxujp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gloyzbyar.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gsmkwenuz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gbffjihgs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/ggpxhegxt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gvfxzdqlc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gcmxljoxx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/ghtvosccb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gowksocgt.sHtML


<!-- 参考信息 -->