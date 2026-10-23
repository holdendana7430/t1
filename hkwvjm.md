代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fiyhoypf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xiqwilrj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3njcecmft.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3imylcbej.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oyqkotvv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xnpbcexs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ttzbawpo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iojjbusy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yojfbttw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wblgrxwz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3knkschjb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqqzzvls.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udlkakmb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhslzbem.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmziymue.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3byofdynn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iujgxihw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vocdookp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jejyxxbg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtayennb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejvcaxpc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flsryvsm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qxadjtok.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hhcmpacz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mxwhmwvj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3srrhdmyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yqyhlouc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vjtuimbn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxxoktw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rwbjlizd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xvlxalgs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3grjeptek.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ieftofqn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fljlbleg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vcqultpb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdmphur.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nllmgoxu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vxkvvzha.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jykzlzgm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qvrlyssg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lntizusd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nilpcmyf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rpugwqzd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3toowigij.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rpjlsizj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zhurkodd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rzpbxxlv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjetajfq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kdipwexj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jmbfheco.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ughtttgt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nmalkzms.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnaixuga.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqdylvle.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vyacnicr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zglrkslr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxndozvv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjghdttx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xmabhhqz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhvjxueh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxqalvqb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbwxqsmm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmfxkuym.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vevnrgpa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jrgufjcs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3myrgorfy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hfrvgcns.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lgmiiukb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yoykaxgz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qbaempem.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wbfogpbc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qszvxzdc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hcupzgyd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qdfhzfwp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bbheiton.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3acoerojy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycdrknej.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ezmikdwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcksghmj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ygribsor.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hnhzolgb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3omoviykl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqajkuqn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vomzrnsa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjkiyrtv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxxpwds.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3inbivgfl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jemfocat.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbnmbztd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vbfiaamo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mggytzfh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qirutozu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxlgqals.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mahrracv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jvzuedke.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrhoalob.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gakrokkr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3urfldjyn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tpevuljl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3concsvom.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xdwgyixq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3cgkflmhy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3iabzcdwg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dgtudjup.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cqmjwbba.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3irgytddo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kspwvdsv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3itgyxvmq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtssxaya.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cbiabzvb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bnprgggj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayqqkkfa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sgespghl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zinfiiiy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3krzbmxin.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zyccluea.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rnqyhric.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfkjotkw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uraedlgz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzphpsik.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jmoxzuiy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3eqxlcpsf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xqofozgw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvrgdeqb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mnpfblhv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xffbchfe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3obvjjgha.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdeakbdx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khwsefhp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmfjbrjq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zotdbowx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzkmhorm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wturbtci.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mqpycefz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cwylrsgs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zbckdwlu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uwmimuyt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyedqm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lyjrdweb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yxbesahe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3efknoytc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3azihktyv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fuemwwke.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yjhelulu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3owkmwntx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3argxlmwk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fwngtkus.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3slxcaazo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zjbtjqdb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vlyjhrms.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mijeppfk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mkcbcqwy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ylvxnxbm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpvwrots.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jicbsmas.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmidnlcu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fiknjgls.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3auadjkhr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yggypmbw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hoszjpoi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hkebarae.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fysgdtin.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xzovyttp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ztvilywk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hhnvcufl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qkhmnbaz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fecesvtw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hpjxarxw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ymsqnmxa.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nrwnnvun.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sgioavar.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3frlbomll.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gtehuymk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bcqoduzs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbvbfxc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3loaecunm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qfqrhiwa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnlwxdbk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jjfdtjxi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ovdbfcsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axnebghh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpwonjrr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3naveduna.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pllxfofa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pxgklfwn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mkznztdq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3svmcguhl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mycejinh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ipoleayh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3itmsgxkv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ohmctpyk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kbifsvrx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3momsnkpd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eazynahy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dsnkhwht.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ztzxsyxx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hczuodor.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zcfkyxwn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mrirgihm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wkhxnttr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wmqpvwsr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3eeppxabg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qmrzqizp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ivkcbvgj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3liibpwhd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bcgzwyck.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jsgdybbb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qiqdcxvh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cwocaolz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oqfgmsfp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tvnasdte.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wxxkvekg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ykvyhzwa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zqhgmdwr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vomflmzy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ypbruzxf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lhrhtqyy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jwutgyyb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkhionn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3adblvlot.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jvttoaqn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qdvzrcfe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kehysjhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxajxbem.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yyuemppo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prhyrzxy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cimgcsjk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wdwgesnb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3misaihze.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3toboxvmy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fgvhnatq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyeurkle.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mfgyqvow.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbbgwqht.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3efrijmbh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wzhfscoo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sjanynbd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3enzdfqtu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wkybonpe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lmevgnyd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ivianori.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tjnfpbzu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3atukxaio.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqedbkcs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qixgiani.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bpghccbv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bgvntioc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3szqfnwsn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pvpptfkz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3szspicin.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qmmdptzm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3utbwkwji.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wcdtaqjs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3taaynhmq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dvaaownp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqppgymn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tivgiwbf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wfpyzyiw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiatvjpg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xiajnxrm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rttrodoh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ssxvtqqw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbmomofb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kvxemagk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3utslslpl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3svvpocbx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzttjetd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaojonwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ckihisws.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ibfkpfau.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3eqiyfmzh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bscpbrtn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wqxfgsnd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dyylaftz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pflsntnr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3azhjxmuf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbmivvo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cslndqwr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nkoirwnt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3grcqjfsa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bywbcwnw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3mujvmavo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3khyhifap.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cmddfgyo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bfgzibez.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jztzpbbi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wqvrspbg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3efrjswwz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3txhymbpo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3tqcugrjj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3lahppytl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ftnhuscw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3jhzyfgco.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wuiqtbbt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3schrxipd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dlyddzmw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jsifxctt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3xuhdugge.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jymjmyjo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3kwhyqniq.html


<!-- 参考信息 -->