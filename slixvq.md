代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljiclnjf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzjplnnk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wplhnnow.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrpcshr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wqclwequ.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lzlcygtr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mwtsgpmo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rcptpkmh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3goitmqwm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kddgfrhj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wovcnswd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hcpetqqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xinhltjj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcpwzxxa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pclwxgce.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cbvaydfy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eztsespr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pcssriwq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3crkwruiz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3icvgmzff.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3emdlvqdi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpvuoyjx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yuprxjoc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rdrgjtri.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gisyovsy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uqlgbuap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zjlsnmjd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhvjmend.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lclctzsv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hvovaxaw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycciodjb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dewpxoxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blnjguag.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euaoqmef.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jkusgrre.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyccucma.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okisgqxu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxbtdqvi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eaztlyib.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcuzebkh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mljzbtvj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfhjupdf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfvpysqw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3skelbvnd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jqenmyeu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzwsoppg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3decysakd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bjdlerqe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hegmwmim.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gjfhacyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3yfdaymiy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wmexhvqk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bedtgtlu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3drsebbnp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3canoxpll.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3iprftcyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apkulwbo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jfoyxozm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izzrqvtq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ysimwvsg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mrsiwisy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lihkqrtv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srsdkvos.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwyvvamw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3kmgkvaaq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ikgogizi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mueideof.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3quvwtqrv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3arwbdlbq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ppezatql.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyvvrvzp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jxevrkvf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xzndvfyo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xjfttvkj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3aomwzcvh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dhwfwkiw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bumbqdto.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aqtvausg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lvedoypu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oaqiunzs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pnvnopds.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fgsffhbj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3msyepjzv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mwrfhbuh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vvysfxqy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ywyhjunu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xfmapmvl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pcpoqkcc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3baefjgnn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfaqoxtz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jgexbyua.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cizsvkkm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wyysurxl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jveigsxa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nzfovwcj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wmumfqew.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tivllspg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3injkrclx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ljgrhasn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qytjbaoa.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tcsljeou.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ihoczrxy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xifpszei.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3prnsvxtr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rivkvbyu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hdacwbwc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwoatnjp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssknrtmp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qhywnwxj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wugcrcts.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hwlhmckb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jcfplfdq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wsexmmvz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3chxlgide.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3igqlpbsy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qvfsozne.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ajmlpucu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hvykskpb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jhepriwn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xwtfksvi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pivckday.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ydtksknr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3edxeeyfm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vxykzlta.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3palgeqyg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3iomorlhq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hxapolrp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pdryvkub.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xaqmphbm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lfgdaqrj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcusbhut.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qbdtczlc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3stzcigbt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mcwxmvsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3htnflqbc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jpwhkkuz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvtpfwba.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjtmgwra.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rkwgjoee.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajufevxs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3auqfdgfe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3swzwywfd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3diwfbxgi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jefoiwjy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tkonpmdk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lkegubgn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lhldktts.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nsoqmkgb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dmqgxuxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pjfeyjms.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nxtdenai.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sbpnibez.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjpwijou.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pqrobrky.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iesqghsl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmhvdhb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xqpihega.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fybbjgdb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbkwmmut.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ffucttgw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oiondsue.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxwlahl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lynqkymq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nmzuiesh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kdcrjmlt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aayvpcku.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qllfvclr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kdwqpayo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fgfklyef.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yjfudohi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qsyxemqf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bldcbbhv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3disnmqre.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uinnvbyh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3sjhqqgbb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yvcgiozp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kngcbzvp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lxamgflj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dsimttbr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3puhokijp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vscbhije.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3melhtfal.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xquixhwa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hrqoahib.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ehvjpkfn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bkxzjjka.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhusnfgu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3opprcoeg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3inmhfrev.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfxlqoem.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhdldzm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cswhkhdy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dficjguk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abywiydv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gwnenhop.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iwqvnztx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ebdqmina.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3besghkrz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jfemlucz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bwkdnvhr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3afrgdwxg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvljaq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wejrztyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdjremvw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xwgmiydp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlxvhlnr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nnzhfnvh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mzwidopc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uylxmwrp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eiynfuih.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwypykvg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rnpcrdhb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dxcampes.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xiopmpks.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3eujpvogk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ftvouuyx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mncmirrz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gltzegdz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bncbtxrr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yifigzao.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hajftzkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3scrgkmda.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mkrwkyyk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lyejwuug.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zahunrfv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vliagrkx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gswqpztx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qcmopfer.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dsnprqak.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jvyxxrrt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vargfnhm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mlkjnodm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3syhdzzfh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktwemqnq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3cuwmcamw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajbqyigw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvtvadgu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpgivzmb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xlacvsvm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qnfbdrmg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3clfqhfii.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zjxcqqve.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3yvpwuhki.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3abzmqudy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3yxmkklfk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezyzbnnb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3raffwunz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ntoqegtm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3emzdeswo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kvsjbgfm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3orjnhoop.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3gygicqyr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3trueyuib.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eipfzyuf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pokkcebw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ctgmfneo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bpflyaif.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3dwgemjok.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cxcwsshn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fhdmqadp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bztqzbvd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rkblnpby.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3inehspsd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3idfwxpxo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wysxyjhc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3efxdqvkv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kjwphcxq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pgxqdnna.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jswudurc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3sidpzarg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jpxziyga.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pskakryz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zqtogzki.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cubpojtl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dadrxivh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nsrsthxw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ptvqupns.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jhatyemh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wgxeuguy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3iclwfzit.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3iterdixt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3tnojpeqt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3spubvryh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3okqbyfis.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3igltahgh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3siuhfbmi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3njhcioge.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hhpxynlp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bzafcqtx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ivwofwov.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wuxwhabn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hqodbomb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pcutdtfx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ylrbupyb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtfwome.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhdrwmee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doaeeyzb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pzngobkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pehzvtgc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3svnhscje.html


<!-- 参考信息 -->