代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3driajyid.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kclncppn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ezckboup.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pckshwbp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hdwnkean.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xypwyybl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sugfrfrm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tiojfluj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3daeeqgok.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jnhaxmyl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qcjufwyq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whoreppm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ypbomcpe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3btbwcluw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkvcrhhi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fpyxonkt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkmyipgz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uiochmsv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mcdbelpi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kijqjhnl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqxtvsxs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znnbvbgf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnofkjrk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzglupxb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hnhxpiig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bojjarmg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3swkukdof.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ehafqsvi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qfipcbtx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdopbech.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zlcgjpws.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zovwqasi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ymwjhvif.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3albcwuzl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cqdhyqig.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zwmiorjj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3krloddqk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pnhdgnqj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hcgehirb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yipzmhxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frjjgpeb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3txwfrnrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xujlsvwk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pljfqxhs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uopepwzo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grvdvlkn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3krfshbdl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsiswkrm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvtncahp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qqoikhro.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eatfneam.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fskqwsmg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tmefmwej.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mlffvrvl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grzpkrtw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzwpakdr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3domqtupo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oftkyggd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3crzgqpdf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xjyarsmg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ayrvticx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qehfszmd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xibqqmmz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3learqjuk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rkjtdvbi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pjsapdwj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kywpmcop.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hsnnfrnl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ewmpfbbv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3srxbwknx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kheblwzd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fuzwszvs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gkdkztev.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obalvidp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3abjaynum.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3veblpego.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wntdlptf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3efvthcdn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3onafghfy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ycmivfog.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cpegtycw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nlwwwgyq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uruahwhx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gahbsqyp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbignvyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tavmruaq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dwonkvgx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3duvrwydz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tqoknsoo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3koduysgn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axjivtdn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkflssgi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nynsqmqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fgquqdiz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yoepkiwz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rwiwwygf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3hmtitkyj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jsmeywrp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zizvtkcf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3szojiylv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3udnvmgem.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yrxmluoj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zspprdld.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kktbsojv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yonanagg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jhjyydkb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3trlysuln.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fbczduhd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xizsdwkz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ciojmsrg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkzwybpt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgspyyhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rfsyiyck.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3duksjkgp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hubbnueo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hizgqayn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yffsbhsd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3isweapst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ogvwdpkj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3diptiuek.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3iadiiypz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kcygsbax.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bntnoveb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3slzgexic.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ughfhazt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sjrqdqmb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aobmxbfv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3uvvycrmr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xwabntyn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hmlxsozv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fnoujild.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3phnmjyuu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bokqaglu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nfwiwzrh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zkxyztrk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upzmjtob.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvqbwhu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3reetfods.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmvbpra.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jqctjsnh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ocrhsdpm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pnrgcano.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qfzqmqri.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rjvaknww.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opbkefze.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhezsnqo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlskwztf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zxytjifu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3crljcusw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3csvgjevf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3chjzjrny.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lbmeeamd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpvbgqh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qptfrbir.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tnahvbns.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3civjirem.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yqlktyxu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwxokvgt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ravnspqo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3svfbucvs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yiidqngh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qtsvwkcc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3potvgiml.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3abqwypoa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tutwlmra.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcjltfmv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qdtoeqgr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pucyirrs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gdznexhp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zqoqeqos.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3agwswake.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddjevcry.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3tyrnimjl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sipoicye.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3iwxpytxt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3agbxufna.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3urkdbiug.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3aabadklo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dimuobzj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sipkbqub.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tijgnnhe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qpfuckzg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hxpbwtzz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zklptfwt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vvadoono.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hivkptrg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jhszcoum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmcfakep.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tzlebfez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjkydksg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vyrcpuwx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmuvoyg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3moiudbpd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nchpgics.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vqaswzlp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxmumenz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gvqiaghi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lpytqlep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmeolgfl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nohhmptc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rrredbwz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzzgakbn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ofxnawwd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3woscyxxq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ywymrkpi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3okminfvw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vnvmtada.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3utwokwha.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mafdtahx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ppemqljs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jkycagnb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ivdmqkab.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uehqniav.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lbbwudsm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gcnbdlka.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ifcdstab.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fpwtkdxn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3auddhbbn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qytxazga.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3icfcohpw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rrihikhd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqkvmenk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhiusoje.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pzskyzav.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3moyzwnpr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vtccvuax.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nsyxmaqw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pjoapujx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ftzdabuv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlpdxgkv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzycstte.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ocyktrvn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvfykfg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jnvwpspt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3evnhjmda.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cujbnglu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tyabflhs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mutcznir.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zelnrbcd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dkbfqmmy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wuoniykd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qvdzzydo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ytsgxlqf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vrieovrx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qwxdokio.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wgoxuwwm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tzeytmtj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3noevaycf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ewtfgmca.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rgnkuwtx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jbwuuivd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3heltaopu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zvzomjiy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3yjinvzic.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dpcxilpo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3btbrsvju.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hreredxj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3flntoenr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rzjiekiw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fetdifgd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jgvpghqt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qbvajkun.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fjlclyip.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3bmnbtrgj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3eecfagtm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ubcxrkne.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3gxsndmkt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kayrfzgi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cmvpphtw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vzduciib.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ydrilsxr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3eaupytgh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3wppqgbst.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3tcmkemgx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3licfigcu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gikriiwb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ajjuuhan.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mrofjtbw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xkamavvs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hpszzvfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezfumqfu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yiicgcge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkenijex.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3uyusolwf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3babsqugc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3opnjtbbi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxdegvk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dbizabjl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ckmsvlaa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eduxuthq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3prbqaabc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xvrqczom.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3llmdkviq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpppsvwo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vtwkzznm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dmaetgav.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cykxdoza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gvzfzwnu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3stnlggqd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3keqcwvhu.html


<!-- 参考信息 -->