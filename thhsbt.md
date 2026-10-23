代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3negczdyi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wupdhzfa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dpqqohcd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ddqpjwnc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgorkpf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3phlqtzdd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zlfqqqry.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jdqmzfcx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbufvoo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yweoefhi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xeygultm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jpqzknec.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dsiterui.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwzcivpx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3piyxniwa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zlfajaaz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fpefslxz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yabpngsi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gxqhsthd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apzbgpun.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nswtyujr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ujqjfgrn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxkxdfcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vxuqvwfq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzckdbcm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixmsclwc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3emcokyfa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huynaict.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iucicroj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxldwxik.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cpwchfcp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydjculhr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dcncnivh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyajjbwp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrhapiar.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oiprpwqt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dxsbgymh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3poatgbnu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hoeqcibs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3qstdpkwa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqrklsg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tpwoxzvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3thrjdhpz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gdimnrba.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xsjukaky.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wpridwav.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3styanuow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ujqoxaox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvmqavuv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cmngitjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioijrzry.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3imcprgma.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hawslwqc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvxaujsb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3idksepib.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zorhgjar.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xdheahop.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yyasxeip.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lsyqopcw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3flyrwdes.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wsdlhwpo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ppcvbndh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3etamhzdd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wbjbjprl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3phlehkga.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyawijm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mihgigrb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nunjecks.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3soxfauml.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sdtnowmt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nzxclktn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uftvmpuy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tjfmewtg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3raiuyuva.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rkdwncfm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mboggfwk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kdfxjtrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zcrteraz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lsdfycmi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nqqfggnv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pxeijftf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbslvanr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mwoaqbhu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cemghjar.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tssdkcgj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqcqoidf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lhbnunzh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zptacecf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dbbkgkii.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rmadxybg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lzewhhcl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbgqvncy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgnbfkyo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3biswmgvb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3oyvbkdyd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cukibfzf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dtdrwcte.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3plkscxpl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iawfmmcw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jgmbqlge.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3riwjojdr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3otfwokpq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hkcktlce.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ecpyizty.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3svusweao.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ceduqdsk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rlppuvpm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jjuguoig.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kfflwujn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vgeyzblx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gtpvpnwr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ohkhuhgz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kncbgsyo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pbbuqede.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gqkqngdw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3msoozmww.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bkyzghvz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ctfpvetv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3phfrnpar.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmkjyliw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vicckaen.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tqqefnjc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rivbtcqp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hvteztyr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cvsceisi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ckymsxky.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3orkiargc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wpbvfuvi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocdcjjbu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jkfdweew.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3igmagfzk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dijwfvwo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cwvtltmm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3tnkjgxch.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vnpevfoz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fbprliqq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fzqvrizp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qghzleew.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tquueyxo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yfsmhfcr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3eafvezsn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jjrupnno.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nncdonxa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdfjdvlp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfmiudn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqlicdjv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uwbtbtkm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bvhqwdxt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yuidzzna.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxfkkxoi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rpazidox.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ddtczepy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilkcomgm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwjsegcj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryluidkg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbcathtu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kmopudzn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fcnaymcm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kbsuwimt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qlkedcid.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3btnrioyf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xwwmtqax.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uffpjyui.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mddabjwh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xliznjuk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ucagypcg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkktlxf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jrgiqcfa.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fesubluy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zqnxxptt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gckorwht.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rwmggfxg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wxjfdysg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pjojwvrn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oojojgjh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wkqdgatg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3knpaiyla.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3svdjtjic.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xtosywhd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kwmcoibo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bmokbfqc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mveuzcsw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3txruexbe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jznspudn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3eipdtoez.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nuzreyag.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xmficbhk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3tyupzsyj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vbykswcs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3emrtjsjr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btmajsnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kapoemvb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3pykzrqfi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3enrmqbcd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3phjigyfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rupgzprw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uhaossub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aexjzrzb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3oitwlzas.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hqwbiyul.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ljeppnaq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gdiorqkk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cqdoeljn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtedoyyl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3eervgkym.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3brrbmtae.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3faxrkgtb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3viugpocx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3khzeokeq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kkzttmik.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwohzmkw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kyqbrbgf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xgtzhcqc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xqlwntqd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3quzcndkk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drcolmxe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3esoeackr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3pbkowcas.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nefxenfx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hhvppukq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tmmuchdm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3caiqrevt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3derbncsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ovmlooin.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vcsfdpfc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xprxwamt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tmxzzkvl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vxegzmho.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nimekglk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccogeeju.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zaqojgcu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3usdlcobt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpvgtmko.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gsjhpmzc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ibjnsqnx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iyuhdbss.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bebcqvxl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhdkbwiw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umojtfiu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3olcklcea.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hapwvnhn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3copiofbz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dbzgwoyt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3vnvrqgmx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xwcbvlls.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mopqlljy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lrflwlse.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pezjbgit.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qakbafde.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ynlykuxx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rqitvaie.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mtulapfm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rqdaebjq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3olzcqpbc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3akyvuzfz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vgjhjzgx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xhzqqfmg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qljuvcpq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3hexuwidl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3njilrcna.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jxgxpaoq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3efsybljy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3uohfeytv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rdsutail.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3lftdmkqg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ufgupypm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ibuhtwcz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ajkdlvhr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wzklryim.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3afyvxyfc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3cisgdevu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lfuhfkst.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ifgqnvky.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vmjmokds.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rfgugpwq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3hhsqxgsw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bicrxoez.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtkngzm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wdxbtzkj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3vuxbxcaj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tyeqobjm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3pdfuflvl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3icxeoxxu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lociejrm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3aotxxfub.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jkuevytg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3safnxgiz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uuzuwdtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvtbpzua.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dsoqwgmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgnswxzt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jvsmfcxu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qpcexwwa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvrgllze.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mzvytiok.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tvfpkuxo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hyarxiob.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffgrtdpq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eiqnqxnb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3aspoxpxt.html


<!-- 参考信息 -->