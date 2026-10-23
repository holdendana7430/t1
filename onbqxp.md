代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzyntwun.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zeirtfoq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klcrffcj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bqaudnkv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxheengj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lvylbqed.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqrvxxrh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxrkggow.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvpjtbib.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fhwvwxkc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xfhtdouw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3feiaagwh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3inkoshbr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3neltjwjv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wtrgcvvx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vbswyime.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3aoimxkgm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vfiswbdo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mswthrml.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnyaov.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3akgjqhcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rmzbitqf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3isanaywu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mvjjktig.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lxduocfi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sjzbyhlh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3klovgajj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3utltjjwh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ffokauff.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjqzwacn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hkneeivg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bxlmcjwu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jyyqyqcn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjsqesbp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wrybyhjv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlfmotcd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hcjdkccu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3eoaqfahr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owonwzif.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3diiwrvfw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omoaxrqw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nukvnelq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3erjocqwh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmeigoxx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkqizywk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydccqymi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3znvrgapl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrfjid.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ruzlptsd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foaqrnzl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qryjkthm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bzmwyfln.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jbpsfbji.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iujszxzs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wfwkqjam.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kolupaiy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbbknng.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jxngbord.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mysxdbaf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ydvhrnhw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gehomglh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3swxmtvfl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3icfpzsbg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tcubbeeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkkzldfu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lzscbktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwyivxan.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3acrnwlhu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3udjbntxn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xmpshdwd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3euwimbct.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3twwwwjxt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3byeanimk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tkursbyc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3szzskatk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebyokoap.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vxkjfmaa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3elbypusr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nreyjocs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bslgjkcq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uhnvakel.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dkxexgvx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zqecovtz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3weigjqzm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qgtqlgbu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3sipzeavv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fzepmbya.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lhdaxtbc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pzliddqk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3neqwtfuq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wbuvtmfu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hjjvgsny.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3erzndeiq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vjishwtq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hbwxviur.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qvsllzhy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qswyimyx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbqsxhqf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3glwdaopy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srjsmess.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uborcdht.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ayxuksdy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ixqcwkuj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3giybrvrp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jhqfjpuw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezglkdwo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivqfvqjb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzotvlyn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3idvzuill.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fysqszio.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hbuluffd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fdebzedg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3isecjgkg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lhiufrne.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ecsekacm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qurdpgmf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3juojgbcp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3snfngzmj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3elmmpjhn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifqonmwz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qragswdg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wquorvfr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kriapebu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hsbfmxqv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sirbxeiw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tssxiumz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3edgocigy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ioqbzarj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wskbtmna.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tikfqnhq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qqrkkceu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dmstbbqw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgxvbgat.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlreswwn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dxrcbksv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3glkiaivb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ccjlbzar.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fpinlcjt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qnitlgdo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vbfnxxed.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hmztvmax.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3azjssqls.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3edrvwkvk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zwkrmwxq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3iigxmoqm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ifbzsvrs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bhvrimxp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3umkokzix.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3szlzsijg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ecbrzaie.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ahgvdvma.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3elywluem.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wkqcwidv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hevpbuus.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xtwnuhpo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tcgvyynd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tayfaauu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wpepycsv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lizpqhmb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ryllsavb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qnepeyzi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmmtalfh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmxcbebw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qhebdiyk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ofztgtte.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fizoyzvh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgafrdua.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xrxqvofm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hlmjrcwx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpgzhdbz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ianaadrl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rmemofuw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjqeqgq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wlfphnta.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3twmbkblg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fvrtjfov.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fmutzjvf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bpilmqjs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vrqvdhcc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vixcazng.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lsgbgmzi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3srlqhamn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kiwzzjmu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3adexgdjw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xjxfknls.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3anejjgnh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dcgkesur.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3usfedkjf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kcfnvqik.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyuqbzda.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dhdlhvnl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ajlchsui.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hsgrvpzx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cwjtqkpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3efnriike.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3snwaipzu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qcrgxvvn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uavgmlif.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fqevqket.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqsmlre.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3irobrazl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wcnoweea.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wjowxmxz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zwuonkbb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jbnbrnnb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nbepzrsr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wzkixzte.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3brmoewwr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tykutdbc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cllhyyay.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lbvnxvzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvimmmqe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ngdrpjvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sduejrll.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sfuqbfdm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvmmbrc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3txyqmfoa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kvaupwae.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bbzukbja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xrlhsesz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ikusfctn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tymvedek.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcwwonhn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ukyitcrg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3upzmqizk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3toqxsjgh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpokssrg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ucxcxjdh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3osyvunpu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3yrsqfxge.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hwyubbpv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evrnmsxj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wftfctoz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mpwfpvcy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rxjfbbah.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bqkywins.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3deyhvluk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ewzxkzjf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wnuogtsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ulyhgkcw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpzwhxjb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbloygqx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wspmubxb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sosdiogv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ifmjxoeq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnxjbzho.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wdwrodst.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3mgbvsgds.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgtojsbl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdrcncuq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gzewzdnr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3subuxkyf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxgkaogr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ivujkqdl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zxmvijip.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jrxzueqq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sobyqznm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ffogvqcl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwaqaeyy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cpyhveft.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ltgemgdq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3npaesnvc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tzccohlr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wyblgsrm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tooovewn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3frjojinp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hxzoholl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jeixgiwq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xfqxuolr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ndhtxvsm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ipxafaqg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zrrnsmhp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3joxcvsdp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mzslpgrb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dnetpdkl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mruvwagg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fmgitqhy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3tsjhsuqf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mgehfaez.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xosfdtzq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xwondxln.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jifzxvzl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3kocfgteu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fvyrtuce.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dfprwxll.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3sgucausg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dcowfzcb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fjlyfrwy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vxctadtl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lojnbenl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wmryinwz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhiimtlc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wuvjtiab.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mykczhwu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffxqnvny.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fbmrvxrd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3htpwbfwl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bbgeqafx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3feadskru.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3khhcpvhz.html


<!-- 参考信息 -->