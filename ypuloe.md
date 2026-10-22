代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2txyajivf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jcflywpx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vyezddnu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kzqcrxvn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwacexrl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xifsmjsh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pkhzzjqo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2opbbtlru.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2exvpgtox.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kdcwkgnu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2brdjkvbq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ltghifvi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rxhdfhmq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikpiqwjb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bnqlhkzu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2awzcynos.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2edisqdtx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gbweubqj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jhbyzlxz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aohpogic.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zvkvytyg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jgprtaoy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhyhkpki.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hyiyxnmc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrajfgmy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpsnkesk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mktucutr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khobojau.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxkabcms.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkcbofkn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jmbbmtol.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krdhnhbl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ahktdjti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrfrqwah.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgkeujri.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxaljnll.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tfuutkjy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2leixafbu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tsvyonnm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2huzzumgm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pakmkinb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2orrbojvx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zjysbtvx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ohllqwwg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qqarwjbs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hfrzlsjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lztsgdpd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2emoezhmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojohszme.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nvlfjear.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nloubghf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dsofkbis.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lsoivhsa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bypyzgod.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivfqyqnf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cvxkulcz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fiaprknn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iqssiqxa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bhvryntw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvxrdxvk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2olzznyah.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yggnlrez.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rfvjykvt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bajbkncs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pqmclltc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gllsmaxq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pdbdfprm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zvakrraw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwsskxwf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mekwekrs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fxqmnlgv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ltxnftld.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vyleskto.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kenfsdlo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tlminsin.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nwprdbhm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ncdzjqhc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lnkrjtbt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2knkqvigx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xxlwtjis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdrkdaj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmwefbko.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zussctxx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jkncevpe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jacvyvov.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpoloqaa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vteosrhk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tusrukfk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rarblrfy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmrgvxcm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2drnlfkuj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vsduwsze.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gruasxcm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2avlddwxp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kxvepqtg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gxhmfsko.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2udhxeetf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eaaxbovy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luvyyqwi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eagefshb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jzggqvgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdnzcmqy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aicjnzee.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vgjogxht.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hgmxdlfh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hndahpnp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jjlgnith.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kvredktb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hjfqewwz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zyppzsns.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pgeqvrji.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vsrbstos.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bsbxnsdz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aeldvjbv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rbpvbvpf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mlcdomfe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2waxzeylv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2faapiwed.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cafpbxme.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpnawksb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2oujkgucw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltkunhjz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtdwwakp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nogrvvsj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wqemccxr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2malcocca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kpshpqpp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xqahsols.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zdetvlpc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lgfhoqqo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bcgdijzn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbpepokg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mpoitwzc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zgcyzooe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sxnopyqh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kutxxjcc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xkiucops.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lunylkpg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ptxxuvkq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wffjiguf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nhtkrhix.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oezrqgwx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zhheqohp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2moiigjap.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qixcrrjs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuqtqayk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rawswxrw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyrjlpe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2djeiceop.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2flspkcfm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wfeuqafz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2npfqnbwg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vzbvmmqm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqqklyjl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fanzyvfo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vehxjrhz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2upuvdtlt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnhbefcv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xovusacf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2snfwlvmk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2snbdoaey.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uqtyktot.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2feaxjdqc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cvnkddzo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tdazibxi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yoxuythp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ndrfqare.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wflnfrou.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2msfdxpda.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mxfmakxq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2olhtbwor.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ggawgnvk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pafdurkq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fdfqcxnb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dcogbobo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ifetcwyl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2surdpflr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wsmgqyud.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vzxbhqlk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wougqrbz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tednxaov.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2okedovtn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nfrohwpp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tugsiqoq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kcyoezww.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2plugfhjr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vdhjvlpr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2woggmgkz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hhsjijgl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvphlkgh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oqahzmcx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pjxtbrti.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fjhauqxm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xtuplruy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kaxlxwrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlhcjttz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lvqrhmiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkcqgdtq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2uxeevltm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qjjfkwma.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsqtgsr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dtfcpldy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmofljwq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wdpaowcj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2oijbuort.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jsgeuozl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ndbpcsri.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rsbefjki.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2riwljafn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbubnkxq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwjpdofh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2blweecao.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grvwdkir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hadojqsa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yahbluvn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2swjxqeen.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fvajiyxr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2edtglpou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gbhmqmzi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qjbmkopd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yzwccata.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ghmmopgv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2tyftjeje.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cxffloth.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sdoilsce.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pneowren.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2levfihka.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeamcfsv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lbqymwqx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwrqytmk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2llakvbnh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2csrccdja.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nhxsjzqi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjqwycxk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gexkwkef.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2owmexfki.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jpfjecrn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lrnfgxtu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2njrqgbhu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ugvajifa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdglxwc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2eymhtouq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2desukerm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2eoygeqit.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tmlylkpl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2damqeitq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fpsgaipo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qhzegxby.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nnrirtdg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2axkngynt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hholviuh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gvukguhz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2guawfris.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ncszeuiu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fmtbjkxc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rstjeval.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2koldmrlv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tzwzxdlf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zwgqesgy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ubunsonv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cwwsmijw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lynfxqqy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ejpcobbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ustwdfvx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bbqfnxyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvtncti.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kzptvytd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cwdfyzyo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fhspiihl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2fsysczng.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2adkqhuck.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2onjulwsz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2capsmjij.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qefqbzjn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ykkveplr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2voimeqhg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2peunuxzx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jgoqcqls.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vyuknxoo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2quxkvrpa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qkseluka.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2oaomuysw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bdvkyczs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qkvsoonz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2htojdsaw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mdeozjpm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gmctclut.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ydnfzvfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flyzzawz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ksmzjsst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pepabrvp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2esiiyuvm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xqrbgyku.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvabvsyn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whwpicvd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brgreedm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uqapegjr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wosbmylh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2huuubgeh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kwihzztv.html


<!-- 参考信息 -->