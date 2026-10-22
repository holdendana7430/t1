代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2deexfigb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thbmoxjf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xukaiats.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxvzmuac.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajqtaogz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mttuhrbe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hmbvbfoa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2unohzlvr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bxcqxjsn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kerrevzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jpwtucqs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nfqhblew.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lbbctpyq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mdbmmvia.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2buympuob.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vzfkjumw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyonmmb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzxrtnca.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ixfubcnh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2okagxqje.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhrtnjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iauphegt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lpzojbqh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ynrbvhyj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nvikvvix.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqyrumli.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdcubwqh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dwdcdglt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2olwndyjt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vksiwbfp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2odvulvxv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjqjhtvy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mgsgrsuf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sfwmskeu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mejuxpjp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bgxaufai.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwhophhz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvnhisqf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gcyjjtng.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knpskpcn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbgazvuj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjnswvzf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lvckobnp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwcobtug.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2owvwrdun.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dutvlnao.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyseutns.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wgsevehm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2alooeaxg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqucokmc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ffmapttp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2orylqmzs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zvsmuylt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2puagkhjv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fgevasrn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2npvthgzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tdadcvdt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qdxguzfw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vyigziov.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xwcxyjpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2joephikw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ygsdjdey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyanzbsu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2urgycjhm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nkdvgqzv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcsedymu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yamneeyj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhyzges.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbwsofml.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2htwwpdyg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2puatqinx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jqasmfbq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2httnixbn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bcjqjofe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srfruvfv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ixxpriep.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yigevdxi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2faacnwzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hondubjr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbaededw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2npxpelej.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pyuxevwu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gvianqhw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2acdavlcp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rteptxhe.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2unskwwyh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zkcavmrr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yhwnrvrf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tuvemfqa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vvlwvpne.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vfbnxohz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xwrwhgsf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gkrlhpkj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsoyjfwa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xnkcyhnc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xsuqelhi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bihejlwl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ksfhhpql.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2icgjhxgw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tmozjhtq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jzqqmhep.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztgcgtyu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiqitxse.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ucgluoof.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dopivylp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lxwctpzx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dakpuhwt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhkfimhz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2huucvehh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ykczxhgu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xkyalvol.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gauaunwu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2scgrnsbk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snrygqxo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lnkoigny.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bhyggyfw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qbinatjz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2trnenmam.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2faqpgbjf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2anrokbug.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2chmmdqcy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yyaghcfr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tadecwtc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2npgfoqio.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jhcwburr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jjtcpcwj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ohxlshfo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xjqxranw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pvoqzhyw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bequxpqu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dfhnqlwm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqxphlpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hsnhpbls.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ryfwcmnw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2timmnuzy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2seaypgci.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ulrrsyxx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iddblrpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2imfpnbzz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jpgagupg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpbprpja.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2geggmnlh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mnmcjgqq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mlxuqxsh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2axvbfolt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2oouavnlz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2crsqmkib.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vrhgziue.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tgsrkytf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pxvdcbvl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hdymezbh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dcauoppd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qmyaxmnn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jirkwckv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ggdqumfx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hrnlmxgq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2smsftfxu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qcpwudio.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fliftxdv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yochhktr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uzhkieoe.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pxoedxho.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tvmzqril.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2caonvgif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uofbqfyq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzkeetdt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xyofxqzl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ekvixrgz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mwmmpugx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2beewrmun.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2relwfwkl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2sangqqdg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nzalbpum.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yakytwyh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2godsmgho.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ijdikfbp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zlaywkjj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jjbtbwdy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fpmqpcuy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2guytkacp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cscxxdfj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fgppsvef.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tvxeobtt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hovgltlg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2seabbsbf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhomlwvh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kpzoopkq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rskdgqab.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xhpgpqut.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fosgwqmh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rftudzsh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vuhmmrbs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lyqqkrnh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2issevlzd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bgcgajdh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sxtalmar.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jhrkdpna.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqrngeew.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rkfwreso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dpywoplm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bcvvaczp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qvwrtxjp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnxanhs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tidjydkk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uoggjlmt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ueftikrg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fljzubnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onrlasnu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jjnhwxqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmupawbq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2othftwqx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fpdhzceo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckymsekr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kuwihcqw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2heypulgu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mazthmba.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2efnocyel.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjpwwwuw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgotmiox.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xexzadgy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rvzvpwxq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhfkalbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ulczhodr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvfhapek.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbxumyly.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mrqsyhil.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nnjnvxdc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qafvcyme.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cstdypha.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dsoqstak.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2avxzgtjt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xqttaiul.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pjiohyyk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uxmcrvky.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2awdxvpdy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dagdwacr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bghnsfpz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qmjqlduw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dfyqknie.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2prmbnizj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dabhltox.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2icoviaar.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xjxmwiei.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fmrigcmj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bkvsudyu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2djbmycuu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2noyzkwcl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2utsaixxq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2erpzkgvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2emoxmkup.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yxpiziwe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2btuzpojb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2makvnunc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ijjcmkdf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cqxvgcet.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2epineivo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tojlviqi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cxbemmzd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jcpnrprj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rtfrwuxq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfntmma.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2piyrxiui.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kjwpaobd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ifhjsvta.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ruqsxfqf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ivimqodf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tphafzme.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qbimihft.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dgefpygt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cdlodmsg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2znogiahg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjhcjb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fhuircni.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ruonsvwh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2saxnmpvk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zevthrta.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2oaevpebj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qloujybe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vrsznwrm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2laqaikhf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fdysyvnx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2eitvqbdf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ptlcdzbz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rqgogejv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kvhjfrof.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lydjlltc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dvqgmqbs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jqqxafkv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yzvtrrbw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2afyqntrk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lvughvdl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2aqsgtidp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gvqhgwpx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kstznykd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vjbxvnda.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xrwxtjvd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2xloedaql.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ktuapimd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2wmxehama.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tibgpfup.html


<!-- 参考信息 -->