代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2eqzruwec.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lbfgzsyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jojkmyod.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pnhrqxnv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zsaqzqxm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2euybowvn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gybveabh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lhlfftzh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nfxwmvrv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mbmuwcfp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2khaqepxt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jxiegpqj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wdredrys.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zpemapmx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eavwgyhf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jjxoahdc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jtuyilrc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ucfzgxze.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nfmwqdfa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnsudjfc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pingjazs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kvdhsdbc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yeittufe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ordfqvpe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dejehwlp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owsuyxhx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2boigduhe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdhtqzqe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugwftpfn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihedwmms.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ycbaazgm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkokqoge.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kfnbirfg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oopqcqsu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwgkgkug.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wfosztkf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hqebzgdo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvyxpiop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lohrwkbq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ywhehith.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkyidsi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2txwpmqvv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cxegyrhx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2chszbvdd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tbtvpwes.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eoueemat.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mnfsydos.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gitdztxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2leutsisw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2scmknsns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brvusbgp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ujjxqtyq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2znaxdlvf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2eyzjupjt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjrxwzbq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2spzcvegw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2opmrpofp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2adyhigiy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdfnngxb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnpckkob.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2niqpsfye.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xzgksgef.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyitvmtk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nbgjtdig.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbmosisk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyobaymf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sbnkpthf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2drugwnyk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gqsucqpr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ejlnslgj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jqwunhxx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gfubkrrk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bvdajnqz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rvxdyugv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2azjjfvzf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tmuhxaku.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qfgfeqqe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jpeslzze.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ucnefibj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ohyzssip.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvyekks.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsgpsuzm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2usazpoln.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cpbcjgcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cnbwghty.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fvlvwxlh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iloyupfl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2iqhgpmvb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2awahexcb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjpwyfrq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkumjvax.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yqxhimry.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2adxkagzc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2cdmahsib.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2boqdpznq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2roebhdcr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cpvtymff.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kzrtpkfp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bjmptakp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2izqcygav.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zdaqmiks.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2naytsxee.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qgquhcca.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggbpuzsw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2awdgatke.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lnjzxyns.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gnuzpjkb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2enynbypg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yduoawfm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2npliyqig.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oejwbfwh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkczdkwq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2aneopxte.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2onrjqrhm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2drvonaxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cznuyfvv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoyqcytk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmqofptt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynubumox.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2abtzdedo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bgprzcuw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgquhvsi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nrazebxc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pxmnqfij.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pjfzscoj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2srvqexnd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ztcixgkx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubmntifg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2aihjvxsi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lcsnbheq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wqrejabg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtuqsjau.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dxsqwiln.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qteeqgbm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jggxywxu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tcmppumr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kizchyww.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uofwsckb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2eeqkhejn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uqgqlzjo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gslurvuk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2njjgfssb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nvlyseiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqkqugy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rxhwqjal.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2liizwfaf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvvvzgeo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxyhmjt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2atlbuage.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ucofitmo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oermcsoh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rwjvwuip.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcjbgchs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrdlpkyc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nswsfsgz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2enufhuck.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2blpsxkbq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xksnkacu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eqvbzmuz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bbthipnw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2edycjlfh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aqknhyho.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zxeuvwre.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mwjdqbvs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2svdghxsm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2onseslgk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbcxveq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pjgjvsma.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jtgswejl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qpiflgeh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2positiir.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kbdqnvbj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dpxbnjjl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlkyyxnz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uwerljnd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2haxgccvt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2itramluu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2suvliylq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cuhgynal.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ftldvoht.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mwefwkzz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kmcjbqcg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sixsyfps.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2djjrqtdz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2edmnolru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pnjqcqnj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2eliyxpxm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2keoweknk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rqxsvnkl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqwktxom.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhmgcdwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mctoxfwu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ojxedkng.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xxosdhta.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zypzbnrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohrzkcyd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2odopnnze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jigglczx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gifkhold.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mkoausyo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrpdgnwq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2htcdbchu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwjyxequ.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2deymbdjr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oayjnkob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyptfvbx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrjenngg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vodgybrn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wlwxcqrp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsiwioci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cvopbgti.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrugxqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2icgldlvi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2thtrvsbn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vapnkdmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fondyrgc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2llbptaqs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ztmcnjhm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vmmlvoix.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dvqgathc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jbietrnv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tgbdxxix.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rzirowok.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rfhehpte.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2monrdhtx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kbwrulfr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2phtwegxa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ixdaeorx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uncuokvm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bpulndyn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ivlawonn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lohzcnpj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vssnpktg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2umvyjitt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2aivaxjxe.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zrwnfqfg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2grrbtovy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukffizdq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtwlzzeg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ixktwxcl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2euivxaga.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2abunryyx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bdkkkcdl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2oacxndtx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xnozpxek.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nvmvouie.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xelyrsxr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2heewvvfa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kuuqclxc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jekvrwku.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fctbzonf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qvpuywnk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kpfmoghf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fsbfampu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2abzhmmyd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pggiuuwa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jfiknvlw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hauripew.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dhvlagqs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2amprjmra.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ueuiufjc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bwzucwcg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2byxqwxro.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zyclvncg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rvplkwtf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kmeowfqf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jgspdvit.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2plvgnoyv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qglgcbji.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2durfejob.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vgdcrfxm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2counoqpt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2djgykvyc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jiarsmxs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ovrryowr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghjcoyik.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rrmbngzh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bndmxwok.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pdwwdvlu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2totkmnvs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nrboqwat.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ylfpxayc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2oagrrhzm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vqowtfiz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pvcqpglb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2iyunsxdl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zgfosahl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gpvvxdlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxynvitk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ztgvqwda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exxvtlsu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uecwlihe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mptagbgv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2scelqnwp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzmukxff.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvswnedh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2okpvtrqo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlgnxwb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zzpugvyc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jkjdqzme.html


<!-- 参考信息 -->