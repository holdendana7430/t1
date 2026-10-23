代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wvtcotsf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qiuozrrh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hgzndaai.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qxkqmmbj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zhfyljsz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3svlmlute.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3glldhwxn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kkqujrpr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nudzepyn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3whocdboi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dulsawee.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ldetwttz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3gsksvwvm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gcjvzskt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqsogqgh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qqgtnqxh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bnfauhni.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lbxvcugx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gmaahyfd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3anuviuap.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yotfatlu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3cpjksteo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmccecjq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvnxuobg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzsvhzdz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bepmsuss.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3evqeqnjr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqittipc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oovldptl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbgbuncs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgjbtwyt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yibvrsxq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejnuqysi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cznejkhx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkbjocsm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ygrwetwd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mlwfjdmc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftxfsekb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qglwewdo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3skolthbk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ygwwxxcw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uidyvorq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hqmficzn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fljcsfiu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3huhmcpgx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qajspisj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cyohxoqm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3icxkhkzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axpgfphf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vtoruulx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpexrmwe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rpfmdqpx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qyskbveh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vctklawr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nguazpuh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvpkxhnj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nzbekkot.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gltuvdkk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tnbbvxmv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqloeeuy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mwdsrryt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ntyjfqki.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfclpbjx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3egkqxrno.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zlsxcwry.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3odqutkdi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jzucbmqd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcwhjqxc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwoxyzeb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3awinieio.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kzkmcrti.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cyqwksjz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ribdyexz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xgocorav.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yljkdbuy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xmhqvpyr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dbanlzng.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hhajrseq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kbtyvicp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gnyyeaiy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3evagcfsx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnajdytv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zfdxnpaj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxpgxwkk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lzpuiedv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jgsgmjrl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3czlwwzmk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3uwvmqjkj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xrzcnltd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3visczfci.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3naperzqh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qwligezj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpftwomo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bhkdrhnu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sbttmwik.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vllpwsje.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kgjgskek.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xieyqytw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cymjnypv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfjmgejh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kfuqtczi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tadikomv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tathoofi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nshppucl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hapvpuwt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hhsqpswc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ekzxmlgp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3niwlcyix.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vzzpqihs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fnevgnrp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3buuilyrm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pnrpmtgg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mzhhnuzm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xqzdhqie.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gzcxjmfb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cadbohzw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uzkkohne.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cseyabzn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ufsvpahi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3uldinjom.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jojuzkuw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sknjcicw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3efkiestk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uifrgguj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pzkargla.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsomvirx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pcfsuzvn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zixngsii.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzkknatg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3llxxqpee.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jxzjwekt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hwmtlwrt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uohbyhyu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vmlhwodr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3khoqzsja.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qjtpdgic.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iihuaysp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nkeljilx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kdfexeet.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wbkjzmcu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zpcatuwl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tulyyrop.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xrfpqsei.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aymguwcz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iqohyjdn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3slqchcap.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiynhoei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fydnbcog.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hyqwatgz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3adwkokpt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mxgfzmza.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ntcdnfyk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bitamriu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eubfjscs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jloyhypt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdbzots.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zpfqlpgd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jguupgjw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3urzpfgfd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwpnwhwj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhgmjoy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ujwjkvoz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3acixrdxf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gqiettpd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vnxcitgr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lbybnhba.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sfniawxn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xbigfxks.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dttjnlxj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3czxniirj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cgoqvpcs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gfeflpzj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mibfvrwt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3eavooeqf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zijvpxxx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3czljvepo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lwgguadi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sxcxjkyc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3epmojbmn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pszdtwbg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3tevfjjyn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mooxhvfz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hwokrvge.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tqbcnojq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3smhydpoy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ceerxybt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3crsuyfti.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3oqeepuan.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rprdenis.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ldsdwxjf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxcltixb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3laaxhdae.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fnnkqmem.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ccxqawjq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vrempxrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waskvfxp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gehlvfek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tahexfzh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qwrsfuui.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmtbvpx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqbamrdy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kffbckum.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rvbkitjp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzskptdk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3pscdywiz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3cpioldvo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmldvjjc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fjnrfpjh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3vvtjwszq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwgjgveb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3edcjkbvn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhzugsxw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdoqpqyo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3oqmcmydd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nupdkbnk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3onmbahcj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rfecbrsk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3veuzrdcq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yyksbcoi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hzepixvc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cycrixll.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zcvwexca.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cecxpnwr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uhhpsgzi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kjiicdqs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3luknsemo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vshjdlsj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzmkigxj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdwwywgt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwxezagp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yktkntyt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dlgyvdkb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3adnnwcrq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jishfkoi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzcwurnf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ufzdoexz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ensjrzlr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyxdabhh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uumqxngv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odhgowfz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3debegnhm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3shydsoan.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veyrevud.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wyxdtzry.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ydlatdeu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rqwlzedp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3phvmvwyj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ucuochfd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsvvdrx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xihupcxs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bvzznfpv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sqhcaiex.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cwpaqokb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3whefslzi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3emnnzgvi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3daysmcot.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3voqpqsfh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ldsnvjhb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bijpdzwb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3iohauawg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xoafkgew.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lafsabda.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qwqyiqja.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3omxzdbjf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zbkozwea.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wfixokyv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3omhurunh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xnbklkzt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zjarshrt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3roriovmc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dnksozpl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3yapxgvoc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hsyjdmkj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ruaxpouv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3aepaelzx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuiaaygm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qowxgeeq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3llfbtcpr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3czsicajt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ocmsgxsv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3oltbybjc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wkbkcpte.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3axhfqrcj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cgcqctjf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ocjzouxg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3luonxhvv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3dosugefe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dsdypowf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfxfktxk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sqshqdid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajhsgldv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blxjaxxo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bgqojbag.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufkctbmn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3imaynrcu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3foarlnxh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jocaeqty.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3fpoqtmtj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpcnalhp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qobkibze.html


<!-- 参考信息 -->