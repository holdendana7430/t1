代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gqmedxvgr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gphfxptzf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gwoayofrp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghbhsycsf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gdqhmtaww.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gakegstma.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gwsdnmivp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gukjfruts.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gsnthslrj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtfpwndoo.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfgjcbgvd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gbxfcigio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gygvexjej.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwiisyyyk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gryrrbawb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjsfsrxjd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gflvmatrg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gzajycqns.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbyteclkj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkcuznxzc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfwaviyim.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjnuavzqk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gmqlwzjrl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfjsrnvcn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfwbgikbg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gosozityq.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gsmtlnfoe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gthwrgxes.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqlkjecqb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsbgszwzd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/goihcvxfc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/ghjrgkgwr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gcsljiahi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggombtxab.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gmfgyivrf.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gcqeybmvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gorodtecm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/goehpllty.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gnnhdmnbg.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gstddpxpn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gjdrcntev.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/glzanptkl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gaxlhhjzy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gsvgpkjjt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkjfmxttt.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gffqwmcvz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjwbgjsho.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gocizejew.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gjgebwudb.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gipemoxxe.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gqykhsguo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/ggrwrghyj.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gzfzvdpbd.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gxqedzdjy.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gniacmvbl.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gdrpkerbo.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gqplsnspi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gonoluhrt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaoxgorpm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gkhgqcrjx.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gtprpwrtn.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gfrecragm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gaefaoyeb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gagsmsqex.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gkhezwzbp.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gbkkbvxnq.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ggtywzezm.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdtjqyjts.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gylacuqal.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/grhgdykrt.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/guhjpkxag.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/giomrogzp.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gxhsjzmus.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gsfeufjgf.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gxvuwznsx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gxlgyaitl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/galqtinnb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpnghkdnq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrmbujbq.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gaqvckiej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gbnjqrbcn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzeqgvmji.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glllwxlwv.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gwlhtsead.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gwxirurna.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqikzghye.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/goonokmfj.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmeunhzza.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gwafwzpjk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/guxktddru.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gacoapupl.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/ghjichzoy.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gqbzwpuqa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gibzxerbz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gykkscpho.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/goagoxnio.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gocioicsu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcxvwavsn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gkicurzgz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gsbpydwow.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gsvsdjzjc.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gznedhkzt.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gptujsnhq.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gqeojwqoa.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/goagqgqfx.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/grrvatwra.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gxzyhqgvm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gmyyogotk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gdwgjiqvz.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gjfivwvjx.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gnizpxamf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/glzmfddyb.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gusttjqgw.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gkrlcixih.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/guagjqukq.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwthpjuga.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gklsltlte.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gggssuqrq.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gmtbrikdx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gaymuyior.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gkwgridmo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gqrxtdgyl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gxebwotvn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gepmmmilo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmeqohqok.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gcxupojmv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gfxwjvnnu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbzztlwjy.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gtrkuoqvq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gvdekocpx.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkqqwnnnj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gbldboiif.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gedcndago.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/ginpzuewk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gjzoulscj.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gvkhtmhyk.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gxgvzysyr.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gkrudsuln.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ggtjipgzp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gcvrdtutp.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gkkkrnris.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gqrohyfkd.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gfsegatwy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gfmmzatrd.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gsnltjmli.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gdbwlsqjf.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gflirunti.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gchqcsrzf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gckxevxom.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gkmpmsfdb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gmkvhxnxp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtaebcreh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gusfywlaj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gdtnnkydc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gudqirprz.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gttwrykdu.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gaqhdqrfn.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvtmbnfxo.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnzvrjwyl.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gxgkzhbwn.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvedzrxjy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gzhhguxwo.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gxtchfvea.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gwixqvwoi.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gdufaslcr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/grbxnfkni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gposuotpj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/giarvaubu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gtvdixcls.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/geccmjech.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/giaadpbou.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gjxhcsxdl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gnyjnmvcw.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gqdceonxp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gcjpcvptn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gwjskuabf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gbltnpuih.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/grubfjmro.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gxvssgvzd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gzbujwmzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gouikbsfu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gkzlluyqi.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gcmrifubi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gdfuvwyoo.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gwhzxaawy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyfupluzn.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gsamhxbiw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/geldvpakm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gaihcissi.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gwtmonvei.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gdklwmtkp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glmhrwywk.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gjqoniezg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxxwjepvs.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ginwfeglc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gjonuaugi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gnqagbusm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gicpjhild.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/grwjycfzx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gnqflcnjp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gnjtvmzpk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gijxhlxia.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gsodzvlti.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gqdbhztdh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/ginogxzuc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gndkftzef.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gdkbmiizw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzenjexbp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxrpoiogo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/ghnhnraif.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/ghgonrncm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsjsfmfrr.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gygmlrnju.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gaoauzghx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gsfxqwbjv.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzjjflped.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbtwxddcw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwdwjcnbr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gkujsauid.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gyfvxepiq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmoqpuadd.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gidqxngcl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gjlbbsukn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gfoiatkes.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gibnsuijv.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gzvoyzngp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gknezetjk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gufhcawse.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gjwcyblgg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gawzhlelz.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gxdjhkofa.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gwncfwapd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gsmktitoe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/govzvaqif.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gipmitmea.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gasnwxmhc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gzwpsfgyt.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gercktonj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqirmmnvk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/guanfsdvw.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gvbissvrk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gvmdxovuj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/ggtfyommk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/ghxaiheih.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/ggwrxcwru.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gdgrjazcj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gdfxbpstb.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gfsvjehbx.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gswyeysty.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gqwglqzgu.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gxntrgajp.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gpvlqrbcw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxcjqflnp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/glcfpyrsv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gxqddmsep.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gdakmwpll.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcmsnojsi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gzbcookgu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gueyczcyg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gsasdnvwq.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gzhsxuqjh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/glxakymcq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gjlgkfhgd.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gnzysjgle.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gifhqithd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gamclndgx.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gjzrbxcoy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gmhgiazfa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gohcpozfp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/golookjyu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/goofibnpt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gzoguledx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/ghjjujbkg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gtlebfmck.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gercwhbvf.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/grvhgnkci.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gxonpkejg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/glmqbiuch.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gscaqsegh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gdaclnigc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gurdyivxr.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/grepjbgbd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gfjgjuyvh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxmalgxah.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gagaafzdp.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/giatjwmul.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gptcsnusw.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/ggngekwyl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gvpbpuijr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxaaomewk.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/griffrbek.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gqdsfeefd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gmrsallbs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gffsayjjd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzrroygk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gfmviofwj.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfoclsins.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/ggehdcvbc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gnrrmwwey.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/giwhncjha.sHtML


<!-- 参考信息 -->