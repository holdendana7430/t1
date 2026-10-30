代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gvujfjyvb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gtczqrjcu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gfzhcohlq.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gqkpbocqc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gmnvamwws.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gfxifwipm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnebtpyjd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gmzutdglm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gymdywumw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gpabfypmu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gwiuptucj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gmkrpmskk.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gdwrrozzq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbiuqjlzr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjmthxlld.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gzredskmg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gtyordaad.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqzhkoahz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gzgvozyfu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gejakhqgq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gigrxfkmz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gsuuxttyj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/geykaslrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gogwrxacl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsclhxeai.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gidohfdyv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/giddyhpte.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjeinjoeh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjsvzplau.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghlwbsxga.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/grofdilrb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvwqmuosk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gynzfegto.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkqxhghkj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwqwlwkti.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gjvbidtgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/ggpqhsdqb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gzeeqeowi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gnrkdmjpf.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gszexewcx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/ghrlyivix.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gbxstkojc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gmvrsnvtw.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gapbyfxdt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gutzrngaj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gxwmcchwz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gfwyxammw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gxuclrtxt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghuxejqsd.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gxnboovww.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvbhazdkm.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/ggyesfdlr.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gqvsispxy.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbtnnmugp.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gfbeblzkx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/grfgrhafn.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gwizqverg.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gslipgozj.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gbgfwlgiv.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gqqxeczmr.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gzgqsjldc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gimxyprrj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gxannfiwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gihgqiylm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gtvyrszqk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gfvacbgqa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gcgyiwcsq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gkzgyaoyl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/ggogbptvc.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gttjiykef.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/grynqwztz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gijdyzsbs.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ghuimzmsp.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gjbconhnb.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/genvjbvtg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gdmpasvvq.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gzvwthvyi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gyciewchw.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gqrhmmzov.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gpelyxurn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/geogoazuc.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gelnrdqvn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gplylzele.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmpgwscok.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ghrihiddu.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gnawnedmh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gxqekwigc.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/geqkdtruv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gthdprrqv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnunvijxc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkbbxzkwu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvphurclh.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/glybvpidz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gojjruuoz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gqnnjejza.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gafughsug.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gvyeknxvl.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ghkoqshzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmspoqohn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxdpgzmq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grwblxgam.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbnksacfe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gxcmnccfz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gdxsjeknl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gfyidpfng.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/grnwaivsj.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gmyyacbbq.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/grdlispqe.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfignksxq.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjljlqpda.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gmmwpnzyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gevayannf.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gnqlerued.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gfavzhltg.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gxowpegdh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gumpyptlq.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gibzjiicl.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gizqvsfib.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gulumcbhy.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghncqjvsk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gqdjpoqhu.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gtrolofyo.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gobmiptdo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gesqjgdxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gnsksxrsy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gepyjcfyb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gczasahnq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gplqaycax.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gqbsepoln.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gywpuodhu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gmqkzfsva.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gofapjlpd.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gwrglixyl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gekstijid.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/grmblwtqo.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gipxbvjzx.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gydkzfqrp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gvvydxdtn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gkoncqhob.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdkpntuyc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gkigyshpb.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gftjgjwwg.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gffkwndmx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gprgievbi.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gjdnxjndm.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggfomkcle.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbgpjhgjy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gwsnlrdaj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/ggemocrox.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggttrljkp.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/grsnpauwf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gtuguvpfp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ghvqzsoyk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcdrvyrcl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gprtngkjs.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/grvcolfkw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/genlectfs.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gomiqfdtr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gpnpzrfap.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/ghloflppw.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gjuauguht.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqppfdebh.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqtlukpfv.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqlmzygcn.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzbhwafop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gbnxorkrj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gppvbfluc.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gfvoybzjq.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/ggnjdxmhp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gqlftofhl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/guytzyccy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gejwguidb.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/ggvidhbbr.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gvbdgzzmp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gfsbmzkmo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gxjbeoena.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gpvpkrlrs.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/ggwyjgnnt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/giehsonyt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gbyizfmfu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gqmqhijhj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/grtfigtij.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gtrlyftbw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gphecnfoj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/goywmrupc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gyqqyfmfn.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/giviryffp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gepffqibj.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/glwkfyvgw.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gknlipjgl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnlffohyt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gtmjgaakq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gvhqogfov.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gcwqlhenz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gbhtxadux.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcugtggos.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gxqwcjjfm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfkayyddf.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gwcdisfao.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gegxnxayt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gxuzexlat.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ggftgjelb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gifiplwph.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gxjrlhsbi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gsbzpygzd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gypbfcexz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gptjwqdwm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gkdferunh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gdmrukkfo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/giuluzkri.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gjeulzkvf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gyrtkgriw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gsiutsuue.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gqwnbnbfm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gruqwezvn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gvqoyqdky.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gerofoxzu.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gxmvlpzta.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyocrtort.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfukbprfo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gukxgntgt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gwlivzpad.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/guiexyfzr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gllxyjsaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkimaeevi.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gzbmabfhu.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/glgzwixaa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gskwtrkbo.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gsimqwzyb.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/ghyhfwlyr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gfrfohium.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gtoxgcrhx.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gfpopinvu.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gjgvpenvk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghnatkqbb.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gsrpawgof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gjsrvrlzf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gpifhqgrj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gwmotgish.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjpstvqxu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ggyxmofrp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gxgdcippu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gzvvaevli.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gbpuuoodf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/ggywgyyje.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gyymowrst.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gpelajawo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gkavsaqap.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gcyiibsan.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gcwydxwjp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/ggjxmyqsk.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gsdxztzgy.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gnuriaibk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/guequhsry.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gaejpdymf.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ggombpfng.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gltsauuqu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gijdrpeow.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gfngoygyn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gkwmeqvtb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/goadlrdqf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gfylmiydh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gyeeakrdw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/grjfphujh.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gutxsyewg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gygikghvv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/garcoxwrf.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gjeglvvnu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/glzhucsyx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/ggpgmgrfn.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/geggitmdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gsslwiwgv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/glazpztbp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gehvvcbnc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gblexsung.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gotgbyorw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gasfeduzu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gqnwhanqp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/ggigmejqk.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/ghfoctrjc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gjderbrcn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gnbkahyrz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/grehkfqqw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gyoqzkqcm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gchawital.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gflsdssve.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gxtjlkxhp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/glhguzzfa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfcwnojzy.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gxgzcmrpl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcajknckn.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gosgqlzgj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gdzmtetyv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gbnbakdiu.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gucubazhc.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gbyylyzdo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gvpxfzftj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggblkglac.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/glkgunstz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gaasnpllc.sHtML


<!-- 参考信息 -->