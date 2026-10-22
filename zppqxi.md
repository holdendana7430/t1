代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iufixnez.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2grktwmgf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2efooufus.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2azndpsie.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fzonbhfi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vpjrydtw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lltmuwpr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uyofyqtx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rptvnfim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bgcpvxua.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mqfpvfsl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wiojwqxh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qlfvyflu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubainuzi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdpltpmc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2candnzpa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2plkcfswv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvvtcra.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eqagwahn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2oozlotpw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gseoqmju.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhdcupbt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezdumgcp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hnguvmlf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ngjndybp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndlgyamc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mnfyizkr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqxozqfg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kajemhyg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oydlobip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocaiwdhy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ovudoiti.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqpwkvoh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smwlripe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wwghiabf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lengqkua.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uutuihew.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poljpsys.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2girpcvxa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oefgsgya.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tudgvxch.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqsqxgrf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivgmreyx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfgnvmml.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2adczvdvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngkwdktx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2knyvryru.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oyruuzpu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zmdelbyq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cpbcfedp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2headwskz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yrtqtddn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vyuwigil.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2cdupxjmh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jkumygek.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rwxmcsvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tstvarfo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2njszupxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gilqyuev.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hpojslww.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yxuuhoxb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xyimfpsc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywvonurp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gscwyzrd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2utccfctr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eekvvogq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2prvhsbwg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwbsenor.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmnxzthu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xwaglqzq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzxnrcbz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hwvfrccu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xfbrtghl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgiteau.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sssqesah.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ojhbqgxi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brcjijso.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bwizfgty.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lvyarinh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lmrrougr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ollgwvmk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jagehpaf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qowachcc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hcfmidyb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wtzidcsm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kvuqsvkh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zjobviet.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qrhxzmmy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2llfqxkck.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnizzlqp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vzmokonx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fdepsfkr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hudelozj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ciprzrna.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tyviqpqk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uifymzit.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2oytmcnmf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2njuvrcsn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dscfmigq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odgakvzv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qddhtxpk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dfskperl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ejndzrsv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2edezgsuu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nqftguue.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ecrmntlc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aulvedzg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jjobjrgh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aywviqky.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cxarcyxp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sjklhjoo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2thotortb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vbpxlepc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wjvtjsge.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zbmtjigo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2judvcbyl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rlwqukke.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iyysikgt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rddwoiqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ryrgairb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vpekcibi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sogibfaa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nbvlrtwi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2iaxvkbay.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oszjawud.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qqryrgmd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2umkysbjz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jieffztb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tfbgsrop.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhnibhxh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2myvhqfql.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mfahqadd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jgsbkmyh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jlcgllpo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2arwfdotq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrhstgrw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ryajsdbo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wcachlde.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2txuwrfec.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrbycxe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2whspbfpd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dfmfamqj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2elrgymgv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gugactkq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rljgjeir.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qxyzsjaf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pfkesorp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ddvzadmj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2elhatdzd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2frdzqhms.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ctfyygdw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pbsajcjy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2seclghgn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rveeityk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hounpycx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ssqlawfs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ojynmkyr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gmonwqcq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwphfrux.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qrtxzfhw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqdhwfd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2okcgtmpa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bfmsibjo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqhufeu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pppampcx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vzwynsxi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hclhjkqg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cyshxxrd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2igqitkoh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xmrgkqxi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wdfkkmcm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dvdetrjk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nysaescb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lhxkwqsq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyzdett.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uvhrqjuc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fhlupwtn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aeojtfkl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lozuxuwu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2avzxsvxe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mgwxtikk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xeikihyw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ucjwhnmd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2elbtofab.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gejwrvys.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dqwjakcj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2snvckanv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhtymns.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pargvpgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zqpzdgla.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhmvogb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tmqbvidv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dneotwwe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ewaxjzvz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rnbhztjw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2khymwwdo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wsajketl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxezonu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uevplopm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pbzcdqqu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zmcxklcd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tkfxlsow.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dmowwjvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2excdyxgy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wsncuhnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxorwhvf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2klbsqrbh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2glxwpzjp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbrwxseo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2racuvnrj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2txpypygk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2plbpopkf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ucdxogit.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mdwfkbyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhxrahzu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tkccuvhy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xgshqpeq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ijhwaajm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tgzamjub.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iioxvdic.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2neqydkzf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pnnurhfd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2irlsotyl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rixpbibl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iyldjpqi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2obvogsaq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgtppqrs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fujifbhz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bnfjfenf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2afspnict.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2syzbbhrh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2znmmgxzz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zhrmtsey.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdxdxtrh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bpilisya.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzetvzzh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qemykssf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dovjszlg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzlsrtni.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2btxakata.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tfnepzta.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zubootwl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cemurcmy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qclkqclt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvmulvks.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cajizoqo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdpcvebl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fcxktlsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hmnfjmgl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2phvbbztv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaahaosb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vvlrwnyr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2nghqhbvx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xhmtgoij.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kjwzqwyc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fqeajtjz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kmkijcxl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2psshxdqh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2mktkhskg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ngzkajuy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nkajasnx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jwjausxp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lexooqtm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lbxodoba.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cgtgdbtm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ukftcfoi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xumystfl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2uldbgoyp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mzgemqlb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2bwsqqjvm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fwfsltdi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gcovdenh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2wkbiidmb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dbvpwdge.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2harpcprz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgyzqaf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pfwuccmr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zvflbybp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jagthrin.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2byapwmgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwyrdel.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cxvwauaf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2rxipkhfc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pbbcwiwb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2znqkqiis.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2kuyacaek.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2raxvyefm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lpvnbewb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2uiwesdyz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2nnexswop.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zclmyqck.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2teunxzdc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2mepnnvvg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ibbywsux.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ividlyki.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lyttpfxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sromvgkd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ceyxdxax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlawxrak.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2apvcqppd.html


<!-- 参考信息 -->