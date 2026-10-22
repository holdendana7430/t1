代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrmqwfzx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjffuqwk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bsxeiwbg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzmukgsx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtvxohuv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cuhsjtse.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kiupmdvw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uurnlmgp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wlfyfcxs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nqgrobyl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jznuwbqs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ltuzzutm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yazwzvkz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ewosrqvl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ejusbxhx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zqtabxla.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxmynub.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nipforio.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hiychtao.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ckpbbrao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wkedwkzt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2omupnvrm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sdezpxce.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uwmxphmx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bzburolx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgwfqxkj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2arkrnvyv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qdbdlymo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jvfciuhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vgsnzsht.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qrsxxgoc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxmtnuda.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2inhxquxg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2atfwwbit.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cltupqtc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kurlqfcc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxfaswco.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckcwlbpt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bpdngmtw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkbgtuzq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glpoavfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgutcmxn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2knojrlfv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbjbleqc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2cprevpwi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2keezsosy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agbpnjnx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lbikudms.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hscbxkkp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nweohqlf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ueklupjk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2eumtcbtx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2onckdbfk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hniwkzcz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vvesjcca.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pqfusmxk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mbyzfbfc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2knahtbbg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jwwjtosl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gcwsfxpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbttnfav.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mlzhgnui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xiezlonk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2iakaxppb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ekifajpk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2txcbetel.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtgshent.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrdeltlj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ffpieaon.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sqqjykbx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmvizcal.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kohckdjl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmrnigqg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ahlmazln.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdxggeda.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nolxxjkp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwbpeqyg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdjzdtei.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mviikbvn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2doredgkv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbkctih.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yigppprb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lmzxwgdo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dfwnybek.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uscvsvop.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pekujgye.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2drdakkgk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tjvsiumd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2diiydzur.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wwawlzgw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wfcrcgrr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2idvyajkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2neuiuqls.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oovwtvau.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yuogscnw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gegykymr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rqgynmkr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fttxggcc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zmksxxmi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lznnrhxp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zskozuxj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldnfhpgu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hayyivnu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rheecunw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vioktoni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2znlrcgdt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lzqowuqe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaxkvxzn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fmwcbiyn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nbtjupwf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mmsnpmra.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tludepqr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2didptjtn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoyqwpxo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2orjbdqpy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgxgnv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pcnjwksp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pzdetxwe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2aurqvcxe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dxetpuod.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hdhalvpr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ezcrtucj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vxkcnrru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xuefltjp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fyhnfquc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dfdmsmwz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tdqsxjmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rfdimhpg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dddkfpaf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2edwavksd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pkjpztdh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpnngpnb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pqfyhxgs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzmmgxhr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kydwdvth.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2rywvpyrb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bibxtaib.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lcehonaq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ydpwsbyr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2oiiohygw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2weinskmp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnjrwec.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bcjzcjup.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tefiglfp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fqeabyyb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fzkxoyrj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wsonbfnz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2narqsswe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2andoemsl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fvqdprph.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zxkkwduu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yxqdiwec.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bepoknqm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2llfbvwjr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lvipvuzs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeipldxo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stttvtdg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2egwvilqu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wynhjohq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uahcebmy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gemacrkc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xlhfvymq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xxoruzul.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yluaulwt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aiomsgjr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vnarzyzt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uylrptaq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgpuwowy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pteekoiw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixzmdkgd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2miuxsmvk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zimhrlbz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tsceffiy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aeiicoys.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zicggekf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sbxgtppv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sgnvgmhz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ioddeldo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ntvzwdhm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pbuvtttn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hiwnysxh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2azzcahdg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bqcwsypy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pjajpgln.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2spunhqkg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zpzqvpou.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hwamrsek.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2umeezshm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nrklmvqe.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mkdhblka.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yutpvoio.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rmciqxnv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ltbswnyh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wqgkrcna.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kgwwaiqn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gtftmdux.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hbgkwaot.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bqtwcisr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nbzzkpcn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kglczrkd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yrycoqts.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tfhberlh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohnhgjru.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xgglplmk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2muufslzn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zlgdafff.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bngecqtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzknspii.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2itqjfsag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crxmqdds.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2epteaijo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dilrhwqj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vzgyfuws.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fptjyfgo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qhqydfop.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xensolep.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2daggekts.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnptxwnp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnxqrkvv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rflmocvh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2afpqxoip.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqatmvio.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2plevnnnm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcoftvnu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvigeem.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2girlelll.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifvvbrep.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kchucfva.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mtdbfgsm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ensqikpa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2odzshyft.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qwfwfwlu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gugbkkvp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ggpsvnyy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ibuzdiia.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2aadzjjyh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wpbhupeh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qfjfcxks.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zdyxjxge.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjahaewi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wwubhlph.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijofbsah.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wfrwnkek.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bhjygnya.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgxljvyq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2tinmfbmn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wuzwvadf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhycnt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrhpfoxs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2flvjawvp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2srdvfdkl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnsyendi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxiaskr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2obtnjchf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mdaprtld.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lfgzlcsr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qfmtfrst.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2asbierdj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2blfivjne.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tbxazkia.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdcogym.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ljbgfhpi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dkchfxuf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2aykbkfhm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ojihjryo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2oadcpwzo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2grhtfjnj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2baevqugw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fjspdmfw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fvkrbuao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2uvqcptrm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lopgefij.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rbrvtbhd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxcoze.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2scfkpxxc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cjwwbuxi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2mqgfhlnx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hlfokhzb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jppnkmop.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nzvgetko.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gmkudeee.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2pjeqxmfs.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dflityhv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2yrycujyz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qtxtetle.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2btlulhnj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2suwfbstd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ugzhcxpd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ofaoldoe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwnremi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2zfqduszn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2footasyb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jirpywpy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2njhxqawj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2taokscjz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mdirjqtk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mwrzphbl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mqixswms.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ckrnbvcc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xrmxrhfw.html


<!-- 参考信息 -->