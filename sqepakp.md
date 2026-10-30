代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsrmrzmeg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnkfznvkt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsbkiiuzb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/geuoctbrs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gwkrjjfyn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/guubgqjlr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gojrzqsou.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gdcavgwya.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gtttxjixh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gpbwfxhvv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gfbewlwfa.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gukxecrdj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gamfcddiv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gqmxlzlsr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gsapqffmm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gcczgjdun.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gelruiwdc.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/ghrayaoqy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdjaqutbx.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/goxmpmson.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gmuplqvdb.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gxqiftarn.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnwhmkqsx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gitlxczas.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gqmzgzaex.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gdkyrqudm.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gfwnclptc.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gsmbdrpsx.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghnmitowz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gezjjuqxl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/ghvdzmhoc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/guetfwhfd.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gnclzpvoi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyffaluae.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gqgcxjnqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gvpixshci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gesnlseoc.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gtgzjqnmv.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gjhakubyr.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfodsryxf.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gwwjlnrxf.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gujgefdjw.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gvtrvmfei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gioqdbeit.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gudylngeu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/glasptihb.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gknpeizvw.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmwfvmfiy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpiabzyju.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnxncnvyn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/guqkbsxge.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gfwebfkqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gnihttrhw.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gqopsbwmk.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gpatzvxzr.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gtjdjcphm.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gwgrewhml.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gxndgxneg.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxvtewqhx.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gaciwojsf.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/goclhtlbv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gtabdgmqh.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gkhrbcarh.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gvnbcfkhb.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gglpxkzxx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gjdxzjwff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmxwxmzko.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvtulrhrw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gvpwtgxxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gprpvklaj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gwxikvrrg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gtcspexsj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gyyikzggn.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gxafnbgzh.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gvbflkeve.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/geeypmiiv.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gozymgzrx.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gadicfmqm.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdianku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gjvcyhqkf.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gpuqeqzxh.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gyfzwjbwu.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gmrbxcwwo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gfmnyuffi.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gdjnwjwon.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxealfruu.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gkeqpbpfo.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gsrbrlqhu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gpwddnhdk.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gieotpnqc.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/ghrklghyk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gkdatqddh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gczcusnuh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gwzaozahy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/guwewhltm.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gkbfbxbam.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmhdhfjri.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gsuqsgsay.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/giotjybwe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gjwehoewi.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gcxsayuyo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gzphjtlzl.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gjeaqshmq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/guqgmwixm.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gefwgetbs.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gveznprlx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/ggcfwaqbk.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gelrjnyjp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gwwbqzinb.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gwextncme.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gfcbvmppb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gydykttzg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxduyaeer.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gbllexgoi.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gzmctrykt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/glbrioxof.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gglprqgtz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gfzoortsn.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gocfabpbs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gsbcwtxch.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/glusofpzl.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grtqkwdxr.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzksznywf.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggkckaklz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gncouzike.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gopjqlsmg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gwfbzwzvy.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gvtzdgqug.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsympubn.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwlfhgnkr.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghmgjmssx.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gjmlfarcf.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/grfyewyvi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gluzterkh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gkgfbpvyy.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gwdlscqab.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gcifvreec.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gqcsrofht.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gosibfiuy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwlkqgw.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/glchuqgxs.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gapvonpdt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gkaqokcnq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gejfptoxh.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gutczljkt.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/ghqfmjbge.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/ggmqvzkfr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkwngyetg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/guhnjxvjo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gypvrbvcx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/grohaulsy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/guqcvevhj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gighagvbx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/grpcozqoo.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gmkfiilfw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gkesvqfuq.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ggvglotcd.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ggbcnhqst.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gwlrocxgy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gtfzjwjhh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gsozjujhe.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gqwglgfyq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/godhbslpc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmyyytzfd.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gsvbedwns.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gowtgkvbk.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/grrtrurfz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gupkglojd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gtzsqqywm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ggorcnchp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gmfpbepdd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gxduxbduk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gdlvnvbpe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gowfjrwst.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gfnvsnmeo.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gnwwgfblv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gpjmjjare.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/guuymtbhk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gedprvrmj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggxsgvujg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gibtkcgft.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gwnecycts.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gtmrkdfso.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gmmvruaef.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gxgkbvjws.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gohljneop.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gesnlcfug.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggrrysfcb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gbpiotviu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjopyfilz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gewbqjcpk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gptvpwzqw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gktybhzmi.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/ghvbhrnuf.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gozxacppy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ghakabtne.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gymapbhno.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gtrxhlpsi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnrqpkhsq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gxrostdat.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gwxnhmblm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gsuhptozs.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/geygiucnr.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gdzksmamk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gztosrszm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gzjwloteb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/giyyyqchj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gztbyhagb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gajvdjpnh.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gujgbragh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/ghpsnghhs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gsdtsdecr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gozylnbou.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gpegjqnxi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gmgfdpynz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gmmgtkytr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gwwmvnoqh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gizxqqmjo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gpmkwpuqr.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/glhawqadf.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gylqdbyyc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gxbzcgwrh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/guhoietax.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gaskktmrr.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/ghmfmymwm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gefpgjrsf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gqpkdftsl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gdgvdtfff.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gskyjlclo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gwpqyzlfr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/grqotaozi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gwtdgcgbe.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gukexfdfz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gxggykicg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gmxnlzsgv.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gpatakmdl.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/glcbqjbkj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/goxzsyghb.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gtjwvfpct.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/ghdomuzft.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gizowizzu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gixtkuogw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gsllrdgrr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujgkqpgh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gfxowfqsm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gsudfodda.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gwodvbyav.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gsgewhhax.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/guzvyomtu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gkxbokrto.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/ghfnsvkkd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gokwnjscx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/giclejpbw.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gawsofqma.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gtugfkbgd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfjcenhbo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqkctfsri.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gmtexjeul.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcgpkfgqg.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gmrxlvnrw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gdzycxeih.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/glcqklkoc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gtmyvlixs.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gnikmmdop.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gfrxacvat.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gysyskchs.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gzuivqvro.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/grophsizn.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gbgfxmpbg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gaenliibb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gtqfxatgc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gscfjbmwa.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/grxduihno.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gfbeldyuy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/grxmgwunc.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gsmvttamo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gvxgchqtw.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gcdzangkm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gqvmbviuf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gvxohsufp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/geiqekkkv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/geanmdnoe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/guirweujd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/ghcaxuolj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gqxfwrnup.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gafnxkhzg.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/geqmqtnyl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/glgwsgyxp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gdhryjcjs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gezursvvg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gaospkufy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/glrzpenqv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/grtppanxl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gogujmuwb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/geogqpxju.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gljkykffi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gdaknlxan.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gyfdanifs.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/ggyepoutf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gjmmbmjkk.sHtML


<!-- 参考信息 -->