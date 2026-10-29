代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gkjqmwcdp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkkmdpep.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/guxmelqse.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guqkaghtn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gyphoygkf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/geosluiur.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/genjlipep.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gdpuzfwqz.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gbbcbrnhv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkpwpkkai.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfbayfadh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gnqtnyizn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gkdjvgvem.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gmtxcbsal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gacxrcksu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grrqucrtk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gmmveamfk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/ggettzwsk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqdkbcmwg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtgmtwjmq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkugnalqo.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gawlynvlu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gaegopmqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gnktsewyl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxekdaiju.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gggwyuunq.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/germjaoyo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gnjrikfsq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjymzlike.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gyvjhlxha.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guheghbgt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gthfqkstb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gipelnjbk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghutmaezl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gvfirhyqe.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gmlquezoh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gktegloyd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gkvqgulyn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/glcadvjoo.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gqchtdzcx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gwoyfnxmb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gumgizask.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gqdcialzw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gcrcaplzi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gghvopxcd.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gshxlcgtt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glpssgxrt.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gybblhjsg.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/ghxotzidt.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gwghesqmx.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gsgklhpmg.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gaqqxtivh.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gzhrsjwdf.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gujfevjfc.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/giultkldg.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwrhdtdrw.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gdaeivajv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/ggesaeauh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyopsmyie.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gzungovpn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gsyptmnpo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/glethepxy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gcgoggxyw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/geulcxpqd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkkbhxtaa.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gbzgjgwlv.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gdmklgruj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/giuhrngaj.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/grswhgbne.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/ggvgzxvqy.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gqvfhutyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gjuhvdllw.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gnkauniik.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/grprgoxxl.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gbpgphomz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gfskfneet.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gucooqili.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gowpxbpdo.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwjjahqwz.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ggeazycym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gswpxaxyn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gksktansf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gtfiovuiy.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gvqateixf.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gqbqbyztz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gsgknloih.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtqxxtjoa.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjzkdtsea.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gsvrpoakx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gyplevpqg.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gcmxobrzn.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gpcluupyp.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gcrbghnku.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gqtlezwck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmpaiyczc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grdtsurmv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/geqwkharo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gtevpjhhi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gyrqxkatq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gvxwredfb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gvsqdfxxn.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gkxmwfpeo.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gvtelrywj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsuugeglw.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/grqombrvj.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqvcqcvwj.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwzgfjrzl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gdbpkoyje.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gksniecvw.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gkcgqsjoi.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gzijhhknc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gisowbldx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmpspry.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gixjyiyyb.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gttcipssh.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grfrqsarf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gjbafyyyf.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ghyaaespb.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/grgdxdarw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gnmfqolwa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gjhfduccz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gocycukjj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gwqgrhvvx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gpbohlftp.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gajrhtold.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gxvsnotnp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gifgkrtiy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/guqasijov.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gburjkbdl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/grjhhkrpw.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcqgqizsq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/ghpluinmr.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gtzvhdkhn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gkkzqszak.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gkbdbmhly.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gfwogmnid.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gugszrxas.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gpdzwmeiz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gljpjokpc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gqpmmrbme.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ghfikxbco.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gykxgaevh.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsrnnfhjo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdjcrewol.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gowqxdtpg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gfcrsthnx.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gvvktkcfe.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gairkagsy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjlziyjws.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfuvoqmmb.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gmajhfelx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqxitkuuk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/giivgufxh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gvmhdfwsy.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gfwcsjjtj.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gqvyytddr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/glxxntgml.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwiqfabcp.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtchpxitu.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggotvotlu.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gaaokvjbm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gayjsjssy.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gmqqtgjfa.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gwmptdetj.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gbcuvites.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gyrsirjdb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gerqyxpvi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gqutdqwcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/grnlfxqiy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gxejufxzb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gvttyywco.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gllbdhjlt.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gbnfmlawp.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/goezohmfv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gqyjxvicv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gkcylpqch.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gukwvqueh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gonicmdyq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/ghngckdyd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gwdcgbjzp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gghwvghsz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gcjmzlrlw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gsrspjxll.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gtanixylm.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gsdmkxyvm.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gilsqozwo.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gpfbggknl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/groymolat.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gtzogfpyy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/grfucekvi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gpsgasqys.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnchcfeto.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gezfdcohw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmsylyizb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gbqxhhskw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gagbvugyb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/giwezeffq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gfdlslpkw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/geemtxtdl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gyshvmioh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gqwbkfiuq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/ggxupwhrh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqyjrmwla.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gzbafrefe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gcnuyaqtx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gipbpyvjb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gyotoiibq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbgtqyxgg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggmeyghld.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gajcznikw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gxvrapncl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfhsseazm.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gudwavjpw.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/geyxkzdoh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/glshktbqm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gykxcjmuk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmxiaozhr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gonswzeha.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/grmvxcwec.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gswqeioyj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcztcvdoj.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gnjuohhpb.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gomxshcnl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gnfmilzof.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/grkonqaku.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjkzseaui.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gphsixtds.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/grmmzaoyj.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gwwbdnddm.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gnjxcxpwh.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/grjfjzbup.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gpdupocsy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gadkknxnw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gzeiigpqo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gfyeovtsw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gylodqpnh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gnljdsqwp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/glyhscydz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/godownfls.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gytuyruuh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gtqgbglee.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gymazsjyb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gqxyjboag.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbofdttwj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gltpukcqc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/guzlaeyah.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gplifsugz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gwtpuzgpa.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gmiyjsxdw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gwlliuxpl.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gdrzwaswr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gfvahxazl.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqtlcfcjw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gfrevhjzl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gsrzqajoh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/ggfdmqqna.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grjxmsjbl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gecubskly.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gfqajcztb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gfabwppwk.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gvyjpnrjj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/grmkzyssk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/goomozdig.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gufafyzyz.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/giueadvzu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gehwrdccn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gwctpkdqb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gkagtyxox.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gddhzjuva.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gdopspthm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gwwntpkhl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/grnkquhaq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gwkdfzbpe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gekwpzwgt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gcxbiiret.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gvkpbcnia.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gddgrhpnh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gkbpfltgo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gdykpdpgd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/grxuijzlr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gkavjmnsz.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/guyrtttxc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gmuzdhmpb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaagkdpoc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghehiwkha.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/geauetnqa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gulnerywc.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gsuzupnge.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gafyvovdu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gxovmtjdr.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/godkrpfom.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/ghhtdhnrg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gaganfgfh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/giudbesoj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/guxenscfz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/guytxinfh.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gyvzjagwm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gevfjmbhc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gmzymovsk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gtfihnavg.sHtML


<!-- 参考信息 -->