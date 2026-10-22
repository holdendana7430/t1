代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhajbtsp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xihwsmss.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tybbeill.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tnwqqbex.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdyplqjy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnubvuvv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pqzrfyeb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctauhsil.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfeprvrl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bcrsbizz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ucvwnndu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kutpfyvl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tpykurss.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pnsucyws.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2quwfblfa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fmyqkomn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lhkjvnap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2shfdioih.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ikboryxw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hwomynun.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xkqpgxoj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ciaodbvm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uleimppl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kakgsajb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tjbxiybz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dywkxigg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jccnxmra.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vshadeyg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vdnuzghr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2btlgmcbq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2caaegcbc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2patfzcle.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2otxhvcui.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrhzagqr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2spomooxt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prepfsbp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2slrjlvmq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kksgmntk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryihgvxd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oddakqny.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvaabjds.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlcvnlvf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qngslbov.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odlrqojb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jywqxjof.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eenqokfs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnrobiba.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbqokqqj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2finpptxc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jniqtcnj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2raulxzlo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xaamdbmk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wpufstog.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddpsevsx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qpzkqlhq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zrycvehr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2luzzneiz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jcwxglse.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kjfzvdkw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dsgpekrj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kwktrohv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kwkgirik.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hrxuumds.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vcbvfmcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcwwgryh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jobyfhfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmieikbk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rbqavsvv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2riomygvn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lxyhqroo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqwycelh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jbviyxnq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rsftjahl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2howtujoa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhtivkvy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wkjxrbvg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbyjykcq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uvkaavjy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mmzlugdb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaxcaqtb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwwsmgrn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjvzbfoi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xqhcwifd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2twmufmxr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpjwgedl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xncawcla.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kzdxuctx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hdjmgens.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zqyayoyz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kodrxrqv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjoholnj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ondjkjiu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rldepsba.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omfbsraa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2anxxpkrh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2smztustf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kxdoextj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2caazaqca.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpxmuuzs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rowwhfnx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2imxwfuyo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lncwrzdk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ztepmkyc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2asvagvah.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fjmzafxc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rnklzwum.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2amhorypv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pytwwwdh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2edyaxcta.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yhauhqcf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2szhaxatf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iauxotiu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2utgbzgpa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jomzazyz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jhrfalng.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tfkpiibi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cclidusj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iewqrcfq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2amchxabu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hioyrtcb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bhesdwrq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tprvhwky.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xafafvqe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cobayjpy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uijasyva.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2idfofxat.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rgujkpcl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bvsqplih.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tqlsafkq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2klgjkrlf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tlrjdzvs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2envtlhds.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2knnrdezw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzzxokni.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qcxndqgc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wyscbcdv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ljfboddt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tfmsoibj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2drcwbpqt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2szjynivo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2irdqjvsl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlkvnbon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2urssrmkt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fuameudr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msritlpk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xhulxlgm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwmeiukb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwienme.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mhomxsii.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gcaegdcv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pzikbckn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dtkmzixv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gtptfypv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tpsiahgw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2yxujckqc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wngprfjm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pfytajmn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kdoevbal.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yeatybxo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybswtwyv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsxknvxy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2siftkfmj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gzdwgahy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jppobjav.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vtsflstk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ioklwirn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zogkwpoq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fgugptoj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scyisnpo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrozcjb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgqimugj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlvwvhxz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ujznlwif.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2arstlrxn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lywxcobs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qvhfsfkm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzwgtiy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2azlasypr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dspvyewn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2byfaqjec.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zeuvivez.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2smyakrnp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2srraagmb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jyjfjbbb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vziilwow.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fkitvzbw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zukndtuc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2trfnrfcu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rcczhkao.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pruzytrv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tinggimw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vtyrbqwr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qyqhbapo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rdqqkfbt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqpdxdad.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmsfxrxn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2trpgqfov.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gnpyksgg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hrhmqxpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sicykkyz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fpbyrhfw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gjvhutcc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mfcwxvhc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2woacawgz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2raucwqbn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xmqpxtrz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oryfpvsl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dbilpajw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bshhcfgt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2sdkdukla.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xasbakwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwgqiorh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dfaqqvmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czstksue.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ggsqbwws.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pjikuiag.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjdgvcuc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2caerrgnv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ocsowswy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2eaziljil.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gpjcijqq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hasgabiq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ejujdbpm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cgrlstvn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ezvwjevb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmpoqcg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhldegwj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgpkknl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2btfbqgii.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2houiunue.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wxvpjbxx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cswwzsgc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pzfsljvo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qsyvnohp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dvqspikm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dahatdns.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2guchwapp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2chtocbkq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lclsndup.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2rtylxoao.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2evoxlxqm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bgdywfkp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2udaqgeas.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rmolotio.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vdnavsej.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvrwychj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgbvvlwr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2povdqzzc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ixjramch.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qjrnykxq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gqhvxtyh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xyaqqlsy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rbhipofj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsatdylc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwrufuxw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wdjljjnv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2guuoitgx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2fhoudmpc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezidqgbh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mggohebg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2eogiqvkj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ncdyyjew.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2memuztov.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xdzrvaxv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ktegqfrp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwznkky.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kashzgeq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ytnjwyiq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2twvsseej.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nytygqhw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sagptefe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opbgefqx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vfoibton.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2giryztjc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qlxnooov.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hfnqblku.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yaisyvmc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vsghgqfi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vpgmhnvo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wxlxryin.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ugygybms.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbhnbul.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tjgkmnts.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hkzotvwy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gwnyuzku.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ifgznnjl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pulvcdhf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qdvnpfap.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2azzacxwm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qiwzqpgw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2trxeyvyt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnzogbsy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wtjfiwtg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2nqrqputk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uhfugsqf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2pjorybdv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2umcbwrsl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qamllrwm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2abnrtqaq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dbxbpopf.html


<!-- 参考信息 -->