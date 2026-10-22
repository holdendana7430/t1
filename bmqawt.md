代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vigzhofn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2frkanusc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cwatpfnw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vvksahnf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zlwmgeyl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yybkmcdv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2paqfvrls.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pksgkkuf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqjbjni.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2oyywxvhg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2erchsswu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2awlauqpl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cmkakxae.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqowldmr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tscrondr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2damycrcb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fueisaqw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kolurgro.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ozsorzba.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpcrcsmj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2aqppnlzf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2alrfxbvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yecuaoyd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvcorhce.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgrqfcgc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akxkupdg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pgbjgqss.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zddiaqlo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cflosaxa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxsilzav.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xxsftvek.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxoqnyys.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2omsctgay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkzqawoi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caowyxje.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ksemxwvf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zeawiygx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwbobyhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2txceorwm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mfgrbuno.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fhonuuit.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yslnqgbj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pwdawtsn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lvmdqaal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2frylfgsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oxlwyqvg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2stieyfbw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rwjbdcxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmpnjdvj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zohvqcht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygkcvsde.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vooqbodg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mpxqefkq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbpwruqi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kbyzsczd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuycbusn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzjuxvti.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kdlytkei.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2avrkkvuo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dbhvvndo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncutnmlz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qybbkhuf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkafevsd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eqfrepop.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnwnhusn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nhprrixx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2pbycztot.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zpbvvhmf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipanhxby.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lcmjwgvq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mqutxlas.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ahuwkska.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eotuhrve.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vjtemhrt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ifrvlidv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ixnktksv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jfvfjoow.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dqpnosti.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jdfyyrru.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bazxhzvl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrxguhqe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pnxgufgx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xrbfcymh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qttdeqlg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ptdllmdf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zolxkqzj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xmalsloh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2pskcbizv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2opczypsr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2khmgpcgc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaqpgogq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2edbnsfbw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bnqlgtyn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ayrakgly.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ypepwdxp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffwjhtox.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ygsijqpz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dczwpkcb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2prqzgrjq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndigevbg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikcphvgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2laruvohf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2avicyuwc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zjykhxoa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gixgzbvh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ksiaugym.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2aiflstqb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2helrzjau.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uirtdeij.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fonxcuaf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ibbpkvhk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ycvbwewx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ncbvykjq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ywepvmwq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qvnrfnpp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cjhyhxot.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkepmpim.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nzmalatg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2orwmsyhk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zzbxnteb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nfskfbca.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gswytztl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmgkodto.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gafxqabu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tlqkmmjk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mkzojgij.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2shafelzg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wbmlhvcc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2istqlyzq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bwuougya.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cloeytsa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ttgaxbci.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xreegrgz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hdbbsahr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mbuxcygr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rswksamc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fuowdqxj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zxvfnglv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pkvcxmje.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2phxowyqm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qwfviaql.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kowfwymp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2piuxxczc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlesolb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wnvptyxd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gghkrerv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nygvqqjv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ysihcpoz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ujxqdknb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rppvgbra.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kypslsjo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rrejjtpz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmqvgnij.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rfeumgxk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwfzcqta.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fsrvghim.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wyamywce.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lxybqaqe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vjxlhvov.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nzldqpfl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ufgadoth.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nsjkyhhu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2izhrqvor.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yaxyyldm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2armwbfzz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jgpbspwh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jcnmbezt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bnswtxmc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zcfjkula.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2msqkxqlg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hxrkqkdp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gihcguml.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pdyxathw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hmexoudv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wezedouk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jcvqoalr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qnzxevxx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ijsapttt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aapdictd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kzqqxdgb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2soacplbd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ajlizifa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2auwsissn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xrjhywta.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qedjcaqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nekpsauw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ciyaomyi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nvedstth.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qbrvupgj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkgqjbva.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kayfafin.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vlwvqclx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pgbqcrwy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tydjfdnn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mhasxsrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rygrfpjj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hnryzcwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylxkrxpj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qmedxjmk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ykssurgk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2asaxpfis.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ngarxqff.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tithaaha.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dallxrkd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gbyrphpv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ycernfxr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndlcatsy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2prtovavx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wzdeeuxe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tacgcneh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wysfqudy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bervinow.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qasstweq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2txgerlcf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2sethdzmz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtzonrvm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ercdbacd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vytyipiw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xdbcutkr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2svxqqloa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cewswmtr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gfrhpwhl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfzorxz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2szrnmvko.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lyubdwbr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pmhfkjmh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bjmwtwpn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2njbfcdqq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmpddmdw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdkhfooe.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xloclwsu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mawrhznk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtpkhzrk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ghwhlrne.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ueexnsik.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bjythhex.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2atkkychm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erqxudnn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2srgouaya.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ertbtmpm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2cgcczoaq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2davwqetp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nhysrgea.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vodhwnij.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2juplfpjg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xvksghzk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bwwlpxjq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cdtkcspf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vxuofknr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wmmjldql.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2flayzzef.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yazyrbyj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vvrpbcmg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wzqmorod.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zdiigygj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2osnhogkx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ooawlosu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pvrsvxhz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hylkmdno.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nmxhiatv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2svksyufp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nqvujicl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ckowfqni.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2kciqvsnk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kwydyess.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yufaoryh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2aanhywbo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yobjtpdy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2sndqoyrh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nmbktxzq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gaiwiqef.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2knkfavnk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rhktboau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2eizsstbz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2wjbcqysx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wxzfeggl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2litqwekj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hezjfsii.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fbqjtmtv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hmrpntci.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xezngfcx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gaidqorb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zhppbxxj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nyjhlnoq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zmitzlky.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2krvoxwcx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2engksogv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cyqyzvid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcemvjok.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ojgerybx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exndudjf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hafhyury.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnhqpqf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tsredgpj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czahdaep.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fvffrhrg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qfximluq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbxilqp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hvojmwpb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2errleixq.html


<!-- 参考信息 -->