代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkzjpiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pjqxarih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eihsgdqh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3iqrcukhb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ofecvkbs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ibzmfujf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uayfroot.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ekecgdpi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wmezcqid.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zldkqyqk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qqxlnxjd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3civfrozc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jqattdqq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vxuujkoh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nwakoupb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jytamnba.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ozmvbncg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwvllmfd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aemhoypn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jkxqzbxp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bttiwlzk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xufmemzw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ynddkvgu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjwbhvzr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3izlhhkxf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3spshhypf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbntrhyp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nazbmdwr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwywabnf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xijppjxl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iwibfbzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxspdpoi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjczlwti.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvmtmahs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjemxmgq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvdbhrvu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjipojyu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ingpphgw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qoxmmvqs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcatjout.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jmwrndht.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhuywbpj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cbvhahvk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bdptzxcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kohtpwri.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dgbepjcv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3osgpoxaq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ndwagzwo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3plgzjffp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fnjvjkeu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bxlyfcot.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kocwnkjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihkztbtk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qnhmadaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlpidcmk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mmperrbg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rpddidnp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmzfjgsw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3opqgynnl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bodbsuhf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jcckjweu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xkcetzqp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jbvqqpqx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyenfkvq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkspgacw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pdynatgn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vwcvymnh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iziwoaek.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3foytqkzh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vaajmrdb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbvscvr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkmeahvv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lytnhfjz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dtkczcit.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hhqvzprn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3efstwlnc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tpaqomoa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yfodfazz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nqjbnqst.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bibtkmmq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kbnobgwn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uwiuhsrp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hqxsbiyn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jxxfindc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3doihiwrc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3goynnhec.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkjovvop.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3whnflawi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zqudrriw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cplrfozh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tvkedoeq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ssznodmu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lvbczeqx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwolhmzt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ibqidpre.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwwfpwto.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgkcggty.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dkwrnqea.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hhllrqnf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yszywhkz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yjxqwlfw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lvwrspff.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bikckdtb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gltkqarb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eekppooa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lmkgefaz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tnkljiry.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cilfqiyb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vgzgghea.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qiozysdf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gieuuenw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfkfldpm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ozurxpgy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ygwbumep.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qabolehi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3aqxytkni.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3knxthgbk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3siknjpmw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qsfczpzn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jvvxddok.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3grorqdmz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ofpfvssx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3urwplilm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3thsimmog.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wetnqflq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3votniery.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjisspxn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ixrmcxvx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kcbqctbn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wwbfsmco.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jslpozxy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rhqoxmaw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3epptoydv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rzqjwlwn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3motfxprd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wbymnqnv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cgeyxvfb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vrqpudtn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jzmrwmzq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pvfbdhrw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jmrmxdxz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nndpuwjp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nstngvfr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gkjqodcq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mxmjhmzp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3exyrmool.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pmvnzhjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pxwnrszu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jrdghacs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jjuvmeif.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufunhhuj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sqscwfnx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zlbdygbp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zedccknx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rgtsdbxh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bhsjyfqj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fvdrwykh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3emdytjyy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gqmwlknt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qrceznuj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eoixvfds.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pwgbleei.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3romngzcf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3osgljiuv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vetnwybr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gywblzio.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fdyvsmln.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ngheezlr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hontsnxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nsxmwoja.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3aclgpieh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3aytcqeap.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3snllfeng.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zjnumsud.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bzroytff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ledbwcbv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tjudwmvw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3azoprwuh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ihjpnnpm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bsvmocen.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nuengrkr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yeugqlpc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hchltsuv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnpltpbu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pfmfqakv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgwxhiic.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3emreupaw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3uvrlfbcj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ifnbydlt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xyldwblp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dkpxawjz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3etfharxb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3iwfexaeo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bpjicmui.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqnvlrx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mjjnwmxd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pumvxkuy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jnlmjoox.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3payneulq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hshnjxxs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ckpdoxxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzgrlhyu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yirpqauu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lwqobrbi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fquvekxx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyosotdq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxhfufbw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dtxzclje.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tjyqunze.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljbcopqk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wrlpihai.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3apzjdpcv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qkdrouji.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wvoklvpb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgvbfxou.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwaitfjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3erzdhzew.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wvdwblml.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nnaaudbt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iaeeefur.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pmtjtzyb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gsrwxufv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fjwolhbi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uoxeyggn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hzlmjybb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3anyrpsbt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mjuxpofe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3eqvnoaea.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rfbviwqr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kekvyymu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3puoxavmi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pggjkwnv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyphaazb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aewzdmyh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vylnavck.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vxxpclon.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3shshisci.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3svqeblfj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpwcwpop.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lhdghnyi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rydaytap.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnomqddo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eowhdyoo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofjvfpzh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3iqpgcddg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3joklugdf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shnivtcl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kwdzmuhd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3snuhhnby.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zeqyirqk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bhqtuzgz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dpzilqto.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ovsbvpzy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3kkwpnlys.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3msvxeisn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3onqtssfu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3fkegglce.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3dqsochwi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nvnitean.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rzktzdkz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wukiirlm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lmfjbocy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3phhuylss.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hydjaazd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ifzwihmi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nfxsnpvq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qzsnbqrt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qxpcfooi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yipxluau.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mqaecklo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nrzkyjcr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cczgnpkq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vkldrzes.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xltmjfkj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3uuquwosn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ghtuunwg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qkdpuibu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gxoxrtxw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3frsdvroq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jystspos.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gppmphwd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zarogjmm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wcfrjuvu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3bpblboqe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sxzygfjv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bgahaaxt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zsbprosh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hmaxhqam.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hegzvvkh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ifyjjtpt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jtsvbqwb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xjcfeydh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3punjikys.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3emclhgni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlmipwsi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cuerbyth.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cbhoueit.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vodehvbo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qedgtfmx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnyivpt.html


<!-- 参考信息 -->