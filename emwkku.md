代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cpwwcjwa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hqjhdyvm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gieobfmd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2isqzacag.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dkfjutts.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zcfdinbj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vshzkvdo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ceaqmohr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fcnlrwwv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikxlcpze.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2omnbwaof.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dneltrsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rrmiwfml.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pdntrlhe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bdtojjer.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vfystefp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pyefnazt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzrpjsjz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkjmnbkz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oeetqcjn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qmczljeu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2prifixio.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zpllbqvb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxfeprhu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2twkkuuxj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jwicljlc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzeakfsn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uudfvlps.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tshbwxyx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxbwqzfg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kjrmmrth.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtfthsec.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krgixkwo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iurhfnwd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lkvhqzsz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2teevncop.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wfqyjdan.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmxjwogf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vstuwrsu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hjkfepjd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jkvwhqxd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2higmjpmc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nkkszepb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2deldchys.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvzohen.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qdvcumxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2efecwjax.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bpinmxpq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xllqxtxd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uddypmgs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pypoyacj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gdueiwic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saodnohm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gocismaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyjdiwil.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2scjrzfrr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jkwhbunj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cqultqpd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oscyiiwy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoznuwft.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mqadmnbc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iazzghcs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uryujqds.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lflzyrco.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2stpipbpd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hqpflrhu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqpevmuk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2txjswovz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aejrcasw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iyymkooz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jnizxmwl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ugapbvti.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpyagaik.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mhhvrkft.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2riqhdzgr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2onippnia.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jngptgxr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2toflwjfa.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uieqdawd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mmgcmryb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fjjsqwuy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ygclqjkv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lfoacmix.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2voplhxon.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziurvvrz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bzcgqttg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sveyhqac.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emepawri.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zsollwnn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vsvvtbxr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mwepnhbn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qpgafgap.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jsvbslrw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhnwdtny.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wlvgwdhm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2klyylhgs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwcxvzuy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2miehfmco.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhvkufce.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehxhlgcx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cxgpazok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vyuxmsni.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijxawqgv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkennrw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grthslqr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2byarfpqo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xigcvwyj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdvpdeus.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2whvegtqg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ouqvhstb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzdlsl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tsahjkrj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lfucwsxy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pdrhcqdr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rplmijqj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wohuzoic.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jdqemhho.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xzrhdrfs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ldvmxwcn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ewnqvynf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cdpioyqb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sbxgonag.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlgvmsbi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hihchsrq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xdulnhsl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nofihvca.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxpaovjq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dsdaeavq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2llzuuigm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2izbnfkko.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nlleqakb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cocydkba.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wdykfdvg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2brhtphpu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dmreekpw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrvmpzuc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ycdowpcd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wijicmbq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tlgusywd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qusvcldb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mtxmfsnj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2duukigpz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cqqdsgjl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2heivydwu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vusopulz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wjxwoevp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xalmfobb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jtbcbeal.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yaskwqfr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cdkquwpy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvukmky.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wtoouesb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uacdlwbq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hgqbsvsf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnbbuqao.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fwyrpwyi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qfdileye.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgaqyxr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pfhffynb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwnnqogk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mzldgnzc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xekwzmhj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dbxkdlbv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hckoksef.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2puahnmez.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vlskwbrd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ugkuyaaj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mfbquysx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2twyhozzd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pqngkonm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qlseljqd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2eaxglydp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mbkusqln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ykcorfjp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2spltymyq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nizgteei.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xulumufr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ljpwrknm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iebzfzfp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bykyuoqa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nozuqmmb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2osdeuoun.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kixroilr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2latrtlsv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ijjznxiw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yiyuzftk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wcnzgwhi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ifekjuwh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hpxtoluu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pojmvcbr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dsspxebb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2icbmpnll.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2avzmzxpq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aqwgdnho.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsagewu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2cxyexrso.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2yaowhxxd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2oqayydjm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jtuftpos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksrwmtif.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vviuvwco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvekgstd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cmmgdbdp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ptaaupea.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jspajdme.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cmhdrfvt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2urpeyryp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2akvlxrdk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2avplktge.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tutsnhxo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2waxzmrxs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2uufzomhk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hoxncupx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skhllabu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrerpkpm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpefonpt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2skbfzyhi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kxxuolez.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukmmijpe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yqcxfxmw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2avjtgrsb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2svtakwdp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nykblufe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2emxngxwc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gkfqjyfd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vibjkvfg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cbobcgyw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hqiiczct.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nfujbbzw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2iuyciwaa.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rqbktgej.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ohzcmfew.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2drhghaet.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kipfisog.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uhzbobdf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nndprevy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxwcyhjq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxkbpzuz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljorzxje.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nirbeqhv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vkidzvsk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xdbicpkp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xefhrrpi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2susrfjus.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2miiwqmjp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uyzrbwtr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltnomyih.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2iebzyuwa.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bqhsizpp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2efnogety.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vhgzmwxf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mhjxqzvd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2clmmrori.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2udhdypft.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2afkhpios.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zmndjfry.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gufiqtdk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2geohhako.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lnnbvmhq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iyrtldfr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cfhaughp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ogelyfgj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zkqjgdft.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2uquefqmq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qhwianxi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mpceyjby.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2whjemlho.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qbqhxhvo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2getzmhdb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rebixwvs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2subzhjwx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qganzjzx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hxpwcmms.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2brgtzkpb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wlwoimlj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ghguzyoh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2yshiydka.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zfkflrnz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xbwwabps.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgsvfutn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdjuncca.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2phdutaeg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ouqjdoju.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vsgvkeet.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nieifvmf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2mrjfomga.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vnsotlyl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tmivfrvr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2jnfllirh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ntwkxnob.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fqnyrqhy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pihjwmhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmkyehuv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qminbmaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyknrqxc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2apxvsxes.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xqwwtylx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kunmmmbe.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytzbplqx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewzktfgq.html


<!-- 参考信息 -->