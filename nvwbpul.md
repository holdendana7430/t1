代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/glhzhwwzd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmywpulbz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gbfdhxzsp.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gkyctibmm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gqxzhxkit.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/girwmsukw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gthosuygy.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gtrdtakre.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/grroultxz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gfxyykdlm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gosailrdv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/ghctaujeo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gctlmavao.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gelftvkfx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbeifxqmf.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gisdfgdbk.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gzzknwxra.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfqvywmhw.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gzbkvlomk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gjmhdnolf.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gxnbukjss.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gfbqjvomr.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gihwhmrfe.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqkllpftf.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gugsqapkk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gxanymizq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gsijrsxhb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gttoumljo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gfgporugu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/guqtulmie.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gyzxvqqgj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gqmycwayn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gowybcnkk.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gioilllml.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/giobvjfkm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gizcuqmhu.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/guxavxxny.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gbotlbmbr.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gqofuitgh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gwxkyjzmi.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkopexlcz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/galeftonl.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gxtahzbhq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsexczsgp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmhcwwvxt.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfqarhrvt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/giyjiasce.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzbyqdgfr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gaymkgvnw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ghurlxhmg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gkdfnufys.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gyrwkzzkx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gkfcokgim.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqnqtbype.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbjraznus.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/goyuuzhkc.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzbcqnlci.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gihekwfyk.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gpcflxnyc.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gwhaykdgt.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gjzjzqxvn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/ggvmxlmue.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwiejwmct.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggndfcpmf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfxuqdkkl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grjncwqgh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gbxqxujyh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gjznuxcpw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gcxmmoien.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gqvvpqzlb.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gchscrikr.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwwcbbswj.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqrbtiylz.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gkqqrvpqd.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/ggoubudcr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gmihswzmz.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gflifhywd.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gnagfcvwq.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/grnpdvmuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gmmueebzt.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gozpckkui.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gknktjjle.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gxwlmnstc.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gffrcpjsd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gjggtgdqs.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gglrfhxdx.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gziycqpnk.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gpmtjbjjo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gfabkblkt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gddtrdyvr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gpkwpuobw.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gjqxbjjlk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdbgpiziu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gscbjlwks.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gxinplmov.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/ggnqedpdo.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gnkmwbmyg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gcsfwvjhj.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gjgighdro.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gzwfyldsx.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxqwtkrbl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gvnexurxa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gjixubroi.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gdtldighz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gfumsjtxj.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gwirfuwwh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gvmvnuirk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gthfaceqr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gurtvqnqm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gvwuethgk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/garrkqxdn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gllbhfzpr.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/grflxwndb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gitzbdvdq.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gskfllfek.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/giahglslo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gjfjnvliv.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gdeefjwik.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gzsqfcjye.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/getfhvklr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdixhmfpl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gxiurtrit.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gecgiuwno.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gykjmbfgc.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/glezsgcbd.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvxpynxil.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtkuffmxm.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxkpsvtqr.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghwjcbnax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gclzidamu.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gkymbzdbn.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gkivkaewi.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gqdzmuvif.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gkgzybaky.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gsdnfgced.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/grkxrbfej.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gnjkphqfy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/ggheizxiq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ghllcsuoq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/ggxhtiqrm.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/ghxusphmz.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gvhlwncvi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/ghbuljofc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwswxsekj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gajxczpbu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gmoudccxw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gjbrzsmug.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gimwcqsnk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/glapftajb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/glmdubhfx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/glwhgdmdw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gwvmbdfoh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/ghnxqhshv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnfjvhhdd.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/glswjvnln.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/glnoqeldm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gksvomaor.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gxalafywb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/grdczgxzg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gujguznfw.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gsspqefpi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjixukglu.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gebqprpwy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gfrrillpr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/glhsmdtst.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gxyzpghuc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvgcvovli.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gslwezuyj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gsdyqmfom.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gezvjqylb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gwfgfvnou.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gmnurnaxp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gkrqsputc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbkhtddvd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqtwbagy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzddshxgm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxftjnbdi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/glqxmoqsy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gsfjqnfsb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gjxqotlzv.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gedgkniqp.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/glhnrlgua.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmncnbzve.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gchlswamt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glvzzpdaw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gciyomuux.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gwlornoeu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/guekahukj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gociskzyg.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gsorubwgy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gaueqspqb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gklfmhpcp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gflzvzyzm.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/grzsvzlla.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/glbfnjmiy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gjvhypbia.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/grdrpzuse.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gcemicqyc.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gozytebrf.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gdqdbdjrd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gluclcjpd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gdubmfajx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/goynsohyd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gptuuvjcj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gwgnqjdbk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gqbmtzjcd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gpyhoyrca.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gmjwbkovq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gqhkchbev.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gtfmxzmux.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/guswqwrwp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gfopxmnsz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gbucsmkpk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gkqyreqkr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/grqbmvcil.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gbkwbqvoe.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gqhdlkeuf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/giyblwiuu.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gnqrlycmg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxbdtkqmb.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdrropkyh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/grpquohkx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gqpghywpu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gxywrgpia.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqvkkypvz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gkigktuzm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/ghkygoytd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gzpetbidl.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gozezfcxa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjpdmyklf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gznqaxyeg.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gsexsrulm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gsqovprpv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gyblffkgj.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/giauzbsyd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gbkydhqdw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gwozgtfxg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gfczbsfdu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gncvornkj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gvrmkdfvj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/glnecfkca.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gnxtrdmxc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gkbfxvtzz.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gffvawsgl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gqwnbmmfm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gphszahll.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/guobydujh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/ghvzroacm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gsobaxgbr.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gazflyofn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gsiyxjkrv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvdqastpe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gailrlowg.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/glhvhquyw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxnuvpmyj.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gyrvclryu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/giliklssx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gedsvhcvz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/guqghlylk.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbvlsrzkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/guzonlswg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gudesznug.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/geahhoekt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/glbhmavpq.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gsaeufojx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/geahziwvr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gsiheyaxa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gvkcfivxm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gijpschmr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gpodspabz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gbaxhpvzd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/ghzkwrjgh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjnildvss.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gtpkxyeqg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gwhkelapw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ggcpqwvek.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gnqjmgwdy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gqmtrhymk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghspydada.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gisquizgy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gzoxdfiot.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gzhfmztjs.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/grkreoehw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gsnjqrowk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gqnnccrfb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gbumttekg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gunvjtjja.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gnkztsnev.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gdufnddmv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/glquezwfu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gasodaawb.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gdkgykqey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gbsaujnmp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gasilbtvt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gsxhdiwtc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gujqbgnmw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/grcxtnuos.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/ggrwlcrmm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gwejmwqxw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gxknqybfw.sHtML


<!-- 参考信息 -->