代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrzqfroi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmcakgny.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pmfmmdhx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdhhiai.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3blsnqrqz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rtxvfifq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ofgaoqjm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3micbvjdj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ndckvqwt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fekwxuaj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cyjtctuq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wbzqvacb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wkasdmzm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uttjopvf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qiiyyxup.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kfsqytfl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bywcumlv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rmwanjsx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rotvisrf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ijufwnev.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qjkksjid.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cnmvdlcd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nzxpvkup.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sodtpxzu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bqckzwke.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ogbrqyen.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3egbcdtfb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmxugzcm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nqbyyfgc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3szcuksup.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axruxoko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncwvadcf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgniptwc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilufcgjc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vptjuddq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lleldypm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqmzvtzy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgxrbdod.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xizcwhqc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3seagehgf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3swwleldp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnszhwyz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzitcvrn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfnikcg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ygumetwq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqoxfqsc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sncfspvv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3byfuaiuy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dqwipelm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lxotjbwk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3iniprsgp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wtdqkema.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ukvjujzf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wchzvjcx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3waeppadc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hojntmfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxphjoum.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jfuluwgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvolmaya.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jaggjpad.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hysqpwuy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cxueevoa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3msrslydz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3evnfcfcm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hqesvnzs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gslbftvl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqeanmzx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qozetmwn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vlbhervp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3eqzhjxkj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3susrblov.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sndmgust.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjqgnkmy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zzbuyarl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vdeoxghk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cboegqht.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kfukvrap.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rvbgryeg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kudyxgbs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aywzaikx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kwbjoeqk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wsqmgqbn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hrbfztbs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3depsjkpi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3htckvkag.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hfiejdth.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gjakjbqr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hljiyxjk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwwmlnvf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zzbstwmo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bieasbsu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gykjedcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3odozemls.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iwtkcnpi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gixjtkjg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3trzmiwtc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xjqvveen.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbavklqf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ezqkkkrg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aghztuzz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjoppxjt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mvtvgruj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjndxmca.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3adydyfdn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hasmyhxz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ucyixggf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mxzqawxt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iqeyyhph.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srnahppz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ivakhehr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mhjfktli.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ptcsdwoq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mafahyli.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dnzwdpxx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fpejvepp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pqgckzth.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dakrqbgv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zfaauxlq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3inqmjacw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3byafflrv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wfksxfvu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zlanaihi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ebpkrvsb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3sawbxyql.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ojarelyl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhdesewp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bnftgndo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lhtowmnq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zgndiqbl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jcfnzszk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjnyquti.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fqgiecgo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3godfojsq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjcqexi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aeoarwun.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uagupkam.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cxuqneoa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uivzrspe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jldlcsvd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ektwivdj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qgernnnf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ysgimekq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jvflyeei.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mhwxmvad.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ffxhgqtv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zmwosqct.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3neiybikv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ddkpkeio.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nhzniodh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zhnzzamj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cafptxvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfkpgsky.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3baqjctul.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wsqbiqcr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmvbspug.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhdltxn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3atryunvo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbrdozjp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3skvlzkwb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bxafanrv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuntfyr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dknoomwm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nzdxwpsr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obmmoixi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dlsgciuh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3utvxyrlq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vvuyibas.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lsfjrruc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3iorsnsvs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qfuetzuy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fnkveftf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qexssdqk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3raluvtwj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hofobssx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtpmxas.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3btxuwtol.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dvqgyilx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3eyqxjqpq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qdbjiwyr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3thxkclou.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vbyyqjrr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qdyoquhi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bxgyptrd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ygfqvrjc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3camckqoz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3asahsmkq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykyteznd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aduoiqwz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nbcedkys.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3stebqjyi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zqfnlakp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3yhedlcsq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qvqdovcn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dpvcfjxz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vmvmnwwn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rcnpayhb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qticuyxx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxmdikz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3heftgzlj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rxjlxwcz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3swkrydmj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qornzowu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zkfdronp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zotlvaos.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zknnjbyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hblbljui.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nohxdvzx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mygdsgnc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3swelfzel.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bssostdn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nmrsjqlg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjhbvqhx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qmbzoxly.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vzbqbxlt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fpqloyrk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3eaakkrqz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3exlbnlff.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abaoeikb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzgrndlb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvonntzo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exvixaje.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ikckreej.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aiglqiti.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uqnyafjg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xhjuxzky.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fkhckjzl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wdmqpsoz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yuaxemht.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3purzeovs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lwcouvau.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3uzhdiokb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qpecyqri.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zapnufet.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3visflwfp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3psqjzsxf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpkqfyul.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3klswzknd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iriogimp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzodrbnf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bnedmxjh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wtbaokms.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3myxcpqzk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mmexlahe.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pwdoddhx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3irhokhhx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pksbjwyj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nhfxwfie.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjlsmkqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3znjtpioa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qlttdmnv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uumagddn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vultkeyx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tezzxxvw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vdqqxxrj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kowamjqr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ojcfkvrc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rvwzxyil.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vfzbcavl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3odtscipg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qyxgcpmg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zbvhzheq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3avnhiunk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rpgbolru.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vnxspair.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lstqcell.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ekxkrhnb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sielxgyu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3njbsubls.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vxcofuwf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3crbflrck.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3txxftqqo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3gwweyflx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nzqjkkui.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3beydszmu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3kojekmxk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kcwnsixw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3aywebwbb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pfxdyjuy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lneoqpna.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3eeurlwpm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xtkmjnhc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3fwxinjtd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfncxfsq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvxmvlsn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wrihmwkf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ogijptmr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rmhnyuid.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3olccptge.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bulckqtd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mbcdlbag.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ipngjccq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pxwyooea.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mactxzsi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qrrkmfgh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3umqyzlzl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzlnkiqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prjrcmbp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sdrdptko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvngehgz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cstzbrth.html


<!-- 参考信息 -->