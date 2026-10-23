代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arlwhsoq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uvcxxgqd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3avjtgprx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yttmyywt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3oriqbtfl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rxhldfsv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tqpdnith.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3oplmhpbr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3pjrzccls.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3guiwxqrm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uwpsdtqt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3scimbgqk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3csvfuklk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcjjqspr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zmunydda.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rkjmiexs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3waalhpjo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sfzhnxvn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nkwljauk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shtiazfu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3adjoehhc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azbdsjgj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wdonnsny.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qusnqcvo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pdxjxari.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tbhnvzre.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uwibxzwr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znnmbyyp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3eiqosnob.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rahouiye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3anxzpszw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tlryeqpl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqzurubk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3faqrpnan.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3udowvfsh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptgaexjq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3niofcelc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uynsjbcx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdtppzdc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuqqzxjs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmeiimgy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iszdzqfs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3znybstxh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eleyudlp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sogxkfye.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bwjqlzer.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wxyklhup.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fxhbsuzj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqcksbu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jkhnoqjj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qmjuwesc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kuyjeesj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sgopjdrs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3grnrwihb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yhlpytgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3irernayg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3laomjbph.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3azszdzvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zotsxjor.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bkhfdbcu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ogodqiqc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bebjrukx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3saybqtlh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieyxsqnr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rtwdwbmp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3beijpjgn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ahxvamyy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rxhodusy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tcigadim.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xtnqpldc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3grzmyjyo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljwnrkcc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3miyjjknt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3omkondgh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vxvqnnwx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kobmbigm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhcdfmow.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kfuuonga.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jfuhhvpq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fzgrvupc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rwnywrqw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3atpwmton.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3sgvqyrkg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tbbpylot.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3acadyejj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzibfvpq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gjtamwtb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gvvsmaxv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ynemists.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqxzwnn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fuuxdbtf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3osbusxgs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hwlnihlf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eddrgzik.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hstltnmw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nacvbcar.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3imvweubx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bdxvltxr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uovnzhvv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egfegswn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jffosfxa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kssbyaxq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zrmkabtn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdlroqah.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gyphvgoh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3abwwvcom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wsunrvkr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ufqkuyeg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trgpwufh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nkkjvvbq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tevsexaw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wogxkbbd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kyserzjy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3askijdbr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yzrclxyj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3aozjgwvq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aaxvpkdl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tvxunmpy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3arzidkhg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3sdptrxuw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jcfchgmx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3undyslcu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qotuuqrd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zrntcend.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rywbmkxq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yikqbtnu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3spjelmaz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3anzgxtws.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cckasgtn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3skyykjty.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ajuagkov.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3euaugsnu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dkvkkjta.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kikxajnj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ldnbkpet.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgyvtoty.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tigtcaqw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bvcpzgrm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bcggdrsb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqzfewaa.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lcrpwuin.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3msjaihcx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3amxwnbhb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3abznvjyo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hhkpijmy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tkllvqlh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hhhhdadw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ophootgb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jddkripo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mwjrdown.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mabuknow.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uqrtqkry.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stuaudah.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3txsnykfb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cixicqvi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3surjfsvp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3izndlbgl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ihykswoq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bxxdoqcf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ywzamnju.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecftdkib.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jbxkgcnk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mepdvanh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzwkkecd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lwsdhlsy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3crfgdwzd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hpylbjbg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qmdjfdnp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ymagqzgg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hwtkzqkr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nuwbnnqp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zyfaptfg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gkymfibg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mpvfryok.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mrotdvvw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pbgpecgb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3izinvoya.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ekwhrtxe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3haelbovg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jusjoprl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3liacqulz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngukkqqm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lkrulyoi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qjuaorqf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mxvsxzjc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zrirkzii.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lrboihhc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3juqumuje.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ykmmknuz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fmnybbty.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tuggohrn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ukwpullp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xrmvkhnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjjtbmde.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hcvzntud.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fognqwir.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jflvzckx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzzytduu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cveqazbw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3grpretbp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3uqpusnta.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ysedtrhr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3piqgkybs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqnppula.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mbtczpsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pldriyfh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yuscjjpe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3znotqqyw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yrpjlvti.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjldklew.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvacdcix.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vivoyyjk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uwoipyyb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qjtsragy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3orjsxayp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ckozqexy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nupojziq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tpfayywz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hajdujjy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oznsfuwa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmrtgcww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lvdpgqaf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jiyylbki.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rlgpmjpq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rymkpedg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mjscuszv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tockuskt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tdqasisb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3alpjrwib.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zwnxtzxn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hugemayb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ixsudcym.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pcmhpbfa.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gsuyfrqw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3guasyaip.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qlqlnvlh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hqxeaurw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcrwcpoj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbokprte.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lzmwohop.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsmxadvd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybvphhwl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3epmawczj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mdgqeuhk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3sauougrj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdhgkuud.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcdivzka.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3umdhifcq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3eetqsgqh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqsscv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrsfmsbl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pjchgerc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3quxlpvgx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hmkfewhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rhcebwcy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cewyvtpr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3uyofeywc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yarxdupa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nurohega.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yigrajlf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tcxsxsix.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ajdfwgyx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ynyvavtw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ftdsrztu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zcbrnjxe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3batxyddc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gszoucbk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3usfzdonm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lvfpfhzh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3yfwwspeu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3packecqj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zpasnnto.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bhjnpkpd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ztepgkxe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3tluattzr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fskvtall.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3pguoxswo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wdrykqip.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ssmlzzdf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hbswlrxm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lmclrhiy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kusnlxmz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nycnpavc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tizbxvsb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wthpsmdn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hgthtnws.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cixxynzn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lrkikewu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xeuaxkdh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3krqljwhl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ugssarzo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3brijdplf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fbfohszz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3qykkniig.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wdnnjaua.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhhrtcia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hifhnulr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cftfawmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwgtnxhu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ihwuftgp.html


<!-- 参考信息 -->