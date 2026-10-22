代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qrspalvg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2uxatmpnu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hnkmgtwr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fmnfgqhb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vhimineu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dutrcwjr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfbtzsu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wzryhjuh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ndrnwebs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2riihfaqp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2saepzemb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wfsxplgn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hejvnzih.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfwckph.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hplheiue.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wgnutuzq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2abdpmwli.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ijhktqyp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ryxjiwcd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pacnzodf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lmwkymsf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hdokmezp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrulepge.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mzdgwdgj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iydrushj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnvnlvvz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qkwhokeh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeygnbio.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsjmobzs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muysxdao.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sgjvshpq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2usjccfox.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pnjrbldi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsvcjyun.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhgkldso.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjuyvig.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wjlfofrg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmsjobub.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2whatpjxv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xsowsbus.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvevbel.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hzhniwsv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bpgmlqvf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mfnkzypz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ecwcqrpb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wfxwbisq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vmjecpxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lebyprkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuncfjiq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xwvpgxgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmedlkch.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zwrzyhdd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dgirhlee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yradsaxe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2delkzgvm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xowasgeb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwfzwwxz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2etiyuzzc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jpfldlaz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2msylgtbf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqbouhmg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cswhqlsn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmufynim.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cgxvrysq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bvtsqrtu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tgevqmqs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2daqtflko.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jceypkcc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgbgidsa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2iaoqgill.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gkznhlnu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qnkseepv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pirykszc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2znvfkiil.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gnywsksk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dfwmehkr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ldbugmcw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yqvetavz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eoyprvhk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ibtfeice.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ozhvpkly.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtkdjos.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fmdesvpt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wtmnlxjt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hpsntmlk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jexobwae.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qbnzgszm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cnoqqtbc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gxpeyutg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bytljnfj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjjplzgy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjgiehvr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhsijaxx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2odqvjsvo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ngtwvapw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwmhthuw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cdtwytls.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lzdebjtt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nonrdvhj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmfqfvlm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2azzqspvf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbtwaigw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2stutvwqb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zrbjzkom.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zvxyjksa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xzhqjxzx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rsppboob.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2apyjujor.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2etxsagie.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iuzahmug.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dggitben.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2owaifcea.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zexhrxcp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ewhnjnyg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2oeokalwe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rczdaoib.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bizfjogz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2idlilgzt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtfjueqb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qlwdqabv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jcxznobw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xlolzicr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xypxtbvi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lkklqrib.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ymzykbzy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iydlxxqp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qxyifgfz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sivnackd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ojmuysfz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvutqdf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2auhxbmif.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwgksjp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2buzradit.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uwfzankb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cmdfcuqc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jmndnngm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vhnjceby.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2crtkmfiv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dpdudolh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zwutexlq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vnxhnxji.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uevsspay.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wxikykil.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmtggsk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcuzwbsb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zimtmmds.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ruqjnkhw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhuwyld.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2axtdwsuj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pgqntfyl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2udfuhcmi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2awqrtwth.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fixfatwx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqcnndbu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlygomje.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtgibmzl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2blesbpud.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hihewqzg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2opvermmn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pypaffmu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lmswcind.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jxcdwpzz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rlxrhrju.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wztpnzuu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fcooprmw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zuhuredp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hddcxacy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ddykktuv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hjydczzg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2inynshxq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wodlmbqh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uykvlfrd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mdvrzqhr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2inpzxflv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qefcfziz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xmlbdvty.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cgdvmryc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gqhxbrgd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2eiqjpnee.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kvwitnpr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xphrmvpo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2axoolvas.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwdycgu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mfsfzbuc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rqkyyezf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbnzxgr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bqetjfnb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nkmizynh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wlhncbgx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vtqwczsw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zymmnkfq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lzkiqkuw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ynfkaxhc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2khfbsdem.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hzyewghs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsevmnvb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2orfbfuqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdphcyup.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mxpsrlvs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gipqssss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mburmdef.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2huuownor.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dkmangrr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vxarasfk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fgfclcnk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmrjawjp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yopyxlwj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vfpptkmx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jrxdgsuz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2denuzgei.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2joeqcwub.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhbxpce.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2elihfqhp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2evdjlggg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2woaltqhl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrrasphm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pqilmcgr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2gcngilet.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qwzoooqa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nbyzlrby.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ghqcjcep.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ayojjfby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2clawvvwk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wpujyhbn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nxdaquqp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebkacwdi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tzuccqgx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cucfrqhv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tqeztqui.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nzbagote.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sasjcsoo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eogpbirs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rgqewyro.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2eskdiihc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eoyaayol.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hybguret.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wvnbhtto.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxxjehpa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znukrlgj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2elxyckju.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fhdokxmk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2eupswjez.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2sonespts.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2egdrtucs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bxrjpkue.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vvcplvrg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mpkvsnxm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2plfvillj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2caxrfeqb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jwoyfzat.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lmzjqiag.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jakmzhqb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2helewadv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ebbbnicd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zckzhkif.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dyzmltnh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2demmvgun.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ktthxdbz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hqrwvorm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gooqamfk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pfvvrbmj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2dicybzht.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hfqsqktu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ipuphami.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vzzqqmsn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nrgeahpc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mbwvchcn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ykkajacc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2spmpglmm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xntvwpxz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pxhyeqfo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vtdzuzjb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jmuyixyj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2egibbwlj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwbovdsh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdieserg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vvblzecy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vmktrfum.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ckhpmfvd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xkiuxeml.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dersvoxt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2duolpugi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ipelityl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xcargeqe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2csljqogd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mgwtqgsu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yocvmyst.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2larmnryn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlfwtnqf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ntvmcpgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jazkaymb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ttspywmb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xpvsujbh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eandigaj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2booowldj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijeemoxy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bbbwdwsc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dutfbogq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfdkprk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eiczavzf.html


<!-- 参考信息 -->