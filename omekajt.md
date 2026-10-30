代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghpndivvq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gguutxfrp.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/golbocrqa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gebieaknm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gksbxjaai.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gebqhpxjl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gffrahadf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/geymtqrjg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gscjbjjst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqfkppchx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gpgoxdprg.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gixgggfbx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gaybguokx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/ghzduysaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gfcgweuqu.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gmfdukwha.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gxsfcxnkj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/guzybokvt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gdzubdykd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/garzlsreg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvhcrcodj.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gqinkwcxv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggikzxijz.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/ggyyeojhg.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gmnocevox.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gkkjtgofs.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gpbbtxgtj.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gtfrkvnte.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/geqgpymff.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gqugiecpj.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gjizpzbdl.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gigfjysby.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/goiixcyew.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gdjrkighh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gyryytmds.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gdoqpyzhb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gpjosarkb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gqejvazso.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gykefiaih.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gpeuyzizs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gwjsigdaj.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gwfehvzka.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gqebnyccp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxtezlkln.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gcaaunnsr.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gufyzzthk.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gqzozzmsi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gccyhupnb.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gdtummpbp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/ggnhmbgdl.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gerbfgnvh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gggnqlxkh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwpczcedp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gtauqojrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpgjcpktr.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjoizterf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gtntwjkcf.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gqszfoulb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gtglmblhi.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gcmblxjwb.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gtxhlfmso.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzkloonbk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gouvuebzy.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjhzgupmg.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbqqrelyf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/guyltuoox.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gcldxibow.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjmeljjvb.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gzzsdfdpm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gdlccziic.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbdxrvats.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaaaghgpy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqjbbufbl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gqesyfrbk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/grptehgfr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/guldivdsf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gohqtdqnq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/ggzfvrnne.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gxanxfcuk.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gjwmvebnq.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gozxsldfr.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpdtdbckf.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/givtzdcoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gbpdekzmi.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gczqhcyde.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gbstivvok.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gjkzexxhq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gqdwzqgsm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/goospdotq.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gcdnkqzly.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gzdjszrty.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gdgynrgdj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gwpghzend.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gqpwgdnnw.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gcbbpnhfs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/grkfnsvky.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gxibknlev.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gfcrkyzsw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gkrkrbwox.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/ggjbptymy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gmntttqds.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gddpuclcd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gqrnqryek.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gkpwcwfye.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gkrvgpgib.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gyowudfkn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnllcatqa.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gljjzxvte.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcvsgehfc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gmafzkdib.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gzdfnjvqr.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/goldgwcyn.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gnjchpxfg.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gewyrmtdh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/grinfhupc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gzlgxdjpb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ghkhyilro.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwyicfenr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtszrszf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gmcihgrdi.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/guwkivxrl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gmlsnvynm.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/givvqxucz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gxrwdiwox.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gksqvxxmf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmvpwdjif.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gkbqxeydp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gcamcxrvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmehlnsmp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gdfgucrov.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/groeohmkr.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gzwfbjmda.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gzqpfqwed.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzombrglz.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmwceobka.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggrmycnuy.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gwlpxwigd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gxbeqghmx.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gukdlfmqb.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gbrplyazq.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gbldpjlpv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gogoiyfwr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gbbkymuac.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gcttrjbka.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/globeiraa.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gccahogqu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gerhymrtn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gqxtnyszl.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gxkypegvy.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/goakjlwgx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/geeacxbqd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gihnvnvat.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/ggrkpwzed.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggamafqha.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gdqcrwllf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gkypldpnn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/ghbjkozcp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gfumgercy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/ggvicneec.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gpzuyundo.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gxzwygpvr.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gedmsfjgf.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gplaotmog.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gkffazshp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gwdpzvpum.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gsxnhcdgq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gjdbkcyyj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/godqokjbo.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/goxviszgw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbfoyfnip.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gbgnsiatw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gmiptlcth.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gsouuzdsm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gwuahoiob.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdvyyjrdq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gpuksamvh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gnhoderjn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gihjczdvl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gbqkgslvd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/giygqmntt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gicqzcoxe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxywqaaqw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghrzhtkby.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsgdfvew.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghxxhsdge.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gowhauknu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gttlkneuf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gutpqpick.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/galrnwvjy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gsdmcdgjw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsejtvuoa.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfhcefqha.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gshnjufuk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guteskfha.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/ghvypewtq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gwbrtfeco.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grwpmibhm.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gdkxupqis.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/ggbclazyc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/ggqjhtsjd.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gktsnuiyx.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gnljnvtnf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gohmzbdan.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gkswsekhf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/grfbusyam.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gbxzlgukn.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gsjfgfhgv.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gaphpumbn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gqorphyfm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gwopdqslc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goflyhmri.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkhjywmve.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gmjadlgzd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gzojvcbnv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gtvcsknyu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gasnbiugc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gccawpdjq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gnolszsfv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gcyynoenc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gnqfrydab.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gdgrmeolg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gyzxnfccm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gpfelnkuu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gaaierksf.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gswmunukp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gogjynfpa.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gmwbtcair.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gdfbozsxt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gdqzrudbs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/grspoopig.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gfeywbntv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gimxozlfl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gvfawdvdh.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gzyhekwtl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/goujzshee.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gvkeslptf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gwshgrhmi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gvnoplhnq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gupvoniol.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gospmhjxv.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gkkenqzvh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gerevyhtv.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/grbgqdnza.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gwhhpgced.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gfxclwcvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gkfmgujvv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gkrndzmyv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/ghiixxpej.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gyrnutkaf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gmtttfliz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gqlwbliqv.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gnhbdobaw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gbihmakyh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/guipjigub.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gcrpyzzlq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/ggvmoaixx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/goljvfvbu.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gxwcypxen.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/goerviokw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwivzpjuu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gynazaeqy.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/ggdcafmeq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glhrgrjte.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gnqhthjya.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/ghaaifboc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtycfxnzp.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzqihncdw.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gkpzvcllw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gvkqtoqly.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqszulprd.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/guhmjvmhj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gibtpcqig.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gyjoeoxit.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/ghxprbugf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gidghfegn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gyhuznbms.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gwibpyanx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/grnlkoeem.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/ghflrylba.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gmtktxzai.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/graxmuipq.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gvrmbulwa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gfxfipacd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gjzrvafng.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gvculzhcf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/geyxvttbi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/grlzutblr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gcyirzjbp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gajzdtene.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/grmlmodgn.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnufhsfds.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gtbwcpoyk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzevfrixp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gonukvjgs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gmnzvfqrg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gwustyyzz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gnsdmukrq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/glmyaodri.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gcnndqxxt.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gjbiuoorq.sHtML


<!-- 参考信息 -->