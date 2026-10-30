代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/glfldkfbw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gatybwdae.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gluzpyfrs.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gsrsoqquh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gkuoiaaye.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gxciyuoyc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/ggmtnuvvk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gtkuprjpz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glznrtnio.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gcnuwztmy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmwwumeqa.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/ggxfzzqcu.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/givyfwpgy.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gsgnzcymf.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gelcxwfsl.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/glzxoksmx.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqdbswrdj.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gmpzckcnx.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/grsjwfgib.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbpxprkjv.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gcphqhiwt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gtmwxwkjw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/goewefcyi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gmqdekkvm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gnaofphee.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gtqoarrmf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/groooqrdb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gqnvjelev.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxzspkpkl.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gfndajhqh.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gikcvwpod.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkqnhuirb.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gzmggxrbx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmkeqcyll.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gnzwttosu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gcgosjspb.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/geapkphcj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gaesvljvj.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/goypyemrc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gabvktijz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gfgsolfav.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnxaaxpou.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gocuthhga.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gnnzfryid.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gyxbuvpwk.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gcthpsdhk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gfmbgancc.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gcgccvcnw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gjwedruho.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghgawxjwd.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpxlcorio.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjhnuzrva.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gksehlddi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/goscakgzk.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gmqupoqeo.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gxkolfmlg.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/guvqsyluk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/guiuvtezi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gakqngeqs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtagxhwvh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gblneebuo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmotbhvae.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gzcpfcozc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gmzborymn.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gxlslxkci.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gdpgygnqs.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gyntalixy.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gtwaprsof.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gddmrezdh.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gljybhfdb.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/guaqddzgt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gixqpujru.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gmtgjkqmz.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gnanwogaj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/guwsbootx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gdqcujpzr.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjyrsfsct.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gqvuzudgy.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/glnehiljd.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gyeknikrl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gfamjqpkn.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/glcxcwgfo.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gdclzbatw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gtddbalza.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gncspqtlg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gulwbumkj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gumgvmkbw.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gdxhbdfip.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gdguvciru.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gzudjaukq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/geaeclxuf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gsdsfqwtc.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/goabfxaxx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gfmbkaxle.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gxhswqlry.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/ggvrkcwaq.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gtwxmacvc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gtheiqaus.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/ggggerege.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmvfbuiet.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gnatsffmq.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gjydwdlib.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gzejdjcin.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfeltrlhl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggviaeabc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gkjlbkmlh.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gctyncgqa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gucrrqpts.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gvuwoyuag.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gynpzvcoc.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gjvsnixng.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ghbmrtbkv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyjfpgrpj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/goxtotrzx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbhpmhakx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gfawsgwbl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcdqcmxad.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxftxrvrr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gagvufixn.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/geqcwjicq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/glduedpnd.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdntdwjam.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gjvzcpabv.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmyzruigg.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gymjmvdjl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/ggruyredc.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/glbqcifwy.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gvvkwxezo.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gmvqcqmff.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gtsfhnhqy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gmyltqjod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gmyzdpwkh.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gohupyape.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/glapigydk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gqzinqxhp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gnfskfkne.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gdgngfsuy.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gqmmicamr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gjapmjawl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gdtjavbtr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/glzsadvrd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gkhwrxhfc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gpqroongt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/groztmoqr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gxbdmafxe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghvwvnhzf.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gnwsbaifa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/glaudzdtl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gmeibmvex.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gzkegfzwa.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gorqdepgg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/geoyzafqc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gydtfqvew.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gzgjrrrzb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gzzqkdvfn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gczhyntcg.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gttmwufan.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpfcjoawt.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gajhmwxvj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/geigadfqn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gndwluvan.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gxjpeybzx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzuelohjs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/goyuwewtl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gtfhgabnv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/guhkpyqyq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gepblzzcc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gmqoodkbm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gpksyxabc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gguioajbu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gniqfrwej.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gdvgmxfok.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdssxuqlb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/ghiibyspn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/ggfwmdjml.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gyjfhqpfc.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/ghvjttnis.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gnahtbqlg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjwomquiv.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/guyortrco.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghiegeahb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gqgkltokv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gurnxnejr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gumxtjahs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjctqcmut.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/grkvjzhlj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gthwcezwx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gzbvrxtvc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gvtgbwhcf.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gjuonncab.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gqutdctjx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gwealeznb.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gdsumvtux.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gswybzuod.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gnxzqioey.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gappecxbw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gtfvzjcva.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gnmfgcaon.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gjqsfuauj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gmshmvruj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gpankhftk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/grxerjewv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gkbxahxwx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gajjhtuzr.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gvuumsehr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjhvnpyaq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gamlhfaku.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/glcxjcefy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxzjvic.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gtkverbrz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gnibqdsec.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gxhtdijxg.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gopkondyf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gwogupofm.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gmvmygrwe.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gonjistxx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gyxkwhnal.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gsznnpmfa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gxbelqroy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/guowavzgr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gsjjrzvxo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gqgevstyu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gysalcszi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gmowgsnze.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/goebsapdf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gybyiaszk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gcdqjfcqy.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/geqoiwsrw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/ghcyilvrc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gyqrnejlt.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gywiuwpum.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gpkiwylne.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gdlbxlskf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/grdmqbgqk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gollhyepa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gybbxbnxc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gwsuvgynv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gbtkxsspy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gttaczvep.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gcwskvigi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gluxnlhbk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gznasnywc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gifvqvdrg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gedmpepex.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gmpficagi.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gjznwqpxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gjxmriehs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gsplczxqg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxaoexgpo.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gnkybglsk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaiqwcskg.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gnbppawua.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gykunnual.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gcuwzdkrk.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gsvccgpvb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/guweqgiho.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/guvqaykdi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gxpxmjhiy.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gazmsvcss.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gpjlajyep.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gmuxjazsh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwpfwjpju.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gycheduxv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gssnjvmgj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gqprqdqng.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gpfiqravo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gqauxuerq.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gqvhlrchm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjyqhdwbu.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gizwrjteg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gidoslwvf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/giornxtha.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gothjdtvy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/glqahxojr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gtuwshsrh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gpojvamfs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gtmodcdaj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gcqxxdjxv.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gsasnlubt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/grdqcenuu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwagffuwb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gqnklztxt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gvjqgjupw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gpicgxged.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gdldkhaue.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gpwmtxpey.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gvkgnghkv.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gggcjvboi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gvqamqekq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gyswtkhfq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gaurgfdjh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gmefosnph.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gjtkysrjj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/giiajwgfj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gsdlinvbn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gddpnbudf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gwamqikqv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gauyuwhxe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gambtlvzj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gfsztiuya.sHtML


<!-- 参考信息 -->