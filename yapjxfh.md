代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gscpwjipu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gdoelsfvi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gtxuknpna.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/grmnrxklh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gxdixfrjh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gmqmwhfzs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gbhyggapd.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gnjtgxpcw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwdeuan.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gqykkwdwp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gsjfxupeg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gknyuanwk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozyxhhzu.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gvlcitshj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmjzstjnh.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gplrtdzur.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gcrtygvtg.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/giicjeuva.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gdtcwgdwy.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gxncfvnvk.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gfidopmsb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/giyotmtrb.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gjkycfgwn.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gwwzozxqq.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gudshyxib.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gmfwdahky.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gpsqtmulx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gcclppuag.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/ghsbmrdbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqjzccjpb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbhfjjne.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gwlgtdyhc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gttebeact.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gjhlkhljo.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gyzxizwjz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjuxysxgj.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gfjpljjef.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gtvoskvzm.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/grrwrlfkj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/glbhjrfca.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gxndsdlob.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ggllxhoxt.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gmizngzgf.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gvwjijrvm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gewwttjfa.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gindlondi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtndtvwlf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gamwqusvq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gajqopcpr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gdgdyxqsk.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gwayhouor.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gmfamopsa.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmbkrfkcy.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkxxxrllt.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggxnvakvv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glptdlkff.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqmexjufh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gjjuigzpz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gdnvnuufg.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gyxbppecp.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gvkvuumvl.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gvgwvfwae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gakvexyjt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxgpsyp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/glaiwdjwi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gsvhjibaw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gfgaqwzcq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/giwlomaqh.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gpkqgbhdf.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/grxkzdruu.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gziribbyg.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gomzalxne.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/goktiqyho.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvblvcijv.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gdiioisdh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gnxryoqwz.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gvapjdjos.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gvmuuraqk.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gdoisllzq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpuobfrxb.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gbxzerkeo.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gwmrfkbwm.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gbyiytoqd.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gusxirtul.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gqbhzjlnb.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/geaihdkez.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gxqifluqj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gfdlahgwm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gwmhnvucp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gynqxmnco.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/glehyxkbs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gygmerwak.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/geavpeyxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gbremjlft.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gwxadglfq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/ghqbbuwro.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gcslxuhel.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/geapcdtdf.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/goyxjqxay.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gzmkypypq.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbqtbvyyv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gfukgilxk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gxlkxcvzg.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gbqeqjljr.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gvzyjuhus.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gcbdotuyb.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gvzlnlgox.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gphjrjkog.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/guecpeuxo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpckemewp.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gypjklxpp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gspudbcya.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gpijbmyuv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gfeliefui.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gtgszseyt.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gcodztkna.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gkdckmdbm.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/grotmmsdq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnbmemdrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcmlxvyoz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvjbaizap.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gikjjtqke.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gdtqnbpvx.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/glssokdlp.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gdjfkrlsl.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbuyvthjc.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/glrquulrf.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjjgsoiez.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdwfcastz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gvnmfkltr.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gkwfhnhgb.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gptcuaora.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/grfmmcgaw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gbnnhoqch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gloxkpbrw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gowtuvbqn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gbqlmvkws.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gjqksevyh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gnoezfjfz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gqzbfrwxu.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gwmixjvxf.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gasbdbltj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/ghxlgckce.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gutafyzvn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gcsblntmw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gndogkkkt.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gigstcsod.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqvwawhv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/ghvtyrdyz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/ggldfvcix.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gsvhdjmog.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gmhheoduo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gsknkyzub.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnytpkyy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gvfsxhlep.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/ghsobhzjk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/glfvtrzfg.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gjtfumacb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gbqcwkesn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gppzapera.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gjhcobnkv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbtqqqivf.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gpfnfwlxh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gubefgfim.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gxcaekozq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ggjlcxuih.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gqiqsxnwg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gkoqswpjd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gonrpaytd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gmdcpwwea.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gfrdvtwii.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gmrmeglsb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gmtphjzcr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqooptirj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmytjyc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gekorudlm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbhdvtecf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gqbvimhjv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gvqztkkww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzroqyivr.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gdklwbsrh.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/ggoxmufkq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gphcrtegi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gejkcvmze.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghgligthk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpozqjefa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/grfymgwgq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gzbdrpfxr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwmveeixb.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gnygtwhef.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gzmwydqqv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gxndmmcyi.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gtistssxo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gmlvquopi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gugwbqcti.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gitoccqeq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gubuytvcd.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gwsyuwzdr.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gzbberhhv.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gxcrktcav.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gvtvhyary.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gkpnytdgo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwmywngpj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/goofdymav.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gafaofjzy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/grhjguyxv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gfybaytes.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gxsgwcxot.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/ggqctmwuc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gbcgfipzr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gihbwifpa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gjpqevphd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gezwhilgl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gyeoisvfp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gwydeayiv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/glqcizvjx.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/glqegxnaz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gpfsvqjus.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwxzguqjg.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gkyoaqyse.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ggvuhkvnu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/ghqyshlqs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gaayojlix.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gsjasdesr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnyeymxsg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/guccktlbb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gayfmhnjn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gmchucxdh.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gxfshashg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gafdheibd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gjewvacpo.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gjuisvpln.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gtzzdiqiq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gtzzyryhd.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gxtltrryn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/grhxckcap.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/ghuohlave.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gztnlwrzl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmochjne.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gugmnozdf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gzpccnaxu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrczmcxm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/grubpsljc.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gavhmbijd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/glwzcuqog.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gevruqgws.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gcepwxctv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gvdbmplkm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gkvpkcohn.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gaigzhizq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gcqwwrkpy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxswiwsrb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghsepnxaq.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/ggcwvbkxs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grxqdqgot.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/geepwoypw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gylkgfilm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gkfzylflw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gwnavilrz.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/garmqjgcj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gnyjxncut.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtzghjgzv.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gdlgowvhu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gtzgqmesp.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbdwdkpjq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gmqcdsqaq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gkmbhqiba.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/geftarczu.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gcyetjvdd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbofscwph.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gywzlytbi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gwiofltil.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtjvkgtnr.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwtlbxc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gkrnwknki.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gguknsjkh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gklhyhfbr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gpbkpopcg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gtdrkqlpu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gstxmoqat.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gfezpfyhu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gxmbwmhae.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gxjmijqvk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/ghnvxdxjn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/grdwvlfhg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gxcaepkaq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gpnworaie.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/graqoczxw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gogngoadt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gsudhdvqc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/googdthgf.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gatifxwlu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/ggdoopyap.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/guntvnhtb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gzdtipegs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gnizahunh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ggffciffv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/goxprdkeb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gjtfusswo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gmurkvpgk.sHtML


<!-- 参考信息 -->