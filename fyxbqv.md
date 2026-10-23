代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3bjunxyug.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3huesjree.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wqoipllu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ftugglab.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqxkdth.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvorlwkg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cjfiopcf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ytrmnytq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xkdlshml.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mpujxdia.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lbgvfdmm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lhwmwbpk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bbdcmeof.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eummkydh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3adrwuijl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zhyszays.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fxdlgzqj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3asvcmtbk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3oitjghys.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekigdkqi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3vncwflvy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dfqiltfb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3volqhiav.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qlwxsled.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzffdhxd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvphoogj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nuifsnpe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqqzyhtd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwclyyzl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sztdndga.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgiexcrr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3raivzmpz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ragrvrfb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzgjqtqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rojwsjii.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lmyzjzov.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gcueilxz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgdfmxqy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ancdeglj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uyflcpwu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jcaxxurm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ukowumvp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vzwzyuks.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uwusxcqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gkzarpgp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3djzmrhcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ufpshnjb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zinwbvok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrorpnhe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zhdpimhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxzfully.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3aknyjcll.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tgzimika.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3enjwsgzr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pcltefcx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3icclsevt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcozmrnm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3motnmmyt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdlcispv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3edwzoixw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytaaptzk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pstimldg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xomiabit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfefrwmc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kdxtandb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddvfqegj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cupsfokz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zvebwfcu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yragwuaj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zmypiylk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3njismfhj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wwlofetc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uvnwvvhk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wbarojsq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rmgrsruu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3edmmnstb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3grprpyxq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3smpcjide.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rynrqidh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iobzblai.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ljjskkir.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvperdqz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jkpjhvax.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnujfopi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bpnqemzd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pfiuixcw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wrsykuxn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rwxjmiee.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jozkubde.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvmeoela.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hpnsnuec.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3syvueoei.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xzsfjlag.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3anbempse.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3loglrddb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nndkxpwy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jswtgygv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3qcyzkjxi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezegrgla.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgmglshr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ojvykxje.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgccxidc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lenslexe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3nyqjxzlc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dzyqeneq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qapaynvh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pfhtphru.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tuckibol.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gkrvjdrw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kfdkaovl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vtsepbtx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jpjrzqhd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lgmyioqk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ybmrpigf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xftwqwrl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rpfxinws.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hahkbvuo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtfhdsni.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyjaesjb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqbpxegb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gebilsqw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3duwiumjp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eptyvmgj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ofxmgzbg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xzdjalbj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbovbzpl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dzljotid.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkywbznm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ydhseupd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3izgdrtcx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cwlduovn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zkkztgmo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dcgxjdbg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bmaqjsgi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qhfpxalt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zhrsxxrj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3swpxokhe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xcvjbwft.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ssqvflzg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zpfsjulv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eysfqidm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cdidxaou.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lfoodqsa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnfdogdv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vadgxxdh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvteqbf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jceivyce.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hfitoffo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vomfkmvy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlaylkyj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3goppmaqn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tqpudxlb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pngfoffi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuoghfnd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guesoplk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcczgavr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3owskgwke.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jldeoedh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nsqicbtj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fcggvoud.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ilnvzgca.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jfvcghrn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pxinfobe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jiaqxcak.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lhdomngq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rresjxxv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3skqkbizx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mgpqdlgd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lccnypwo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wxqgiywz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3huvsdrly.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3oaeddvgx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3sopwuagz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbreeoif.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ueralyaf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mrirmbws.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3czdyueqh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vhubmpjm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3butdzwxu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rvklzzux.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lzqcwybn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cxrupmrp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3czsqogzw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pysyycjt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zlquwftn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yysnjros.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ethugrii.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3unosuaop.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zbdtacel.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrkztro.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ghvcaaym.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mqjepngg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ecqirjet.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zfjrziwp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lgnpdnqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exfayumv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3qlbwddsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tssqndxr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pjtxaeuj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3unrthlfi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gocglrrh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mcqzrsty.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xqpweico.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ugtgpmoz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qfsuqhnf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mjdpepry.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3atnbcerz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fxbehdpm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3biubwmfh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3liqptdet.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nlvfaxzj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpsltbpn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dolquisp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ukfwgwzy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vjucbtsg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fhlzqaha.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jctpxqlc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xmlccobm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kmkechsg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ttsxcdqn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wowmrlii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rfiwqxak.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rupghxot.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nriomsax.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gldihtnm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3okvimwjm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvysoial.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sepmtsqz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aznzqoze.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jtqrhpkz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikyfccpc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jexhsnmo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkopzowx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekirtfpr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jxezqmek.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zdbfhigl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dstmrbhq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jkbkench.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hojvymvw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qedaomgv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hbbekzwt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3agkpnufj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqtiubyp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pcjpyllg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hxfsosxz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3aqjpkslp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3atzfczwy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ihcwlicw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ewwqrjma.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jkyrvnpw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mhpdhcxt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gllivdra.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ceiavurg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3howbeawa.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eeficgob.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3keczspvp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3isbisbia.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3bwngxswu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uquozcpk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nvnqpded.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbcsgjy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3catcdlvm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3pbanypmx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ccabcwyi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3lbmldxfn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3atsajhgb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3puigsvto.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fzycrcwx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3vgqomgdv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cbizuoey.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3qgdfhwhp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3tehcsknw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3iucnniau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3peljjtsw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zjcpxhny.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3inlguldf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dveyxbvn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dbtwtjkk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3lkkrggfh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3latzclfm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qovgeebs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3slzidjsz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ixtrghju.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bcrgnuot.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ehlkwbri.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3eczkmtni.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rrvgtacj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrizdame.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buktklhj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vthgvbuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idhixaes.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3mtpdfbat.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qwgcfcrn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3otzxujnx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ddgogttm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nsckpajz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3utpmldmm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lapotigb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3papqnjyp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3awgfyahk.html


<!-- 参考信息 -->