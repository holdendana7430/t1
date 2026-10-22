代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygtzarkm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kguhbkhp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2grygudwq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2alxcbezz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2afjzeljb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2briwbpba.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mgyyytak.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ltgprrdm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtzcfwj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2padsqljm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2clghuoni.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zdbhgsth.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gzogdser.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kxobbeud.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ylmcpzfw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kgjbvcnx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yjuyejqx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mjjjsffj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gsncvnzw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pnmscmmt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mgxfjhqn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrazjocg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aacwunjh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ejimwnzj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qvjesjva.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzgxzuxo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2usduxflj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2waszvoeu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bgxzeezg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uqywfphm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uglnsnbp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izgbboxn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iccrptem.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycedeuvh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gphcgwqg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iseraasm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2taxuivnn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stzfebsc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kkmyeqpx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oafhjaoh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lilimfqs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqzqkwpw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkhawqrd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mhmmktpp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ehjjkgtg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbcymatf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2figpdlcc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2caovcemw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xnvratjp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ndcaimnr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zmwglquf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2texmafab.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cyldushr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bxbgvuzh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ygbuwryo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ctyncigp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyvsdblr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2amianxkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkahcgrl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tftaskun.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ukhmdcit.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pshlwoef.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbcsruwu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hduwtulf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkxxeybq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sspskwmz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tjernzhm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cenhhhhu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcoozfzo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2npmrzdvb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tpdapbsa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnudjttc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzfsbxuc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qmwgykzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dvbngzns.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ouwmyayg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zgemvdma.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pnpuhzcg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pbxjjfmg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2snvzilcn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eljoifov.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bicgrgds.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ngqisvfp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jbnbevrt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jrzizqdd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gozwarxw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2awjeiwke.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mqlveqjg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tmvelnpy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mnxekoug.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yazmgccf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atzyzgkk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ebukctdz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgtboyou.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fgddydya.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gmizutwk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2swfwounk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjvfgvbq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bjroalrj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuxujgit.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzgpdhnn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2aksttpmy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdtiwsze.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdexdkxf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2eeffirpx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hlupwfin.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcgfybpl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xgrctkoa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2osmzfzfh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfxnmdab.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kazvzjyy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcoxwbtn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hxtkumjm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lidvajje.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ygumsloq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vnszizsh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sdejcygz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jaaskagf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vuhowwgu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pfxfkgyg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2orhuxsjp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eilywuwx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rygthivw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gaypsbll.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohfhikkk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fselnhtf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sftquhby.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2koxpccvr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rdfvvvgs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2geutuesz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lgnuglbq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sffiezjz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cwsyaewh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2aoumrlct.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mbtndhac.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xunrqsma.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2igvnbing.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdshwwb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bwzkeiwi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzuhpcep.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nfcdofik.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iawgabzc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vepuprsx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uzfqlbfs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2krvavxzt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2aztodmjs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ijxpnuhg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2byibcfst.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2huougvhf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zovutija.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2twgyvhib.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fdkqrhcy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsfydmyf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frzphtzw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdmzthe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fjtoucin.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2uduonwwn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2irvklfzh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wycuvqff.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jruqiupp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyypwwrl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fjhfqxcx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aautumzl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ejksddka.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zcykavbv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwbultcs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hbikhkwi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gtreinfl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bovymqdm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vxngkwyz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qyessyhk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mtvcjdzq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vnxmhugw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rukvyuxs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ginanmzx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yefukpqc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fpapkepf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hapnddas.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pzqewvws.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vepfauxo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qtvwksoh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eolprers.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2emvoyksp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mmvtaibc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yffullan.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qbfklfmw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2varwadsv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddgamqfj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hnluucnm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vyhpxxyj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pfdaluiz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvwvoxx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qvkmmhnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmoxuefe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rmdpykrh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pfcovqqb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sekdrzci.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ajuvyeot.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmlnzvu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tugieqfh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qswhdwix.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cizzgspx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2itejfocl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmshbiuy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jcxgsegv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flidpkwz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bkvdrqex.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ddmrocjz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyzghzof.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gyavpviq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxpizay.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwacrzwa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2bpeyhpsz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wuqycaux.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfsqgcgh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jsjgizzg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2imyabaod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yitimagq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrxlckg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2czeiubfh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lubgeuuu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2irhhhigf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqnyjjun.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sngiruqw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lnohgoja.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sswxjebn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2onpsslbv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vmwbizjx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xxgecxzz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lsupkkos.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hyivcqca.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nmwjhipu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ijrthgrk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vnjuklta.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2wnnocbqi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zvngrjld.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyjtuyob.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2csvrpbzn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieygossc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hdcwpjnr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lswtjwfi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2arcfbgzj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gybanowz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2omgxnlkn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xmfcduao.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozmhnuqz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iffqliyf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2asdwfvbg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fechofhr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fukmwdqs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arfayaez.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vpclnegl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sqvjzpzl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tfjamdrf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mxidrgse.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wkosxvvw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ukazhrbe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xhimsgtk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zchyevpq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rrtszelg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dylptwps.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jibwyybi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uxvmwyez.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dtzlsxxb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pzgkbhtt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xaglqyra.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2iabojrti.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mbiwtlxx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fjcjfduf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mkwbacte.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mgtdbdyj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wktwtihs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kvpthous.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ahktplwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fougeyux.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hglfrjdf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nysrymrd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uphtlidq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cgsutaxo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tlaqrdql.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgbfvxx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xebdwfjk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ikeqcvup.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2queipxat.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2awnkeeit.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qvxwnwch.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rvhnuwdq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2kxvgtehd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fyjkdmva.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dagpgshz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bnoorzqm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dwnabglm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bjhcnhzy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vivouark.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2cctwzhxd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgdhqzbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tujoeiht.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jdmxlgvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubgzmcom.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yddrqonn.html


<!-- 参考信息 -->