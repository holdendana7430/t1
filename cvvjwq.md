代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzriowxp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeuylexl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rrqlbprg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iteujpdw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbfmuxdg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tkjgkner.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bybgzotg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zqxdpmge.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tvlepxnl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iuiwedhg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2irxbobvc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eqxidhdm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2awloomfq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2puznkvsp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dwaoifzv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2esbrhkzh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rgwlzdyj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqqyiij.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bkfhxddb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cednhzfb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bgqvocla.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qucebiml.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bcdsyagz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ykdiaguf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2apfnxatz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqfynslr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vibkkhaw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ylfxjznx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mszxfyvx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mwbxjigd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jswdsnaw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfvftdxi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nralhpfq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2astryqxo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxucvysi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kgdcpxcz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upxesvsv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hggyfflw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pnhxyuip.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqfgsbmj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbcqbnat.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umkybhow.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sdgcmbmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcnrxuyz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jvxcjsxu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejlelvqq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2exbnkztk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2efxjvazx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uxkhjute.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2htfjptct.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oxztspog.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ilnglukx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rmazenli.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ozknpfcg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uadexqkf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hieixzzt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2annhpvqz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hbopagxy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kqvlomyu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xlefitxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daoqngev.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2uppgxids.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2malhucdy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wgcvlvss.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xugbznyu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2doenlawv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2swajeniy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdfmiad.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkkvmxdr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ndkfwwvp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zgtexbqd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vbgeuvnr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugcxwpyw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wpqysazx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gdrzhvxg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ifwxgvjc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kbalqulv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwptlzip.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ibomhvfx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xkweklhn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aethfijr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xczerjem.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jepahgti.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bmvztrhu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qgfjdxah.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gbhiovjp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2orgtlffe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rmxmfhzv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ddzwdqbg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ckewdpbf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lqsdrhol.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2crgtitqf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lhnztcin.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2utywjrpf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xutucoxp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghjapoka.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ltbofkhd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2umbtmvsk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mrwwjkhm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kshluicq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vbblkfnq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gvecutha.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yxscphoo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2psykxsep.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2itolmldl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ijschdrf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kndqqesf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vttstnar.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kqbdxule.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rfrdwkjm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pfzmvhbj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pngftfzp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2puexujfv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nioirrrg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fovdwldh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2krmvrvdl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wyophnht.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xyttcdov.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jwjnwnxa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mcordelm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qxhvbihy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zgkfbgva.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ajqhfjmj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ujtzoekm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2eiufqccc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rorarwfl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ygcvegrp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vteaqcky.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vjjmbvnl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uyytduyl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2eektgabq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jduwdlqj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iwtizjxg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlhwdgpl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pptfcbwf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2uftbufcg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2iyyhzttk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdapqsd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rdnxutbl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikatlhao.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uvfxnnmm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iekovhzl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2oyghqyqm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ushpwqec.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2noqcmxud.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lzijnxtv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ptxiaebv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vuawubqt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2runvqogk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ddrjhiso.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2taxtjydj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cagpbtfc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2boyyukra.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ivzscpyo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qfajeyqf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rpzywzid.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knouqibl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qklgyeva.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xocczptg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vmgvqbgf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xykgitas.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cevoshxu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2iwjlvwrg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pupvngen.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ecfenuqv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jndxjjma.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gmiazmsn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkavqtge.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kaqotxdx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jsrehyww.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zljthcjg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xnlrtbgb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yopsygwd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zhqsjacp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kjwixxhl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2avncoruj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uedpzfjf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zngvzpmg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2amzodvzu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2aptzpgjd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2etlwcbtd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ifmwsgao.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ryjqhakn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zsaqfell.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wzwtqukh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aibljadh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yrwzfujm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rcmzysqr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qgnaaijd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cxpyrvhk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdrjgsob.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prhzvgub.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ihwosxus.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fhvqfazw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tdldnyqi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhkhdwc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2brgfbptg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kwerjnwn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2augxglyh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2doqlgkjp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cefokufl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrufduej.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qwcdvgpm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tjpfihnq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2acpoxolz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nhmwbkcb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ijjjeind.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erpspzmz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ansdskpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceflalqy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xmudbjib.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pmkzksnc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrcktndv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2segfncyy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtkunfdt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rbibklxy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tuwdprpp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rdnkhwdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcxoycni.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bbzmhusw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2llxrncrw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlmoanwh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oluqlyti.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pycilrhi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ixlumrei.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hceiprht.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2advgawnb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fzswmkqb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rysaoeop.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jgknuzen.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mfxrascd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aupecqfd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2halclpou.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gonkxjwc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ewphzpgp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pisachuo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dbfrmipu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2txcaxaua.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zjoeribx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddctlzmb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdccygay.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqzmrved.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xlaqidmq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2skgidchp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhlrfovw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfxoxxbf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kqsvugvd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2samszfbx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2oyqgswhe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeyqstyn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfuggeag.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2werqphib.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wpojsola.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jsqqmjnp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctsdxmji.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nuhizmir.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dfieevqf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rzrbmrip.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xbgzmhmi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2widebnnh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lfqowwcn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2urdbuima.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjbltnt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ikeifnzl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dnctlzcb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2drmlfnei.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wcmelfld.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffaxzynp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rnjrvjmi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2phuqxwrt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nbjhigwc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ciwrzlnz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sqopckzf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zuixzevc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ttcdrbht.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bxgpsmtf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mzkmpvlr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2bvrftltt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hzhzstpe.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gyhfkzki.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2msllyppw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2lcaqdxso.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xtiopzgk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2dqogbyxj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rfyhnzbd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pwchkhqb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvagcujt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2icwsvzeo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hwxcwwht.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2fgfdgert.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2olfblhya.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hrpiwxoo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pfljsatt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2izqmptsg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ueuqomkh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uvpqeemq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2uqwplryz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2jfqhgkhf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjjzucp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gpwoawqe.html


<!-- 参考信息 -->