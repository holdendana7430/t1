代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxrzetpb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcpyasdr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kkkeoizx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rteriovm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hhqrejoe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wjosbjbw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qpzgtsfc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhymobod.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgsatfj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iliaasfc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mvvotman.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vvuhgviw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lutvptny.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pivdnwty.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ftqhlqkf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qsmuvvqp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yfbdfslp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gusyrvkk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sjwjtadj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kgqmytjf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jsdbaaod.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssfknfpe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zzvmziii.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hwtphtsk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2prkqmbon.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xpnvprxu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eoltfixy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwxusmft.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xjxuzbhf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kdoxujkq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqwjefka.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxvvykso.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdogmlkj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enxceuyr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gwniqdpg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhokzdrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lysihunn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ooihvetx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrubutyq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hiiwzavf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfcehxja.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixxiqymy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2enjygvhi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pzghjrmk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jvfalvaf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hckdqesz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2suthhqzx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kjapnzrn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qqfqlaun.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2eszhmshj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2twjtajzq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jdbisrfu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yetjsjxi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fmmmwaei.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gxdemcwb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2djzymydn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbzeitfn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nskwyhqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgrrauyy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gjildzwn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lszrbmbu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cmobuscq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fjvnczwn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mvvhbvkr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaazybrq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rptapplx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wfrjoohn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbuvibom.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnknbqtp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ylmznfzm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2amyyisdu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vckuysjx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmaizpjq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwxtythh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gcgpxsrb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aethyqeb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fnrlcglh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bwxwywrh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ebuqxetl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nlfpitmv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wglgjwox.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2arfwuzmf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tylenceq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hjpcaikz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nfdiqupu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ukcxraex.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jbrrgvyu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lymjmafu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovdgzsjy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uydqjuhi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqiqncc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtoxemwj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zhadjgpo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mlbdbkhu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vpapfpdu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yvvhgcne.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ffrnnhdm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcxgzbbc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiacndwl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzbbwsex.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kxcvfgba.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uuigsxfp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hsdetvye.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvrjhhny.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tdicigut.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qiaynzap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owqtlkpe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vfkmvgvw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2famtgexe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnhnbfv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zgyatnfr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ezzcuthh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dtuhidbf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fxsqxdfe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zcxosoqo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mkbgdzlu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ytplblai.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wvjlohjg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2euaditpd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zomwelng.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zstsioqn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hbfqambk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xgvlghnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fdkndwja.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wuvmuycj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dfpqggcd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uyhjjmqi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wrikgxbe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2omoxeimd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2exghyvky.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2urkkztqi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hocmsiyi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ypnrqhnh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2btzykvhu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hyzpzuct.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rgctkaca.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgptggrr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2uysbyzqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wezdurce.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2omatpvph.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rvzradfy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zssiowjh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gksoxsrs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rltgnqsn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sazmuscn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jolrbpbd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rkpsncyy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2duduxwvg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jnjcjjzr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2azbjfugd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kpqclkuz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjvzhgoa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gwitsegh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dukvmcfx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iqxxzgeg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cgaligxl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lddaidcu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kpkwbcnx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vukbtgqn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gdxtmyxc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhaklboh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nmektrej.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemwpypl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2csfhnpwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kffcztmn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2shijvfqw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aymwlfvk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gncjhkvz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pbnuhaky.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2heeyokpq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rrahrheq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hhesykit.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yjtjpnnb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zchemsbu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2thwqeudz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hmjwunez.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2olaaucjp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ykdgceyd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qmkkbhwr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qhiutvzg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bbganvrt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnixrrwl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nbofutud.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vuwhseoh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xwpmlpdf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dmvdsvrj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2moqrpols.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvzwqoi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yoaftkhd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmsxcjjf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2octwtgxi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hozsotco.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uwyrdpze.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2glmmkcvb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2emstaqja.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mcedegcg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2webxtchg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2livktwxj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dkwocuoe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qjnmxyzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dyapavma.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zzhsihcs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xrpzmidz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftvounqk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xfgmisvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbcenyfs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tmyifqgy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2juqexexw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2thprpmsp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iwztwqhc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2leipxrzj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzoghuh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2msgzmypx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2abwpnhrq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrrotbu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mqgrvvqe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yqtfiecs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bekocblt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcmvpjo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kmrienvd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nvawerrj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2wlsroqud.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2czxmuaik.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ezuhnbge.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vwpcojws.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tolyucdo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bwfqbxtj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2quotfjqb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kbrhdjdp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2syfzfouf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zzfduqnr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vgheqiar.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2clmftqrj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pmsgakah.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jiyhmzgg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mitshcyu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hysnvidu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaiohrie.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzioswbl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ynzfshyt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2krrkktwv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftkjokxr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukxvrkzi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rtzzngfd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibsxurjy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iitfvtzw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbucbrfg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csykptcp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2diagzcjj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nuzblbnr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qhsurkpa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2hrfucmcg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cnlkcwcd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rltssicf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cupnosql.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pkqgwfxn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2opgjtxch.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2emaozdrp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ovkuxfjk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qfmraiyh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vnljmsne.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2bdqdukiw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xfqjdkma.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xzmshcau.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pdqrveaf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2azjgvjbq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ohnjtjvg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ixkyseri.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvihlcwe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2uhcegzin.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rrlxeooz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wqvisptj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2duuysatn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2odublzbu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xqdhjpuh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2pwfskpzp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bmcciuol.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sljjvkwy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2elsujqvs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gtzmsaqk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fswsqbhr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2elyxgmom.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2iufxvjwl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2usrpmbgk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rwdkteqp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uytmhtnd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ojmicfne.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2itfubaxa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2hthskqdp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uwqlhikl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sqerrtzt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ucvixnto.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2waqtzbqp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ebodvpgb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2teffcbeo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xkzeflrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujymmzcu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bljtmywe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwulgsvq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zvjbcizk.html


<!-- 参考信息 -->