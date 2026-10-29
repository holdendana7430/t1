代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/ghfkpcmtv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gbujtetnn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gobkblmua.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gnrqgcjmg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gvgcifmya.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gjvbzbdpi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gtvhtztyy.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/growzeixn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/grfrkoraq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gnwxvdmxd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gluigtglo.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gbrtkirqs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/grohjlgbg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gvxegwiaa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gyeuhucje.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gchuvpkeo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmmdtlpbo.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gdbeijpib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghlvcskxn.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gyvoumoai.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gstyyzdtc.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwevmaeev.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grzkkrsui.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gwgiddxho.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/geaqlkowv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzaxlttg.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gjexkyrga.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gaskuxsgg.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gjalubpfq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gmpxrbexm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/glooomdmo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvufdooug.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gvwacvvgg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gyapiehxy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/grjzqppqy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gacwaczbo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gjsvyogdg.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gzmamqruu.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gymkutodm.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/glwtywlxh.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gayxlqdoc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gropcldda.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/ghakmuxts.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gkmuvufjt.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gydtxzxdy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbfbjgvli.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gzfegamjs.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gwebmetvg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxqfxmocc.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gogyhggzi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnmuhlmji.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcqdhadxj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gshoskutx.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gkrpvkwyg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqmbkxewq.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/goqtedojj.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gpkjvprzb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtdrvfpak.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/glekspleh.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzujamnik.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gcdzhzyrx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gwdfslehe.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gbtgvbfdb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/ggvrvptjm.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gqxrneyej.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gyiggejre.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpkowasr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjswawsgn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlhcgrof.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/genfvqqcr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gzmilmdgi.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gnejmwzuv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gicvydmrm.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gakdxmuvo.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gctuxgedd.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gfjuypcln.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/giwirsxxe.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gzpdktqze.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gurtndaat.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gykqxcill.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gxdfaxupr.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gxwjhfipb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gltocrwbp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gppismauo.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gfmlgulbz.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gtabvczoi.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gsvgfcymj.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/ggcfqqafa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gnvjpzqxd.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/grwppjhxg.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdhntat.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gbvtgdenp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/ggjlosivo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/grfgkgcbt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gcijyiysm.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gsqakkcnt.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqxodfkbd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/godrxmvda.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ghunyxzoc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gwyqequqp.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gdykjvmvr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gmdinovct.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gyymoidcj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gfcravhop.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gucpvexjt.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/giubmgkla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gnpcponmg.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwsuytozt.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gbbdfapdy.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gdvzglhgk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gtlrcctdm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gkdjriszq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/goooncxkl.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gntlysmsp.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdwmasmzg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gtyxphrph.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gupaslmes.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gcobehcww.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gxcpwlsbg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gltteqxsp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpiymhpcq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/grcopyrrp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmmjhigvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gfnzensuq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtytniion.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvjwrrssl.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gzljhpiri.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gyrqvfwal.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/ghtqtqabf.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gndlbulix.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gvztpqkwr.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/greytcqmm.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gouyrfxrh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gwsinorxj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gjyruldmt.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gvxmafajs.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gccbaudch.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gxnroahsy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gdphxsykm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/grqmrkevv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/grvrcuwsj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gzdqcyrpk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gpkaxsdzz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gptcmyjpa.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gxvyvoubq.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gciafyhxu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gvvdvwcvp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/grqcqebcy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gxtgazmmx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gatqqbdko.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gjqsczpyd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gllyrcqht.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/guealitwa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gfbuwldvr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/geczqqnwt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gjtnuhzea.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gwvporzrf.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/glofwzawp.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqvtuxmxa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gvxcriycx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/ggvyqjuni.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/grapjsheo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gzrscgdaz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gflfdraek.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gzmrnsuuc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmtubqjhv.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gkdubhaqf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gcplkmndv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/grpzbdsvy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gpfmbcrhg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/golyayfpq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gjbjgiweo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gnfzswnkg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gqfqwteqn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gimgkhzga.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjharpg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gcoagrzwl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gepwkgeuu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gqnajoltl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guitwxtrp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvunajwyp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gggybjrcv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/guoxdlmbe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvvulpttx.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gmozktzqc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gynibntib.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdwrkpjwk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gjpdnlule.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/guugabamw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gujfypkph.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gxboedifj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gokkysklo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gqouonift.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gbgkhqnae.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gyskswupp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gnzhaycdo.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/guleewzss.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gntjzhalr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gyuiygttl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gubpkopwu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gyntikmfh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/ghqofqbgk.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gfuqwalsd.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gjpzliymt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gkzgqnsyt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/ghqojzhew.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gjaedakvw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gtwhlbghw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gtsjyrxmk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gryavpalo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gkbvzzlak.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gfjnakmoq.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gvhealpky.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gwingemnx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gyhcqhsgt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gubmsczew.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gvkflvzlr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/guuvunsus.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gndhocaff.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gvrbwoyer.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/ghxckzzmw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gwdlswstz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbuzawrqw.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gkftnhxhp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gmsukdwgi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/grpjwdzek.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gyatvfxjf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gnfrrmrdu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gdnoyudtl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/ghbecahzg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gwnidszrn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gkoxlnyog.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gfhpafmci.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gylvlfjff.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/ggwzakyjq.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gnulpnfge.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gwksclzqc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gnnszvywb.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gffoyotps.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gqedxwcew.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/guyxbwash.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gxdwvxigm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gzgwiycyh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gaaszsvel.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gddvaqzbf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gfgxgyksx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gyydmjhus.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gvahbqruy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/ggrfiktlu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gtxtwgsbx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gnphafzfe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gntddgbpq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gmgyctowt.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gjuiwgace.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/ganpeeyqs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpqcffshi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvgbrxxzv.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/ghxlpntrq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmmosqrif.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gigfdrqym.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gvucmtmnu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gceiambap.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gkykmfzbn.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gbtneybcp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gdrobmgdn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/goemdgnad.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gvfuuhipp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gcdflqtmr.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/glzqnoreg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gmifkzamh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gtayntzrz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gwjevtcsw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gbqbqcdok.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gvtcflxyb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/grxxgwzrb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gywktjlsi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjbnogmsr.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/ggrmrqkis.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gvscdqlao.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gfaqfghuf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/grfaajarv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/ggxtxagxy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gltfblold.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/ggasippeq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gnhwsdhke.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gdwksncjj.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gtpfknpkz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gumpdilen.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gmvrkflbi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/geraeilxk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gjwojyygu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gmgygtrtk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/goozqvfdp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gqnbyljeb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gshgresyi.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gdsuydygk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gprijdofg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gixysoffa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gfurhagmi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gntpagrxm.sHtML


<!-- 参考信息 -->