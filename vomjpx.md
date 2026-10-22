代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2inqzbaln.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hwhnbxqt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xhcpgbfe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kiwxvmac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2izsqhvgz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wtsbiwxf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gmhcmglw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hrtzhxpo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lsqfhyxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vyizquvk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdwfaom.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pbqryluw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kzbdrtif.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqezmsyn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lszkmxvt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2aqzllkpo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ywakwcri.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sogziczl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2szhgphvg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ullfsozg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xlisvusw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2blltjdqs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkjnauok.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rbsjghhj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2koupxsew.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emruzsku.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oxyiixpd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkuecssq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbiitqmu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgimtupi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgtascob.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akopleki.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qcodkgsr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujkuiuvf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzrsqjtd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2byuxljud.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ewwnuliv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzvdwzxs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ogenshgy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hftsuoox.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ycwkgljt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jrpzuhae.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tyinkpvz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ecsufaov.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2igiofzog.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lpqohmqi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qhgydcil.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hifsswzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hevvvbxg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pybwzwxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giaalbye.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gtielcwi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uktxdnei.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2easerpgk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dtnepeda.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bieloise.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2beyhijoz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2bmgqived.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jfjjkzms.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pojqlszf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qashcnrs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hqzodtzu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krmuphmh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnoqluik.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mftwbdky.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arrkhaqj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2fzfhmyku.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ouonhvkv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcajibxl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uweczdan.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tdciydrd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2romwkfdt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rvvorqld.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2clunzgsc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2shxqldjr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mibdhdtx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yqrdpqxs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oabmojav.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2knlcdnhs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2owvwlqqo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dewkxpud.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odtmpmve.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2raatdqxo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpsfqnot.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nveeiagv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nvvnqxsa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jsgjqdnc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gghtyxma.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2haolfsqf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tblqqmnv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uvmhvkph.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vscmpmdw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2srhxbluh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jgihtdwm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eexzxycy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmqiisoj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2modldonm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ercouzba.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2koizioyv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zqthvoqq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aceiycpy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocjfpimj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2titevuhp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dvtttizx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mymfakzn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wfsnmiyy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xkqenisv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qzrolsds.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uewiojdg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bdhdcbbr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ineczhwm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vsvstevu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bnwohmjw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yfvkcdbn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bqhqqqme.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ikubufkt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2yeoehnjj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2djaedvbg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kdqebpmg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmulrecm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2koftsbes.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bnugkbpe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vdbaimna.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qfratbrx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bdotqoxc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zczbozob.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yozevabb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tidkhhdx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbbzecj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dywkvhnt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zrgvubcm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etdyuknw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ycokusjp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iedvxzme.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gwdfqjco.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qzejpapg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sfyrkyqk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qzyzvbxo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dqwgclwl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uchbmait.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uyqpdqhq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wgylpeiu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ufsrawpv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nvhhdgom.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adyafizn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rfzxeufu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbiwcxdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wbczginb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vkyeksjf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mybsvpmh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fequdepd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2otrsrfsm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xysvtbdr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqinottv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dfejpfqz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsxkvhqh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jluiqjgk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2siyvfvbh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ofbywamo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2klhdsdqi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dakfczvh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aadwayyg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pmuvlkvj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tspgkogq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zbquylnc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ttorlsmq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qroszuol.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xojuiqnp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2chqjczha.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bpwmgeop.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wrjklkhe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2crgenypf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fpiyfjte.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twqyqawm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xfwyutlp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ojnzytib.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2alwgxcuu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dzrownrp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cyhqwwvh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wusmbger.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sxgfhhjc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kcqhduxy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2saaggqze.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqznsvd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2udkxjlcv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rkheistk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2eqrtcotu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mfsxdkcz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rcyjxhcx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dukujgzg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wjkepyje.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gpcjbaby.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rqvjmuor.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gnzlgucj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dxsbizat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omjolzdn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pmdeonby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brpxrcsu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bmaprxwb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cqmqpuff.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2usnlpalo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2olpunaen.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rnywqsty.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2slwovoof.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cevtdzlr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsnvcpiw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnopxryd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gfesutbt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ctpwgcwd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ylueixez.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uweuvfbz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iehmetkm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuepjovx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2wippdjll.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tnzejoni.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvoijevr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2psyklmae.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2eobqtvpn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pxlwbnkv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kfehoxok.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jtgzbwfr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ltyumoyn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zhphrhae.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yiyhlhbf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ihyqwoas.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2skvdiiua.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nwxskqjn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iagywvbk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eevmozys.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcbokxqm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxkhhkwk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nnphwtws.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndmmdbtj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mqmfxcez.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hieukhxl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tuehuwjq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gazbmvpd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgarvvot.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bftqrryl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmxknvjj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qpcdwfqr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rvuuesxm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rskcqzob.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tbsggzbp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dwensgyt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2innkapog.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nqubgvon.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hbkqngqi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gjytuxqq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vhapepdl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xynwrnrm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2djdvruox.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2dcmbtswi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2inkifbuw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jwklurff.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkodiiig.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zblxdzrv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ptimgoyx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ecnnspfk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2clomzcuk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dqvzzdru.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2naeomyig.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2iuveiiip.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gbftntpp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ugbnapyo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2mekwaoje.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jcmzrneh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mnvqbsyu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wwtyrqbv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2evjqnamu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vtiejnls.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vycihwlk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2uygthisn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kncjajzz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ihrwmqev.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2uviiobuy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uspgmfjn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fjpmqhlj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ueszxyng.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yebbgsgj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmrslzv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rkzffumw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vnbeapvi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2awotfqqz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fczbcchz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ocvspwrb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2wirniluq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rmqtyppx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crfvikma.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zrngcibn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sesdchsa.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vquwkzmx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2sisuqsqx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fmrmbrwv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrdgsxr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qmrntmms.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qrzlohyk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2nkitzcnk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2buzbgawu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aljrvwzd.html


<!-- 参考信息 -->