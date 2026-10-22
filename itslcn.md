代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thjavrqe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxakdhlk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vybwyhrn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lcsiuwcj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmbmpnxn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eobaeiwr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzvalpde.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzjqqpx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alxotswm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjrukvzw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2amtlxyhl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ikopjgqb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oahcamjs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dfeqohib.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ozrbnweq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tfbjlavu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kaifcaeq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2timqojop.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2scgzukog.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwjgiqiz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkxihcy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rfnvlurn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hrakgcir.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dknarezk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uyphmojc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cvykaksf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pyyetksj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ugibpfkf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2glnmahzh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hknqysfo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxelkvpi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hsrkuwec.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bmanxfah.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jliycgla.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hvpgvzfq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2woivywmy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zeaxjoka.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qvexalfg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wchihbsd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhufcnbi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eozfpmhg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfknohvk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jludzhnr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2koeelags.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ormtyvmf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agaxaqbo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ipaxuebr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntfaltyc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufpytihd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahssyavl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgaunwct.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyovddu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rneprhak.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqciwqzf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mvgsibde.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2peanxbvd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmjzija.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gyucfixz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2prxsqcem.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lufwvfuc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zrvfhubx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzxeih.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wadieymk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2grzuoaoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnaebwci.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cjduhvpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swlfrdyo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dgejlbog.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hamtsjmk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmsedmhe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kddraelt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkxnvsxx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mgogmlzb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qshokcfr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dsvzyppj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hevbgnji.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jkbahskz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jzfmntrl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cgdokene.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueuvxtgz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hagjxihz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ujksinvj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ltptzuai.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2scirnnjs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qlavmzhn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2knucgglb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lobtucnc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2obmnbzgh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dhoemvnh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bnkrbssc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2eqvluptn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nskqcaad.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ravsnfnh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dndriwqj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2scotcqzl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rkoxuvbk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ubtvqsmt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ozdqgxti.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kjwgqkqa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2daaxzqei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhzgxil.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufcuctxn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yiyzljlu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mqsfjwwm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2igjqyczi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcrwwdle.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vokkoirx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2voxwrcms.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2umycgjhr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2atkszavm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yuebqety.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gihlbltj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wnfnmphs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dnmsqmmo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2itiawdeu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2imeujfrz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bdeopmxi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ybvdxjbz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zwkpezht.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rrywdewn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ukjeiwnx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2unapjkmp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hcnrobtj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivdjpcfl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wsbcarzs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yquahotk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gujwloga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xyfthnsa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2anpjwgfa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wprwewrz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xmapkkes.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2azqenkri.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2inctsnrc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kcyhrugv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2imxfiokr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipdgoied.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2chmdhbgg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hxjrwprk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2plmjukhz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hlokdbri.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2riqrrhym.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kjayumrc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hvrunpic.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rnbwhsqc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lwrcfvih.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iryykswq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bwngibil.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgzycdlu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uibzkfuu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nsvluupj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mrqyaygf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2krazmzqe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vqlonceh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fpkwblyp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2eopmgfpy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rtaadepi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2johqhfqg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gkldzlup.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2eaidmuut.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sdbuodll.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zsjgkhlk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rfklauhp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndhwriyu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sswefljh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2popfvgkb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ohfmnfdw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2uzfftkty.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2majicpcc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bsdrlcou.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyazhlob.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gtvuoioo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hekqceml.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2opqpxcor.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2giainlcv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oucqyqwj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wjnkdjmi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jlieaahs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mhekotpz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2twezhtqs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2imdoozha.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rftnfwdn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tzaccqwx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kkpjkmwb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vjhkjopv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zprqttio.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jfrhaxqy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mjtpzcbh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ovrmsitg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2sdmmnujn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2olyrytzx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rflydiuo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vrzkkhcp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qwnfntez.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ghqatufr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mamewrky.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dazhfqkx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cmtotnzn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rneozzot.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wpascnbf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjhknus.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2anxujoei.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2drwfpzpp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ljmvxkgo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cuhupjgg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qxlqhzmn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdgtbtdl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqhlmmg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gjgxwcom.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ggcedqdn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2krkkkvzb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qgykqach.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdcxqita.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xemtroru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytxayluf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bvlstafq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vcflrcfw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtfdatmj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aervucdn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cluthvob.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2puwutvfb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wyydifvp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yleivlmj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2uxvyacyv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2clfovrup.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mvoecqwi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lsmkrkeq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zxszfwvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvildyzt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eorjhwpl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rmzwkfcu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dlaswsvu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2syscdczw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kydfywss.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zhjbfvnz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2golxfpne.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hgukizxm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wmmsuvht.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jxbfjisn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lbzourmk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ksczkfop.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zuvjirzm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hqnrugcb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2znkcbbgr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lfcqyowi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gsopvwnf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbrztimz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fxhljfii.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vwsiojij.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vslaxtfj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dntlszqk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2eeifwepi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2eyytuomb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2weaewsty.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2smqfrmna.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vpxojlvu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2bpmaohgt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2osogimem.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rardsmxi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfqurdef.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ukgdrhkw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qerxzlmd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2invzwnos.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yecyugwg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2iaqntsvv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nnlxnguc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kyafliqv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ezguifqo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2byobglqq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dxkyidpt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wqdzkpbz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpaxsths.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2elwbiusz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dzftlnvi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2qtcknvxi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2adguprnd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2esuzylov.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mrnxrllf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gwypyhzs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fyluqbja.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tuapfdlx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hwvhuqww.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2obfjwcit.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mjaenzfj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xammvtjb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vnnbpsrj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2uanddmlk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rvodduho.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2fgnsdwnn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qzhhzvdj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rylqoauw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2iowvxlsu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zdiclulo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aqvftaju.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2uclpiqvm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xojeqdbm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2rpjqdvfo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lolxpjaq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2fmfxnfiu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dqiwgmsj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mxcqgbde.html


<!-- 参考信息 -->