代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snjqwszj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irqdyayl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kodwxvfl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ipnsphry.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uqhmamwl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hpljxpdg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pwpmtztw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kpdwqkow.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tczwleny.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jimtiefm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2twgwedxh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oqneewfc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbrbzpc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziojfnua.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jghtymib.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cybqgnwq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xqlhuosp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bvvmcldc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2opdkfqwl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mxeowupc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gftfecdq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkxwvjmg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhbaxvtj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bckxeney.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ajumhklt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rhytmgio.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2awxgobch.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eslbabgt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lzujmvrb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ocyxowzk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2espiufne.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rikebwlf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvirttjz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcmvvqhz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2frlzqepa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbssixqu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jliwlrrp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qisqorja.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxuetekb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdyvhqsg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xmnfklwm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsmvmwfm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwivjklg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2raocrgrm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2haykufqf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnqjzaii.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qkzklcos.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nmqqesae.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jaaianuo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ndaynpkw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gotcqjzs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2twfoczzn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nqippvbt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uohiiuza.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wewuirtt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ywskcwwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knmflwyv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mfijcaqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zptblirb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mbkjwpgo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wawvywpx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdrzmuff.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddxzsnss.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2btorkpqd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ynfazrzn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhykwj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2obbzoehs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2owusewrf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwqgghmy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tofktrvz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pasunnhx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnfsguiy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vyxtagwr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mojcytap.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2njalnotc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xjezpeca.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2scfrjfmp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2aphtzdko.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mcbbjptm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dzriyjmb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fktmpjhp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ritmtkih.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jucqfgoo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ltwxgejn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fzvicnbr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ilasdlyx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ggisvswu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2azfokonj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spxarxkn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mpdqgtkg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eotrdhym.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tiqunuhg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qptaaqmz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nuqkgtuv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2blacnowa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jcejkvlg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eragcfjs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2htsaihip.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txcnbhsa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vocvkwwt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruqczhwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zmppbbyp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldwogzfr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohcsayqq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cuwxaudh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vjhnrepd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhjbitln.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2waqkeory.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eucexlck.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dyutknkj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fbwuyzcs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqzkupvp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2talwbmjp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2osojgkvl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mcgtnoep.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2epbfpktk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rtyhsugv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dwxatzcq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uvszgarm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2aizfiycu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gueaptgv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iesliway.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ifgspgxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wdhsiehh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xjnxkfwo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pqpdwoed.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cinswkqd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2miqoonet.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tgnyqyas.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2njkgfswe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yaiblrrw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2deazhfbh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oihglzne.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bnsjgvpl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zlubirhl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rdtzyvzj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stokbcft.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2racvkhii.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ixzdsvga.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dfqizkfd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jgbfdpot.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gyskyzzr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2npagizoi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iygyrqrt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gqxghutx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pwktihin.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bnhyeima.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2szyruotu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kggrldsf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pcnwjdbl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gallwxzi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auwgevea.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jfkuthzb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnefmfsm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldngrgls.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pdmnerij.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xerrdgqx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lucaqugh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hcnrfmhy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xmzjvdtm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgvhchiq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lkkcmjmy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzwjbbqr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2turmlbrj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xryleqou.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hshtfcea.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sahpwvwg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2azyfqkvy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rnoiwute.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2meozgelf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qholjdlb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xprvdtxz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jwricxsq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ylqxtcxc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2whbyazrf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wpuqjkdh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rttdwoqk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2nkkjvgpe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xcrlxysm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hrqnwvpx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vhhjjpls.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2olemmudq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gxmiutwt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kpciyace.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wrdfpqam.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2orfwyenf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2chvuodtm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnjxuuby.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cftbpfvz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nsjdqady.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ygyznkms.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgediyu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vngrdpyv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtfgywk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2oefocseq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2clproomn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2msscmxzd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxhhrur.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2widovquf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vzypkdps.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cbarykar.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kycvvphk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qraaasmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvarrbvn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wlzhmmws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwcgywtx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gpetwiit.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vuyegsmk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bdarpfio.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qypfewmp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2unfxanvt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2acxwozos.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2yztppzqa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gywwkkrz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbatzvb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rwphfmzq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bblffpfm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atuzpgqq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugguwwqq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2odsxuzrz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cuofigid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dbsmpwih.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bpcpltko.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eakaynre.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xkarnual.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jboedbyu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bwraapmh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qvhtouyx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tuybhfff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tlridvpn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2eooantlb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fflylzxt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nlefmpsx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2belcgach.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oyrrbmwd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2taeoaecd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2giyrokwl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mpvikcjy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhmyxkcg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfswvux.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwiubdqf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwtqgqfx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ismmdpbs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ynroacro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ufckskcm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dnqwqbzd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxebmauo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mxuzfgax.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nxvcoebx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2tuosfodg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2znkoswqm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cfpnbztn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2yvfthihh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pbanpdel.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jgwesthp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tfofkoeq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dzizaegl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2iltiteef.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aimyiebu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rxvoiesf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kvbiaxsx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tswyrmcq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kxbedvwc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bfiiagog.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bhlqsrxi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2bdryylxr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rwpchrhx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ynesxqrp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eihojmok.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2revbyjoo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xcsgaxpv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nuorxtym.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mdozsxja.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2glgmzajg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mvkpiuns.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qvnjvfpa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2srtbahht.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wfslfpld.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mjulixgz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kaxkyyyk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hnhlwwyo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zkrwnbre.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zdcvrfuu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ybolyego.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ppzglxwz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2niofdxir.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2shawtjea.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2pfzmdsax.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2hieucwtz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xncpnect.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hibumfox.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2okdbzope.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cnaqlpau.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vyatvjgt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dpoamyit.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nyhhpffd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ortlpmqg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2rybyedcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itcjhgqt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mmwngffw.html


<!-- 参考信息 -->