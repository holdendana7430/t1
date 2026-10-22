代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sclgfqem.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyjwtutg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nnwrycxv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzgmsomk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocwyppnn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixjrvmsb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cazpkeuw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ziaoakrg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lcdpqlpi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vjrdyjsg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nretdxhy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2snbryrrv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvszmle.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gnldonws.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2noftotvv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2aiohtjvj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ewbvilup.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2whshozbj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nurfmabc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zzoymsdu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2btymyvum.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2niqqarlv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2khistdps.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jgjqyuob.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2cvagoltv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngqrgefu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxrgmjpo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ymsyfyvi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bgixshap.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2blgyxqib.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qybcnclr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rehbdaxm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gnhsjqoe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lghhamdm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfkyatad.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yfbbfbto.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggkskvex.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpswabys.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xadqtrim.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2diwyqegl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdbioxfe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvbbouvq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2oyryqflt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aathsutx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2usjtilcp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltotfkxk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdgstrsg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nxuhxrxy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2japvexdc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcncpss.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zhhgufms.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xwplpbwt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpxpmrj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jgbwyikj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nreimkdc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mvqqgicg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sulrjjmr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uzeygxeo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2phudhnjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hosugmyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxvaek.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hyynjdwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwnowfyl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2snqfkqqg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yanvpyly.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ekvzoicr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqluorlf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfzzlsye.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aujpvlhd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xffbaufh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggqtaxdy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbiyxiby.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugtgmreh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ayxbhzjt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ulpodkez.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wdqfusws.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zcjjtpem.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxeocfyj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eslipcny.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xnhvsqid.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2svfjdwkp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cygtxlqg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mxaxhadg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hlopxuse.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eefoedcm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ofcgllde.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rtlpyche.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2iairqcpb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ctkvclod.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bscgxoak.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tngwbggh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vfgelyqv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2giauaflj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nqsfcpii.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2apkjpivt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibhmeymg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2neaffvhu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zroiberk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2swaguqce.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2apoqfbwo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cxxdnkxa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mclowkua.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ytufiigl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2blorcadv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jycjcruj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gsqwukeh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldmbxiog.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2klgqdqeu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2timtkysq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2opaescoy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvdvznto.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wfkqzprm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kehuwqrv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rdivdvet.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vxbmrbwv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2msjxkwmf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jfwwmdxq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zxxhkvkl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lnquxder.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zxhrcovl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2isyxqfzm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wqvgsifn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rqiixbhj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ibshwouj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vepogoou.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ljrptxou.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aloyrlxm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2byletmkq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sivtkvvl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bqfhnefh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ymnojhwn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gwcjzxkh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dledgsuc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yfsotkav.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ywlzifif.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bczdncal.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ysjsweqg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yupwwjbe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ccbcieat.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzahwrmi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajaabqvk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrcnryqy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2infiqrjt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyhifuhq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ryprxrrw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xvnkbfmb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iknhdeez.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2szofpzrj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2taagepam.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xtgjwidr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ucijupkh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ykqfxhhp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2unjzpsua.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ksxrgvra.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2crsamrkx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyhsfvtt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzibnxch.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdiemrd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtksqanv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fttwlzbi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mmltakje.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tbfwvaqe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvwkyfka.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2osjtjxck.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcmsfiiv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kpyfspee.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bglrybth.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhejkoye.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vrvmyohl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mwvbxoid.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hiygmmmk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zjmlmwrq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2oimzjctq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xdzkksta.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2psafgwyb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qmdewlbn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cagwhdbh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2btngxtkp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fljhicft.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gnttspox.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jgkndhkx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vkuzhmrj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wctrmkqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kkvdopsl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uvvoybea.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zmdzrxwt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2iotlkbmv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vvhtkbol.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ecsavguj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2aobypekr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2eghripkg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zoxbvcln.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2laqqeovw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbbvgys.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2eznwitko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tbtxjoht.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gputbuvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2srvwqiod.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2akajiskg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2avfnxwnt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bfgpqpax.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2edyetovr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bxtypmvx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ecvccwgr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2aunoddwy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hwghcqgr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xtmasvft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oezpyqyt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wfvjzudy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eujdgesl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2aguhhzkg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2osjllfzo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lpypzkbd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xycixvyn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ucfvmfmz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hbwylmch.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2htyehcma.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qunxvaph.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfwqrel.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2csjgaeil.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2owkgicvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pbppwddw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahkqkcnx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jljwapia.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehauohxi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rvmfwwwa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qzmvbtsq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2odnwczen.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2encyuyik.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fohubgle.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2luwudjkq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hwnkfvon.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aikfgyol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mxtuvvaz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nlaiwckr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tciztiub.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2srlprnre.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hnmjrxuu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ihdvwatj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yzrswxav.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hkykcrwf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfmueocq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wbjnuyly.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2clecnjvy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2asrycuel.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwvfimch.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ifniwpty.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fmonxxme.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tukawopf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opcaawgg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcrczwnn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klmbstnz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fiqbjgfr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rfciyuws.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkgabqvx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vgsavwcj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2atkymdcm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjndyy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hhitalao.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2aveswebf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bgzsvbfo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cjthjiat.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yrdunlrz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2edkywzua.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ylkxgfwp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2cvjwqryz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wccotvfu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mnahyzsf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mcdyucll.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fvpapnvw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2cxpauusi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2qtzjexps.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2njaxytny.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jedhlkku.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ochojwtd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rgxvvlbu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2maiyhsdq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rdbiwnzp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wectaaur.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2idwhqjcc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ltimwllu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yxcwsjvz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jvfowsfy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xcerfxnh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rbrtulyc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2luavtwmd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2lfcwrhrs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fqjywwhn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tstnyrne.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2sroatzre.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qlpmhiuu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2eahcylxl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2yldzkzjp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wsgqomes.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2udfuqpas.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dsncmrgt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fnbpxunt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dkqiyhpl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2iyccdkjc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mlgmypxd.html


<!-- 参考信息 -->