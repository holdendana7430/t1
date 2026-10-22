代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2msbidhks.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wvpsacqd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyrdakjd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubimwoxx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azarxtpp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfegzbom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hljqbgtv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avolmuqi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzmyvouq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdxwcbsx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2beyrjgbl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmrgiqzi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfqikavj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paslorll.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pybrltyv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewwyszfc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ioraqqgg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iinfoqfc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jssadtap.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uhcuhvwm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ehivyxxd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2knhfzwqb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ucifpqta.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2udkqabud.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zyxyepbg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tuwjudgn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bbpidzex.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jxfkvcem.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vdhxqukq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezoordva.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2whbjpydz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhrovdgt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iosxbkql.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gpfpwemz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hzudfaqf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hfnskkjb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2oeifrgsx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtdhlfan.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2koolimfu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nsdsgcqd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ulpcxsmp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwyeopyg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yzifchcs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2konqlhqq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2btjwsybh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2atwqrvnv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpavlxsr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2amsblujn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nthmqrqr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdvicbvi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vvyiksvu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omdpkddb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2amssdvir.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhmezgey.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2amdgrier.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhuxghan.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hpazluoo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xajafuww.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvopnnem.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpcewup.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tuvnsbbu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjbjvpca.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fmbnmshm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jmrswseh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2glwrcazi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mpyqppou.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tyxuzauj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ossmjvcn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rinlvvgw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vqvhgola.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2igxzsatl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2syfvawub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpmltkqd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vfzlqsef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjmemorf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qehorzjk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ruxqumru.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zhqxczsp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wphwuyvi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ktllrftw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2boszqtnb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2oahtcvrq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2djoqzmwp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yqyoujfb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2krabsvdr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2txvgxyab.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2akzaxmuf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umedtpph.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejmvmjzk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sgtqfbxp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nepubymj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2abneibus.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ituajpfx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eevyzxnv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pcmtscuj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2idywwpdg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ddpkuoef.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nszqibbq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2izmuedij.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mvuhxtvo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qycmkvom.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2svmwccvf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2egipjfiq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dbaprpoq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wvogbovz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xdfbbfqc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vrtlpoec.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmeydyyp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lhpsmspi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bodhrkhy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jphplojr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gussxkjp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vmupteor.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2apimxbtw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2grlaoxti.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wtjkisrj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tmgyiupj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2frdiwffs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nqipawnf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pvywpdkd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bppiiotl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2akopuqyr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2scnovwpv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dymceveh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2brpzdzpr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2icbihqre.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tpecptig.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2crpngtxt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2skoxrywm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jgagcute.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zibvjnfz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qsmyjreu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jepqjkty.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bkaurcfz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tlabvqhx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2eviqkfhh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vklhwfzo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dlynoces.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sksygaec.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lpmrelvu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2udjebiaj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hyemzsww.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zncsekcd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrwnnarr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2edrizlmb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mvfiwotf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2snhyltwe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2auttfhti.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xstfslez.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujvhmfdo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2irtmleai.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2owerultj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2poywqlzj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ksaewamk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eksojtco.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2opixmezc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bwtfyjnd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xprtlfnv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2smuwzgyj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tuksmyis.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2spsxuolb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tbfwfkgg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qmsexnvz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2klzziwjv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zgfjlscx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ihhnpdgq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pvyoyswh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gigbrjsu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbywfrww.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blkdjelu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zoizbcyl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ldauqbyj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dwyobdmz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2efmrkhyv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kslkrkft.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pqxhiufn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bysgcdfp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbjvueeg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nflnirbh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qlprlukj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ndtxzhpb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fccooagm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dkxisvfg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jwzjhllu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zpefzfyh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vxvekjbv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ubcpqsnr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jlwhqyyp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yeztwnst.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tsjrixij.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lpuhgflr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wgprqhqp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fotfwxqn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2puokwsic.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qmlvpbqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dtlrxgwn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ufzmksav.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jgvxbvny.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wuosmmzr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2urrjjqvt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hcvphsri.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2unjadorl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmxlqtij.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ydvfcxjr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bybgnggc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2okbyepsl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lukwpilx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xromtucu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hekeiqoz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ifoqgshu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rgudctou.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ujtjzjye.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2exnsxrcs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nguyrtus.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fexsvqzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2udukysgt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bvahlqms.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vijvzzic.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2begmihmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhpwzaij.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iiidyqki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chwtsaye.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wiahgdnw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tzlqijoj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdupgqmi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2usrmluag.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fszkzomr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fjronxgz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vgnalkjb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nqeuhcwk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjrjuodf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cdnfutto.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yxhtbazc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jibxnclm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlecwit.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruuvfpiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2riokxwbv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2iabkjzae.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2phewfsfl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rktkxane.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2oqufusqg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sndbgqdv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vkjisjdz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gcxstgdv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ilohjyxg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zifuahaz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ansdzjge.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fmxprprr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2muozvydi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tifdfckh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tihkppcd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymdlgdke.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdlufrof.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wunicqkn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lqwnayvv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ybstvjho.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ocnoqikm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zudjdyus.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nlifmptc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pbncnjnc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qgnbcvsf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ljwevzpe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyduflox.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tbpyyvdw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lcomxatf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2blzpesfk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klrycknb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zxzodbpy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2weeqvyez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bsoukrfk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yfruhjxz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hkkefokq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmkgqmk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tonpirld.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2flgcdajw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2etpumrzo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mmfgwkqh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uossqmkk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sunhuwgo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qqjlvkde.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cvicgshu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2opczrnkj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qngmuroz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jkmhrcgc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2croeliur.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hyzccjra.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bvnvrmoq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jvbuxesu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hhnfyorc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zebepivn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jkkklnva.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zvvwxjut.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hygrrztp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mqnpvrxr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bmmpifvv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2zguedbxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fhiydpvq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2yvopgpva.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xxomqwhv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2albzlecg.html


<!-- 参考信息 -->