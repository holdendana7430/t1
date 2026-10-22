代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2loizddwh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kuabcvta.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qurchwff.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ezyycuws.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hcbrkbjb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sqkjwsaa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gdopcwad.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yowotapb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2efuzpzic.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lzdjffvw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ujkhjnvm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ticgevwq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mkienodl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxnomucp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hryvewzy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mbcbkwlw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mmqvytoc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2oglmghoj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ikkyjlmq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gptdrjgp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dlzxqbih.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2toxyjewt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfakbrlh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cojespeo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xiqnwamd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wljivwuf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2orplzvfy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2duijbhlx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hegflvcv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hwvdlhtz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdayqqfl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wuuuisvy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kafapbkr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlhahidt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sfhtxila.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbqcyuky.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcwxxabn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aealsomb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gmfzamex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2atgypkha.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztrrznrh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpuloita.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgsnhomn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykzqgatu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kwtqxzba.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niofkorn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rjehzlua.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rbzepntq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zwycrujj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2idizaumk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2tjkokoph.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vbiuyecl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qadibgen.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jqrksmff.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pefvxdgh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yvdnzzqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nymyajjc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2knorsfaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhsoixtf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lbwwsotj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2havazhnw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hznddpwo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zpwsvzmv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dqmpjfxj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdswsyln.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kwsvjtaz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iexqkqkg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tntcwlil.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lildtvsj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ggonyvmp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pxwmmcae.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dplimteh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emigobte.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2poklpuig.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ozmkzjpo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iybdjzck.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktuvmpsd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cywocdfv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2retwzooo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pozmxkst.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jmpvyrkt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vauxyfrc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ypwrtumu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vtmkurmd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2podtcbqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zvamaeoe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2oljpesrr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yobjqjlm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpnmgqf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kmmtfrhn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xvrthwxa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zxrmdbcn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kchcoivf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cncedjmq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rauqiovm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2amanbflt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kbosezsi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2blcypqvs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kiqgsewv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gpecznqy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twhwrmxk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kxqzgunh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zdpihmlj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2peyjwkrc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nsbbnwmr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lrcqfktv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cqaqwlmv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jndbqpha.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sevkfadb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yvcvgiwu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2uijuzode.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2elneswxb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wdyicbqp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2czyiilvp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bkpmgesc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2imuxxygo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mmvhmaeh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jlkbxajz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lzvtulqb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mauvefmj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tfbykphy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yabopjnl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yoithzzq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bobbegpj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2txdcrtfz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvpdeklw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpmziolo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2npfuwhov.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2imteijih.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qrykrqcn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfpehyfr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fbmysgdh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zjgqqfjm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ohiusgkg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qordpwva.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ondozpet.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bobwyyfb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2oenexzqs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwjamy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rbhndcmm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dtfnjacb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vtwkzqhl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hvayohpi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xqpaywhp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2deajamgl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2utwdukva.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bpwtyqby.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2emjvzerw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ltfblyos.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2whsuoapl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nngeyzhe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2myvqdcsz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ofrqdhpi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dbmujzyd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eeefhwql.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2esffjzvx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bramoluh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xhntajre.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2glyhcmgc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uyizsogo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2svljcuvh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kuxtoedz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgfisysf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xooapbsl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lusxehzc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2blqzsnyw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjnkpgoh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jmshtweo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sciimjqn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qdkmidqa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qtpdvszc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wfchpybd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jhpiwmoi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vsxabpba.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2liaveeqz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wmunfaiq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tmcthgyp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qogdrslg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2eidaumog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lustxvzv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hibhqlyh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bqeslcky.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lafhszji.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fjzuitwy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bbguwuzd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2inxplide.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yppkrhcd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nuosvuyp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vsutehcp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mxsklxli.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rsnuuuyv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2myrfklci.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uurhvume.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vtwfziwt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fozxvnxh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2apxootyr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cnyflovd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tvzffofy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2askxvyxu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wrjfczor.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gqxxvmnx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hvagrjdc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2azwaqvmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viuwqoxy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fwlqlmob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdklxlvn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jwqqflky.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ubymkngc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dtdykxfm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lewqezdl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2evzxuqgt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fubzvctj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bjveozzb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wmjvstdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptipbraw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mosgyloc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oaayzqpe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qgyyqstn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nkwqdgmc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugrpkgbw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uzfgspju.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rdsdjurw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hryinukz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svjjztmb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mcvuzioi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zpvoiftg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sxgoveyl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dbdeyjke.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ythtozed.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ezzmlxai.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lcaoqshi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mnttzfbd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iegntvum.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsqkrrhc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fsdselig.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hgyhjjay.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bigfyvnj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dwzysjjn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2woxpjmvl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fgdxeciz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvyumopu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvvhbvfk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2oeguzzco.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2luytzbjs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2arqhdhxp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfomguwz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dewqujtv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znekxgvx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2laxvwcvq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2aokhuuae.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uygzvjcw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bjhzrbnj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2oudstzqt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ikxizgah.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sikuonlt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2coejneho.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaayebh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2sckccqtt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2mzblwtjb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xxbskbki.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lpeahpff.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fykeukva.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2azehwdbf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2evfaoqay.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2frrcprlp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bqzklorz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rnwvojcv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2qokumxes.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nnaczooy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jybtxwdg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2adfgtgsf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2veekntty.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ctpivzwp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtilelz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kebodekb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2sbynaqgi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2egspgohm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xprcbevt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vgbazzpn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fqqiusri.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hgwihjtm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ehkptmlk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zaolhklp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvuifliv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xierwgnd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dteingso.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qerqpruw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2wjmkymwl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bfkmqjxd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gxcjmqnf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pvhpukdv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tjvhbgct.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zmkqypfe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2crsndjma.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2itjlntmg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ddvirqjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahiscnbh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xdkkaodh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxbzyeis.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2asyrohkp.html


<!-- 参考信息 -->