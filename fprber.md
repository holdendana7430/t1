代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekndmook.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ynjpombe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pljoomtd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyjwwwqf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yditkzsu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cmmobdxq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmaknnof.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rtsajrmv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcwwkxrr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqgtrflm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sazclcys.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhaocjpk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkacewqm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pcrnbvfh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3myvsjmwb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yfvjognc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3robqryca.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3umqhpxxt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ftighwrx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vczavnzi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3owtpsgyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kegwqlov.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dxlwwfpo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ehainflm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ryyiijoe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vbfnlyux.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fwyixbsp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jycztktp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmdrujc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qzvzcbrp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cuukxnuk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zoyghpcm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jdjuamgq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3llpfgtdm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yshotdqu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bmqozcbc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ghenbfet.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ntsnumjj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vcegvdsg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyfyhgre.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3slbfhopm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3voffmhsm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzlsjzld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qvqqafsm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3laonnbon.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxizvzad.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lgbsloli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvywdzfa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckoakudl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekvnqbtz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xqkqmxam.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snsdjpxw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3vmdrdykt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvkktgqf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlbysjag.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3puqymyib.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dhutlstf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzrmjqtv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qkrgnrov.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yiqhcaas.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bnrkxwjj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nspeeufx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qiobmbvx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vzjgfkpc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3aeozuosy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nyqfkrgv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vllcwvxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3oiejgobp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkeyfmge.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3meobgifp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttdonvob.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yxemxkag.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dhbbewzj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zpsfqbpl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jifuvhwl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pxwghdam.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnbntelt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qtrolvam.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rkectzhf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3posfqbyh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sfznlasi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vrqpjped.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbqnkrhc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhunlpd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3furpzghi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyoukodk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tttzrjqh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yxzpxerf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nmthjlbz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tfvqlvjr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qetyxtab.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uvztuhel.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mdkniaji.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rwlnkcqv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3sbskvahj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uikwkegc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lxtkxcax.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3toxvcjlp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ndstljmr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mluhniao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3friwkivf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tipbhqkv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uulwzhfd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvyffoyi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zbawdpjm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hyjrmscn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3blzfymvi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3stqhnmlf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3aqbpzawv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3opmzjyrb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xieqkshc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wielwibi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wivsdqfm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3itnqsdkw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lvaqfcit.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsyxndbi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3awuzzgrf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jwqmwjkn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abislsvg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfseuzxo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kexvnoje.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3slnnoxwd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rurzzsht.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mmrhrwyo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xqemtwtz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uqihdikr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ihaqxibk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hchebyzo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mjxmcqzl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qwwueiby.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mxiiitym.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3adqbonup.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zdefnlip.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bmlrzqwd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gexigiap.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mcczxrdq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3knljmkih.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pqwjnxhs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vsaulilq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bhaqruxe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fhfiosgl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxavdzzd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3spxabkxw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xvrmmpzv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ffcxamvs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3uevupwhz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bsingjam.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3byvinruz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsqhmeog.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zoaosxso.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uplcyksd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tnmctumk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3myihqazr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vfzmhazp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mmuyzlpf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3oastxrky.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uztcrbny.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3afevgezf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3udyhwdab.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gcibthqm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zsgbqsdf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cplqaoau.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tljhhtno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxqpvou.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3shaddpqi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yhandajt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fenuckoz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kcsoznkk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qnponzeh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3iivymule.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qjjfevlt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3towtctun.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3muwbodgf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cvavrepp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhzdvkfi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itdwzywv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vqysmtdp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pghiyzbn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzoamaag.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gmfmgjua.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mokoayxh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nwzemisl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tqrfuyrz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xsvxckaa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jouzllwk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hrspcuhj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3scpxqklr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hfdzcfjx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ynssddse.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ecrbsqin.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jmbhbiyz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hvjrkxxi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rhxblckw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eidziyyw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3akqbigzy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gyqcgdkl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3benkhcau.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gmgyndtf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bidpeiyg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nuasblly.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3peihqrne.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mlhjrbxu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fsstldpv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yplvyjvo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ahlscjkz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tejnmdbb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3olgornjj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wivfwjqs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3giqajznm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcqpvaeo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nkefxdde.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xcfzaigr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3exadwhjg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ahtfxxwo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cxkabvla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddmxtltd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3edfmomlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttwzlpcl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kpgmyqsj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bpsnhxpl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ghduripn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3chpaokyt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbedvyo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ykezcfce.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yolnsuih.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wtpxsxwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjzppauk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3anmmgnla.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zhmiciao.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dlawfqyq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wjxkgjsz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3emewwzlq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3holbusru.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ugdfaipa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lhvixafs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vvqyuiom.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zljtquiq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nspmflxi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mssczdqw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qmmwcwta.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3itydjqzm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xiegdeyo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tencfghp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3eflaqaxr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dvuloclg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vrnkamia.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3urnipgpv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pfenodri.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pkjqipos.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3entlsich.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofjqoxiy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbsaul.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3thbsvvuz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kusmdzun.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqejyxjs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3roahfxhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ozumqkxq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ypfgvgwk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wrafrfoj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqrdjiaf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cpvmkpph.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rxflhwyh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3nofpsxwj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rcyyjhgv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nczslzuw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3efptawyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3monpvezv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pppehpza.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bpfmninw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kdobioit.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsuqoky.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3afslwcxy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3twcdamsl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3whmarxra.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vojcbxvc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eobobheg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vbelnitd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zifysern.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lzxqhxow.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hdmkxfqp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jbyjhpch.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fsxbhnnc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ykjfebmm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wxlqetyd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3fkskvhdt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3izkomrwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wonnxvfr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3eupyocgd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kurkiuzm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3bbrxmidf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hlwtfrcb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3spdxkkgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lyernztt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cjzhmkdu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jbbhqmih.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ycgjcuvu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xpsjqbyo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3spoohxrq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3brkqhvem.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3itfprzfm.html


<!-- 参考信息 -->