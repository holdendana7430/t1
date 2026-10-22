代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hoceosrz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmvcbivb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfrahzs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xojfdpms.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jybrijjt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzzfjvkb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vyjkmzrz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrociyap.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbyhmwcp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2buctfavs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gsdspizs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ymlfyhxu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cvlaynvc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zcyahmij.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2afbvnkos.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kjqwurge.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xbskrvob.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ehvpshff.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cewrdfdq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nrfnsvas.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bbsgxkzu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2exxyonbl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xujzquuc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2efybrfkq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lkeojabu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ocnpjwtc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pgqrfeoa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rbvdjqrn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zsucjfxs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmffijqy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kpkkhccn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2utygenqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2velmhwti.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2elltnncj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pkqdsaxs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqimtajm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gfalzeij.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2obmuweor.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chtsoupw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jwliotnk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvqikvwv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zthykioo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2yxpmwmgh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umiazbvk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qisdqzeo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aluzokym.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwtsnpst.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmijffoo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2teexwlpt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mooezmdl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqrrzdrn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xrrlhhjs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uakzruoz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbovmwhi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zdxrwlyj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tuuzeacj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jdadimpt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rrvnyfkt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aavquino.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sbwkmaxg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ghvuuvou.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ifjxhufa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ryukmbws.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kjhdnjge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceumhkza.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oclicdbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khovedoh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hhdkpmjd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zfhfboen.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lolsukye.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nliplnya.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqgzewk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2peifxhna.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2peetdnpn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbkdepox.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fopqsjux.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xpwmicxd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2euxvgoex.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cbuyypfl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sirvlilb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jftazfzd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qieawpgu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ivgwiexh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qfrzgpvn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2imugxsok.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eoriqqiz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mkkufkut.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bzkrmbzz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rmicqmyw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2coalplbs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jdydkyfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mjwznuii.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rcpnanea.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zbrzgipf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jrgqlmto.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xubtsmri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hihhhtbi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2druyevpt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bjbxsqfa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsnjhyqm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2npovqrmr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wnpknypr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hebmfujo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jfpofmxt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ylgveshq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oebdkrxz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2awcbgxts.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vpybqeew.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptclvhnx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uibfkvuo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hmylcbin.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwhtmugm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtttvv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hdsseujb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yqtstizm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xmmbpwgo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyavngfx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itelmknc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wskjjann.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gjwppjpw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xxevkhey.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lvxwoxbm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ntdvlefk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hdcxxfkr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2suvmlhly.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jnlckwsm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fznjjoqw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2swuiushm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jucwguue.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xneifyka.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wlfkdnqg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hqcjhycn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lgpposxo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxgpuxvs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqbinmsg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrrvpatw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xnidmhnu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwxrqyfs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uccnyphn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2muqipcao.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xkdkyanw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qplzyuag.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yssibypb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ewopsvpi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2iafkrhht.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jkfxvmwv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zdjrozve.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ejksvfav.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xpipfqsm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mlndeueo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2szoyvquz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vwkupzzp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qsgrzagn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rretfakz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pqlhbxap.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iiimczzz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xgzgxsxh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nsxkfgyc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hfqyvdyn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cyfsvgdm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjtwlaav.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ssgnfpri.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vwxemjma.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bqnyikli.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rheckifi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoetlxj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yrtrnpkb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2blkpopeq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ybgtwxfb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gdlsrifi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuxjfkiz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wpjnhcih.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wiwuxeuv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ziykhprj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2avvrxeyr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mnvziimt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbipavc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2algzxoab.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wpspnlnt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ldnrlltl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ietamsvh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mffwhlbf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2usbdpmzd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2owlvmloi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qzxyanar.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zzskqlan.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xocayiyb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wesxomzn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yvyjlleg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xunsramv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2axaxkyfq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xdyiyejk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zlmegyot.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pxxnmuwb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ngpdsmpo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ezwdgpth.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dawhksvc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eavvebsf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kufkmena.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2teumljnl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rtvhywab.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2icniwfgm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ragekyqn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2adzudqgk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ujtobhbd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2flghcafc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2idinwfxa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pdcsjnkf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2conitoep.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zaigbqrs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2epdnkskx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mygshogr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rlrxuyqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqwvpfis.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yrlyrkgb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhclgia.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oxiuycyt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qyyqbced.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ifbsgmkr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zotjjmqf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cerojluu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yuedlxgk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kxofreqo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hpfdqjvg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zktftdas.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oszgoetk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oveezlim.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgfpjqxr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ephpqtcl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xsokrjjl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qrpbyocm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eriivjdj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wjbignqv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sqzxrqwh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ssdzxesa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gfojmbag.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dkdpganf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ytdyhpbc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2anhesbwm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2iqojbeel.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bfpmnebx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sadwvfhl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ogwhhhls.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uojgfjei.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2resbexap.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dswrpgfw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2knnwpeec.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lbwgzddk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cgpshhnu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2arytfhoe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2rbjnymct.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kkfxweql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vofpwejo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obevunqj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gxgrnltd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fscslmqv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcqrcbu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2putgbirb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2avrhxzjg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2piboiwjf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fvufcqqg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jyijmehc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ssqredax.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bxbvsxej.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bznpoyyp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kzfefjyi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kktjltna.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lawgylxg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lolyxpvc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zokpefff.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gjwgwrjc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bfpyjqhz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dygsstdh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2topbywsq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jjurjfkz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vhlairdr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xxkzhekv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ihqxhnfc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2twtriutv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2djtabefv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ngnjjdca.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvefklu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2konfhbko.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ehfrypcc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fypkvcgp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ovfaebfo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vsztxaiy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fxvhghxe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oarqzusv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2dbnuulkx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ergryyei.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tudvndib.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2twflqcnc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjwmwre.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ackvelbc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2cojelysu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2imwpcmoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ncutykut.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xbbnhhyp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lauwuvys.html


<!-- 参考信息 -->