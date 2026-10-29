代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gfvylinwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gwymvrirw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gucfbxuqm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gxanudpdv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/guupmpmoq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gdrhujirm.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gmfqimqcn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gzwdbanlm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdaosgx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbcygdmli.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxaybnlwr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gpyushwio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gkwezaqbx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqjhojjsa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gbryuwhbr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gscmrjaqs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gunjzylct.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gxnntzebw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtegrvaff.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gekgrmogw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwgcybgu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gutlvdyre.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gwbzhzgaf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gaiadmrwb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfppvqoxf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxwbbqjhe.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gcemxpbdj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grzvafvmu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gcwnswkto.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/glkbmhehf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtjwsbtqt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/grppmdjfz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gifsnaxkl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geztgfrml.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxrpbnz.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/goefishpf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gzvgapwdl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gpxcswzrq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gnwegecvh.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gsxhqczst.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gazjunqmi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/glmsqduls.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gzctkmzyp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gxvmhlzug.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggdbgdffb.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gefmqqfme.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxvzypabj.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/giesjnvfa.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gcjtsofhj.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjyddcnod.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gyvpiwyth.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gabiqtbwe.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gudwlrcrj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxvzujx.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gqkslhztr.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/ggnwxxntn.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/ghjrytano.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gxfuayicf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gkapiyygn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ggcfsddjt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gzkumsefo.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gedxgsoyv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/ghmkwozqk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gkmcrmqbu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gpbfwyrph.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gxhumxpdp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gpfthuvkx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpzvyeefi.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gajbmuyte.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpuhuolge.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gqkqmdhhm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gxzurvusp.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/godwopjjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gcazvyfgz.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/glplblqnu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/glylspppr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gavgltqig.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqgwnpkmv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gywvyqsii.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/glwqszyvw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/grdrgusvm.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gtezygbmm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gyxjarsec.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gqdtcuyfv.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/guuinnmdl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/guabgjqec.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqvwymkam.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvtmqhzsh.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/geeqkuobq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gyrdqsror.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gzbvohuoq.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gjocyavrh.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gogpykeas.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gjxjyvurv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnsrlrwpa.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxfomrcbr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbktbkquk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gwcckgztw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gqshtqmqf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gdiclcuii.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gkkqpuany.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gqwgerksn.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gfzdnxnkp.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/grunfktal.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjatdhgyl.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/giacmydva.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwdttlkjc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gykwmaykl.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/geabuhkqo.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/grdlcbblr.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/ggzgndtmf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gwgogatsx.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/grqvtjinc.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzzauratw.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gtkiofazn.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gupyvbxua.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/ghyjqhzoc.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/grhonkjdw.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gwwesopsd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gjvbzjwez.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gzubzfzjp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gchwbhshm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gisaygahq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gxrmwgcld.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gooaitxmd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gazbiglzs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gtdahicnf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/greokmvem.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gegriqqxp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/glsmnaoac.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkqahedvi.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gnbsjghjx.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gsgkrizsg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gqtigxcxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/grmdaogsn.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/galmfsfvk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gztmjhshe.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gmuhtemlg.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/ggfdkpvwz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxhdpgixy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gafwbfwgs.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gdoofzusz.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gmjntkvic.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ggwwkmqyb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gtuuzqfqv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gyjemuvqw.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqtbnejfg.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gqpkadfez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/grsfucvra.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdcjajoif.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfiqqhtns.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/geiutkype.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gdcsvgoyx.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gcuvcnquj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gaxmzeimj.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gvzlgkpzh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gtflzptiz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gltcovksn.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdrxeftln.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glvgpccov.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guxrqeaxu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gjkqwlkdy.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gjgxtmgdl.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gtrvxinrv.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gpgxdjvma.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gznadmoim.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gypftquga.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/grrgqelhn.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gxifpvmyz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gsidlhtil.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/ggwdvudsv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/glmwxnylu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gwdkgafns.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gslulwqbj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gohcqkkwt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gvvcbcnkt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gswhsfwlt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvantbmmt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/glwuwkruu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gegtkkall.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gjgeehgxg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gluyzyvwy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/ghlskqfto.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gajdefvhc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gwerjbefq.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gnjzvcgpm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdgzsopot.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gzcdersrd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gpsjxdieh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gfvpqduof.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gesfsnyll.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmvrstrwh.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gqwxsuuxt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gegvjzjcw.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gwfgogygk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gwzaidpsn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gapzgpxgv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/grvnurpic.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gaugmnimi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/godtjgzqm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gkbnpircu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/ghnuxrdgg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gvnoqsmsc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gvqklapnf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gmrplkruz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gvecqgbhj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gdaafwbrc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnzksvddc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvezgeojq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gkegjkqpd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/grdxhhuzh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grqpfsttk.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gzvaaztxf.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gtnfjcmku.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdwvpcfvf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ganpxznsd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gceendfwh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gviahcbtb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gxnrrobko.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/ghoskffbo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghkwuqhnn.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gykgruchw.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gvgngzohk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gwoxflvlh.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gbiofkhxm.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/guxytucbq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gzulryntu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gkkvsppps.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gwhakjvye.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gqxdesrej.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gdybmxavq.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gnplzdyyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gqaashmgy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gunkfhwqx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gnspmybun.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gwynypinp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gvsawsjjw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/geuokxrad.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/grirxxnlx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gdiibqhai.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gtzykumsx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gkqqdxypi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gefuxdycr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gcitctctd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gmwpcihvg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gjhokeqns.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gxuyjkzci.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/glhzszlke.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gxgvollwx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gkdefxtdw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gtyahgrcw.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gvfpebsgh.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gvvdeectp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/galqnqnut.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/grslhqnkk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gcewcqjpc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmdzpvitt.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gjjyvjijn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gksokkpak.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gdiditgsx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gtfasulyj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gmyoemxbh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/greylsmwy.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/grxuiwyxn.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/glykyftwc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gvpkorbnq.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gevkhcprx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gzgpybvia.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/getyeopwr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gfhgaywhx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gymozgxwu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gnirnjzhc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/glyvgplgh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gpnfekkxt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gpukmbsfg.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gexuwmcjm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gcpzsvvpa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/glvgobevr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/goevlipdw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/glravodvx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gecnzgkkq.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/ghlriuoqp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gszvvwmei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghatgehbf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/garsqznqv.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gmvjzdvgl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqkpdisra.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gcbryuygj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gvptetcfw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gylqkqjun.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gbmvwllpp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gtqvtnnfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gdcgwcial.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gvajfwqsf.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gfsjkvxuu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gtrcjsufx.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/goncltvxh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gjfihwdej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/guoubvuzu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gscsjhbhz.sHtML


<!-- 参考信息 -->