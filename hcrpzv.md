代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2empofltg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjxbkyax.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rbaaystb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzzheeuj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iogpzuyp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqkpwhqb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wbtbedhq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2okyxeekn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ccnhyvsp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2blzfovjw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bsetwynp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2icklztvl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lziwztnz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbfmayz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xstvznbh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zfzkaeoe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iefxhyue.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xxzkigep.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hzlfnfte.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fmnslufm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2irhjzgxh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dyplbvgi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sxzqyqku.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ydfuroii.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gzshkniq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpoiifne.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpwckqun.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mnvmidnn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ymxtaolg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hiqixced.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jxqxtknl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjvlrtxq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2voersdco.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2aadcddou.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djsaevcy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmanrlmq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fopprjnu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvyzvsvy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ebgvvohi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrhgrfij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncvbaaxe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlhfroki.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ezwimpon.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vuvhhxcm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qbodowrv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjlwhqwu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlyznclf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gmilfvzz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2oqcsehmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqgwrgdz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oxrwegsd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dfztgkad.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cdskhzmz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pciixunf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tqswzitf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lxfsgatw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nzxcfwim.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jnwlljbp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rkfssaqh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yfyedodt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cukajqux.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hchdsday.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eijyrknd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2woonlqme.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uexwrojr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnvcuhek.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxcanesv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hhdqgssj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mopmqayu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lqnibgfp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2anfixbxw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwfnsijw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ltabcmcq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ahgkxhqb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eqndguvx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptsoujoi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2udboyyth.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2grrbryef.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kzdasorv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cdfmwlkq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vikbctzt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tiltvdyu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vvdxoswi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2neuhqqhi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vzghmgyr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hxcltnti.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vayygsvi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2eoibjfxu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kmtbuzyu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tojfparb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ifbwmrly.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ckokaong.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wuiehctq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmrhwci.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asabxfix.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvbbzpko.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lybrzeao.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fnuhrctr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kftclcqv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zqydzjvb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hjvpioaf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dvpwxdfi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wcyknmsa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpgvdkih.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsfkryrc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2skrdcxke.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjemtnku.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2airqbcaz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wzmscwba.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zqbpqjxu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ajhpjzhu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ppqsefzv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vdkmepsg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pprvadwc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wjssfalq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ssyzhjlm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rhhpyofb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nhrgvrsx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ilvciczt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zqsulqry.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aaryiwts.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ezyacira.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dilbmiqn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2orcibhjr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mgqdtwha.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lubsnmfm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eccqlzou.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pnykmhsg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ivqxlkjm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dsqnghog.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gmonhefg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcgoxrfk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tpcnozoq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2osfxmqfh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilcmiluj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2otxgkety.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2glpnjpxx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qzzbreut.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2idasgiqm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2otjrhzdn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mmxwalxm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ngplwxdz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2chvrojsw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2opvfsxle.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pglhppuy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vsstchlk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yebcakhb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2spzjdsoz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2webnskok.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rmwshfch.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2owznidxa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ynueimqn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nsedomee.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hakomyvk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zwhapidn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjwyxian.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iggevkag.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntocqgop.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgahqubo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2babkjpwd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jfdbdsnh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgfodnii.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2huejutfp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fuuzouxf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mlbujgki.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xubujrps.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2curuqpss.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibklmsau.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jfeftcyw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cyxuqcnc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dgaixexz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ftbljpss.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2oekqeqhj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bjhtdqzx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2stbyewjf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tpgmynoa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mttbqlnf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uyhlpkfe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ecelodmv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ddpawvdl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rrunxgwr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zeaxhqdk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cmogvdtv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ljtakvtw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2majlwgve.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2omxesgll.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lvruovry.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2djrhzfvt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2drogdgjy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nkzhstqg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlpjhtwc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2puiretti.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2haoupqoh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yojhjinv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqqbohl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtupese.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sfwsctpx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejqrjnbw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2owsrfwkr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hpuzldlr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2twvmvgvj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kaejpukj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwlatmdx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2girfdpaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qwtyjslf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jctvftpe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gkekklul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uutgfpgw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ltchlufz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asiutfhm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bqefokuh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2edcvzavc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rlqjytqf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqvhynaf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2djefabtm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2aznpzzxr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2slaqeddk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lrnjoaus.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gssykplc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2phyprkrh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tdjlhnbm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxufxdxa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlmkfpjm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wcdhvcos.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lrviiqkc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2utjdyltk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fkbbfaaj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aeucbqmm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hvxlicjc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2emoebyna.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dsgljgbp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vhdtxdoa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kfcynvxt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hxkuuscm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zhujumjg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pkqverqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nbgjsrhb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lqpmgqdu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fxwovdbx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2emvfyqhn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vplsetkl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpbsdkeg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2eigtgysx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lmzeiozb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjdhovjh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyelrfqb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ukcfvrbe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qywknbxr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yjvktblf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbjrzhwg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ooyvymvp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmeqswcy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlnamjr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kctnhjxn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgneiiiz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2fputuxva.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rfkvsohr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qhhhvqph.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rslbxpia.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rwpjidem.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2svykxxow.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hrcahvwl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhbeikn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2amgdvuxl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ipstypfs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vsgxejrp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2azytpkmf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wsanmllo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okwytxdq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wthjuihu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bsuhxdqc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ewwnxsop.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ejutwnda.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nwaksvzw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dbbmjzqd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rywmqmpa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bpljuqwh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qmwtetdo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ztbqcrov.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mwelojxf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2quazgupk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2kpeewdnk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hnzhlqew.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vpzajpch.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwcpuh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yymteblj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bzdqjnmr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvbbgkdl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pargnudw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2reydepem.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lnenisyl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fiajhfvm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tccvgvlx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cvgpafch.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rheppyyz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cfslwdjt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fhmhkruk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mbzuhmqm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fvuttxgj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmrxzscc.html


<!-- 参考信息 -->