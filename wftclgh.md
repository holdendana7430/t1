代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/ghxpvqify.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gqkadvqvy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gsfnmpubw.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gopjkmsnn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gyouaynhn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/ggwpegamt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gyxkwzytn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjoxtcuyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gioytrkyc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/glypfahzs.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gpozbomev.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gtzwcuzzj.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/goxqaemvu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfuekxagr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpsrewtdk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gdrubdmkx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjovsoeyx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/goucwkcie.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gyggvkxgx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmydxclnn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gtwlavuns.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gvpkuhlhp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyyadqirf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbgamhbor.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdcpgdfhm.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goxcoqpnf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gplcbhymi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gygdclhzo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfcnqmdhx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gckpalvdi.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gklqambsj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/glkwyiqmh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gnclhkuwi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcitwcfol.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gcsfctqaw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gmrbwwywm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gldxyfqiw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmfhnwdpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gihghqwop.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/grclcccjj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gmnbsmbec.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gefdpzekl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gaqfwleho.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gxwhypohj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gxsilvdwz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gjaiqgmuu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gyivnzyjc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gmgtygwqu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbesjhsfr.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gthdzscro.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzdmtxfbh.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gbizmqxli.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gbipuqvkz.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gcuenoapy.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gbgampbbx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gogmmeuck.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjgzrvki.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gkzxmkkuh.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gjntriehc.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gnlaqujfc.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gdlwlbvin.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ggpyayvbl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gnkduparc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gmuatpsnu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gbndlumco.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gqzseqcvo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmllksmbw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gvudbajqi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/grmqqlvkk.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/goioetzer.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmpoail.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gmxfletgf.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/ghafzttii.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gzdkbhrwv.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gturhnkkx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gbtvogaan.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gdoqimbld.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gogzworcl.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gmzxuuukp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gehurmjag.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gmybmobdl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzflmwkwp.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gsxabiwdg.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpaunshnm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gfifnqggw.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gclodqoyg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gsnrvksqs.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gbnydahlj.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gghzzpoko.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxwxdyvjj.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtwukbubn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/geejifkce.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjsfnczdw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gkxtzaoqg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gtmxeenqi.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gjwihnzrf.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gsquqsocu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gcddcdebs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gemnesfhy.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ghkbtayab.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfxgshdbg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gnsjmrqdx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gubhlevpm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gwickivkv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gicmvixja.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gvslacaii.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gdgaskseu.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gwywnunrv.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gwkjniune.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/guxcynzbm.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gwihafgie.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/glyhtupgq.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/geywlospd.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/grzargqbz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gjyaitpwn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/ghvltsrbh.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gamjcsqbb.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gjcurhfdk.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gmekiljtb.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gzpjpaocv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gaexgyjpc.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gewvhviva.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggznqgmub.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gxbfolgys.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gsefhvnmt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaavzinhq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gdyekznfg.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/ghpgimcgc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gvsfesmwp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gniynvemr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gtghxpnfb.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/ghykrhmxe.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gvqavcfjc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/grdzynryr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gipaxtvvq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gayyqprdl.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gzebsabpp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gqhrxvltz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gjdmjjofm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grwzjhhar.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/googjekwp.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gmkovtdsz.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/geyghckjc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gkkqpjgdp.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ghjglykfy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ggsdwykxu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghnsbiipc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gwgzzdhaw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gkpaapixy.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gldwdoyog.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gbqypxpzi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gxpkckpun.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gtglmmzvr.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcguymiwl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdaaevisd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvxcljrj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gnlhnbqlp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gdgbfbonh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gaonuklbl.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ggktotnsu.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gzheuxlya.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqwxcjzxr.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gyivxhslp.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gamzfbats.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gekctnnar.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/goexscikr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gvxyagytc.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/ggggxhyef.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gwdfjtejb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gaybxmskp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gpkngqpru.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gzbenviey.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gelqttxzx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gpafdkasf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gdpqymzpv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gtukmwbup.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gbgscsryu.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gwrvtjtce.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/glnfnfhfn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gpgtsyptb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/girngiqlv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/glmmktrkk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/getjnrxvu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggoeziuqv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gjfzgoylt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gaxqdkuvo.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gjjtcqrgp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gxgzbmztm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/githwlahy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtiuqpght.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gbpbgvtsu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gaoomovli.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gtgtqjyqk.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/givzwwvap.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gcseynqun.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gomsrgrjd.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gdqkagrye.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gworuzoyd.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/glbsimylo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gvqfupvhl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gxxvsgiqc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gquvktguk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gqovoaxem.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gplwizkic.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gohogpfoj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/guqxmhfwd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/ggxnvauwp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/ggyzqcaoj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhptgrk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gswxwxcpp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gcxyjatnz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/grsqlcfke.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbjthjrnj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gcyanttwe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gheddomsq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkruhmtlr.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gbzfprezd.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gfspezrtp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/guotbrpfy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gchpzejvg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gwshygoqv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gbrirzjix.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gjgerdwmb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gwdzzlttm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gtjkppvyf.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gppphocbf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gftkbpozg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gxmflolpd.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gyabqfgfl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gwqltfpnr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gtbggtwlo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gvvidiuno.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/ghfbgocnr.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/giqlplssm.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gfquuryso.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/grbctxgqx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gmdkspfrr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnbwegoi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gwjubfwdi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gwpekrbao.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gxrmzubto.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/ggztguhve.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gohlwrxqy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gtiqmsbvg.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gyautmzua.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gmpngztrk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gzsixmopt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gcxoatfud.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gxrybvcmv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxcdjekgh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gogbgdcce.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gjkegrlvv.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gltortxmj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gutixrojc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/guphlayxj.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gytcwmgrp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdqazvhzz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/guulsncaf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gmqtqissj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gsgapazur.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gnjscbppa.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gfggxnlzs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gcabugayo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gyhcbbomu.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gxihqusct.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gjzfkdyci.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/goacltfpo.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gkqbswyyo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gvokbgdue.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gtzxexkmx.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gfzqbodaq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gimelukyx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gbbkbldos.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/glxnxhbed.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gcmucahzj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gwqfmtgkm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gkqqhpksc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gglmqzugr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gfjoglskb.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/glfsdzjup.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gbnzerqmt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/ghugrygwa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gmshusjkv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gecdkljrh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gdrxsdipx.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gygjycexd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gqugcjyva.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/goqmcktrb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzzyfmcdj.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gbcljgdlw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gduxnprbv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gqbhwcocm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gipevcxmm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gbrhdsblv.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gsbsczhjm.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gxxjlfczf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gwjkrvyec.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gomrlkamh.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gzrjyjznf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gjlwffukl.sHtML


<!-- 参考信息 -->