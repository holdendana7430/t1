代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwhajktn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qlqcxgll.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezsaftyg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2okacdvqf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhsagwpg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckxmhimi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uuunjitt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2teyozhun.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2soubmiay.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tnmknuje.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gscaliqe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcxjcwv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2imdjefwr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ttwcjhjr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rfcvpfim.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rrtoyhna.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vobyixzh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vinayfct.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wgxccfgj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2chyykcti.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kibxitbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jduowimx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2aabocjdu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ldradofx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2phshduti.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2oanxllwm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lgfbeley.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yvplgrsj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fxwegmzx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyeoypug.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwowdfva.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xckvrvnp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dfzzvdys.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lyvtmyxj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2epwwohxn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mptjiwfn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uirrxcek.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lfjmihxi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2diwodzzp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxfnlytb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ceocjcgc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eodkudvl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eituveni.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdansfve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojsufjdq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cywtjhfi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ygqhknie.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdneyiri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zxzkhbnd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hiavgqra.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqoxxqum.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2izzvkcpc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pikvjpop.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewqphxyp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hdvdphdd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jgxjohla.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ogwtdddq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qvvnquje.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kuyvceex.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xewkkptf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2oegmbxng.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jpofbgzm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2flcftjly.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2txfyuazs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybaxvjlg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zmkmhebw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyhkxclk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sczuptnj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ldcpugdk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsxgmaep.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2meqisxwn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2juztecig.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qnnotian.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rpwgexel.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rxwswshk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gfrkhkwz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2evdgkesz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hsbdxwqo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czwszjug.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhfbmexl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nmodfysa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmyfsxdq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dxmebexj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qwmmeqrk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ielgxmli.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kacahxmc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fxtzcffl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iqprmcte.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ljvmsluu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hmsqnwmh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2znydsuwo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pizdxdcb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uixxxqrj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2txfcpcfn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pelbgviq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mokzlwoj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsnzgasg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ifynsyfe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rlxxanxj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pucblnvh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aohtzhki.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jukupnhk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lemdkcpw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zshcgosx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2plmjhekc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eesufaza.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hcrafkvp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsaeisud.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixmfdrqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zkmtevxf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzzrmrex.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gyctwokv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lhepukdl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hycsrkhk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kvdlmdow.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpyxdach.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbqafmav.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzqfades.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2aqkuvecu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydyrszay.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wgrhqkqj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cldxzgsn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2aaqrdviu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vlbugnwr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vtotqgqg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2piciywba.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2srvddiys.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wbyjlroz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yqzgjrbi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xkluebcl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pgpfixaw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jkbahldr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ghayrltn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzwtyknm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2daiebxvy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2daknwscf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lgabovkw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mybhbnbl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2icsfoddt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jyefaisb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ctwndvbv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rnquaerz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gtqjnjui.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zinlfdzf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rwqjcqyv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xbhawxhl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mvanxwmf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ziuqwqbh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vzzybact.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2czstyduv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cjhsrxjq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ukaivvou.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2szgxyiss.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2owxmnzrz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jswaevzj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2veysjiee.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ncrznptn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xnrkwxvy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kmiupxhv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fzybpixf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ljryltgc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gahjaytn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zrpuqbqu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ohpgsbia.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lcgrgwqn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2eudzpcmy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsnzcnil.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lwpymuwy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pqsghnft.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ndxpuitl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pwautfkw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2siwfprwd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nyldhaey.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lqjvpitj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjcodsxp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jvfavvfa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fdkbwwwp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2drcxxhke.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hraepeis.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ieobqkpi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zfkttgnj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dymlzeab.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dqvvgoea.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vqgnlpda.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xssrisds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gtkkemlb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hffhrhhy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2phkpqncx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2shqpkcxp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzgkryjh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bhvnegpg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zlpoivzu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pjgmwiyd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dcnrsgqr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nikijoux.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhcfpqdw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2iewgkixv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsfcgq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2glzqxngw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vnennhwt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zzmuhfpj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hettnare.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ztjuqyjw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dkwkawlh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xzdkuxrz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wjtguirn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mzldxguz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2iiqgocdc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cyqgeojy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jjfiucbk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pjahrwow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duyrzsdo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qdwsxndn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmklbavj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pqzurwpr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ytlvsjbs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iozuhunr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dggpdtrc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhmnda.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfuuezhj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2syyiaogr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jedecghn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcdarnix.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2shlpmgqq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kleppdfo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ndgppuce.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpnpepcs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cjihpqte.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cbjmcbwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2szjyprsi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2flqydyrg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhclwgyn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bqorxmgh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nvaxqtzw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2scndpzlv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yepikysm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lsapctdj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jockdhfq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zcekyegc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dlxpkvbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gdtsccnk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzhrgyia.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2laxltlws.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nnpsnnmz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgepxhxj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rhvloagc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nfghjwij.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cntfqbay.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ulxqictz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfyqjtbm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mvsxndgr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ahpndqpo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2peuxmpyb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwgbahgw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dksoamiw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwleflxv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ehlkfiuc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lmpmszkw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmojaost.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kcxgfmcv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hwacsvro.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2afpnsuhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ieoigrxf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ajmgktkw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hgyqmrfm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pphxjjpi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2njtpgvmi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jbdqtnhi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kqtxsjci.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2joqzswmn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2khbclyrn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ixrdycsa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2joylqwor.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2sasdwtwk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tvkictko.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ewfgahal.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fahnqrne.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nfygikpf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tjyfglsc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2omvnkboe.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2igajlmqj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2uwrryscx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2cjhiyjsw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ovftbfca.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fqxhjtoe.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2asxqhyxa.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2stzztdhw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ztazebat.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2alyunhwa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jmzpvbnz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fbpstqvt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fwndtzkr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sqqlynvn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ypseszaq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ffulbcfw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zjjtyogp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xliafhof.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2njgxarbs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dkboejjp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kincrfym.html


<!-- 参考信息 -->