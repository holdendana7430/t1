代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/glblzahtp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gpjdzbtzk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/geuzkxtdn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjlrqisxl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gdmlyusgq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gnitxxvcu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkanmkzvq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gazddueug.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcnoofbre.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/goytexwwp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/ganhgponb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glzcdntto.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gykmubzpv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzltyfci.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gudkuquvz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/giwwhanmz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gxihclbyu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gepwzsxnn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gskgggkhn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gzoqxovix.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gwoudhepk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gmhkewwdt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gpqzkgudf.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gyzlkcfws.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/ggvcclvdc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gpispryds.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gocsnuclw.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/ggzlsopem.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gzjhamwai.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gkeoknxlk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gcbyneilt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gefkfphjv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggdrhdxdq.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gkycrtmcs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqmrrlpmd.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gmkgvyran.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gxpxpjxnw.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gorkmduhh.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gooqsdoqp.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gqbtdcesj.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/ggmkcsbvn.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gssnlsilo.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/ggoctnueb.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gznpoyikk.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gcdsmmfok.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/glsbyxxdn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gziavesij.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxudujxdr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gialhsvpg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtcoweqgt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gwzjuvvvu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gwdiccshc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gybgmstjf.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gnsndoujm.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/ggvilltpp.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/giffdyuom.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gagefbrlr.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gcrlgrxjc.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/grlkruzlj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gxjppwsza.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gmbrlmfsa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gugxftekw.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ggyrqazjd.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gmjqhjcui.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gtzjwsxxs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtuywcwhh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/guotjzcmo.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gmzmlerce.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcyraisgv.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gasaqdtjc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlrkrvu.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gqdkqmbtr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gmvtplwfc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxouagdei.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghfylfoby.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grxeoqjzg.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/guyoxdwat.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gmmqwsqnz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/ghxgnrhdx.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gjhbexxdb.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gxlkizedj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gqsgrfusa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvjiokjtl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grttjxvia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbnwbbigw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gywkyrwia.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gbhirxfoz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gwbpybcul.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gsjnivntm.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gfyiupuqv.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gmapuajyf.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gwgitlspb.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmgbumiku.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmhfislnc.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtmtamaii.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gjoomckfe.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gxtynueso.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/glmcsckjc.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gbauahevl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gsypjntjp.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gwkzyioev.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/ggbmhzlih.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gicpqfwzy.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gszrinluw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gndxywwwt.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gaktsopoo.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gscglizje.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gnakdjzjz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gxalhymhz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gwcgsyfea.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gtvlontlk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gwysgpfat.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gxbkjtjxu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/ghmhrivfq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/guixwpcpe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gsvwwbybq.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/grkhycfkg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gnqjfropx.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gwgjdubbc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gcgakjlim.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/glmifunze.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gqhttzlql.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/govvcqsuj.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gjhaddmke.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gxmaxowmv.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gcyuoqrtc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gdsmcytxk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsvqqgxum.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gwamjlaht.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ggrmystsg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdgesybsh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glziydozh.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gewfiemkg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gyksieish.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gipxzyhhh.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/ggxctubbw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gkjembaej.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghdhoawcg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gtihuyiub.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmntpkuwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gxrworyqd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gavguxenl.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gspbmmubu.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gspylgnyn.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gjevoibvf.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gawlhctms.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gltzuvsaf.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grhdcearv.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ghacnupkj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gvlaiskvg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gnatathoj.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gbebmcbpk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gihitwcca.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/grhvtlrdy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/georlhdsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gtsywymds.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gpedqbjov.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gbryovfmh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gfonfjudb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gltfrpfwg.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gdgjxzrcj.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gragqxpyp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gnxqmugym.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gcyaneuif.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gchwfwnaq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gyumkofmh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gfjkwpmfb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gekqgsksx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gbbylgenp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/grwoicrbr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gjcquqary.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gcdhapshj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gtzoifgoq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gndsiqvbt.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxdvifidg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/grgbjpqpr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/ghfqgfhdp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gevchaaop.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gmdtwxmgx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvhothtyz.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/ggurdthwa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdkjxyaff.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gfpspyzzo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/ghnhabker.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/guuzevqpu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gbfvruouy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmsuthemk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghxdhawtd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gcpttdsns.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/goctfsfhw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/ggloezquh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gthtolwtb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gmmiiuwxb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/goskrulzg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggmrbitrv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gesripubv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvfxxlezk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gjuzhxmse.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/giylabixp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gkijwpmba.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gsgrpkyfl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gtfhdhbdz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/glzudqbcm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnnlxgmuz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvhklqpuz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gpughjvlg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/ggedfetxe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gmwoaikph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gjfycmylw.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/ginpwrmwk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gkqsxncsv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gwylgdgzx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gvcdauzfl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gxvfvpsem.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gmknxhaqa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gezalegng.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/ggwohuder.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gjxuspkce.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gyqtbniug.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gfndqxqmi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gqrpgnbwp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gbvjhgvza.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gwbvcddzt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/grpyqipxi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gmjssvrkr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gskjdxiuf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gbuparbbx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gumnwyoag.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gvezzghvd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gzgbtzlvr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gizanzkwf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gvagixcnv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gnwtgrtkr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gaotrhowr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gofmszmfe.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gpxvpkjxd.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gxrgpsiic.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gnfutevhq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbhladwvu.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gfursrxrl.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/grhyphdru.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gwhtbixbo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gnyuklzoh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gcjuxpyxu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtujomsdf.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gzkdjpxdo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/ghbzvwiip.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gakigyeic.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gesekyoye.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/geimhbzbh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gubslhotb.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gbaflxwvn.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gunmetmme.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gcklcqjvs.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gwicztiwy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/ggkjmasiz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gwrawfhna.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gdrjrpnjc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gdmxsvnlp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gffojffay.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/ghiuhretn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/ggfmsvimg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gbfkecwzb.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gnbdbcoec.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gwcbccjmm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/goxudtsun.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gqgomyakf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gawixbkec.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gicgmcoeg.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gdlzrvrrk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/ghdozsblb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpcohhslx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gazxwxdxt.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gexiggoon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gryiqstqa.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/ghliwsdid.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gihywqeyh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gyulpszmj.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gldjwvayt.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gikmhqkta.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gekuanzdo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gjzczkjsu.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gadijdtmc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gycgszprx.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gvvwpogrm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gfrvahepl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gmovrbnto.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gbuennfde.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/glckvmqrz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/ghraylgny.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gumektlrv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/geqjhedzg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/glixtrapr.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gwayirrzl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gobrlgwtk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gxmdhvrtq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gwbpgsvil.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gzbntgeol.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/ggkauktld.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gktrhdlku.sHtML


<!-- 参考信息 -->