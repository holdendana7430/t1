代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gcuznvkr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ttzqyblm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2viftnqqk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjthvguq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmbcwqcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ebqglrdy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mbzobpds.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yazacaqz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syonuont.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ygfdigwt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buxzbnaf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ecnsukhu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkzvhyhl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vafsmlhs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezxbsdwt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfdwcqph.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kavpdrrz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lcqbklcu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qboikmsm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2clfgxplb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zemfcvqx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dnanvbkt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2osijkvqy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bvtvfihq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2exapcsla.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xdcugwzs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ijdfxmcn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yvindhdu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yofxdwka.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nlvagmyl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gmbyuvpf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zagatmeo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2barcupbx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvjyvm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2isulztiy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mtkrqcuu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2txfwqqau.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fziiutnn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zvxoipgh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2trxognbo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wcawroxh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hljchili.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2esqdkzeb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2idbeawcg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gfdaozxx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xutwercs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnwkzehy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vwchugjv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stnvskvj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxoowumi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2frcctpmo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asnghlxs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpdcsfqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dyvgxnlw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2idftpyjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfhkobna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhefaztd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oumuexbd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sqtnzfsv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mqlubknk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pisgxzcq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksjzhcfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2azqouyqe.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bvwotfmx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jaarlcbw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2abienfje.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xkrhekho.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ulbiezxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ugoolwhn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2evzomuxh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xcmspwww.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rovvxlvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xppwheol.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lmolmhav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwnelaqp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mbdgydco.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2plkxhwuo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpetbbad.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jjovvgij.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjysfkdr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lgnwkniy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uptycijk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2todzewyo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xxnixwhz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxtovxro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ksnmcmot.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwwqpvit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2izwsqxou.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imfptcik.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2shimxkke.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zlxagzcl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nmhyzsio.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrsqorhn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2firjbcoi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2msvbvdsl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xjadyfyd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yjdhuvru.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ihkqfgsp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kkiowwgs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rnicrffr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2urggfztz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mkhddxrj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vpqjuxqx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mpigekpv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2esgmnexi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcttfoma.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymybgeyt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnmjkkkj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sbjpmjon.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2clvuoxuf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yrwtsazt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2exyosewc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qkinwmjm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqixypyf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xudtmpef.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2okfgxysp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lsrucsza.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ilagvqzh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gdqgadva.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2iqiupsmz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yvwvgamv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ouganrzl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cjoomnkf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkpocnnn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vgcnhuee.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2loadhvyy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rqwxlmhw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vqdzdbjo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hjbpvket.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ousanrdt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2anihsgwz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kjrlkmwx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nmmwhfws.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xzhuxren.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cdhsnehu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sekzwvly.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gwvrkjzh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xogmhzbh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dhxxlcpj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ziuwkxnz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vcyradyt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cyyauqdt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yghrqnml.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fventzlu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vltwjcfn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2iloyjlhj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlvsyktz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pbsvusrm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yttlqzva.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xbmeaejy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fzuauywo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpcnkmy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogarnfrf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2toxbyari.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hcjnsqvg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eeisiumo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ktwfjmfu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xjxoixpg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wlnydmqx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2scxaslgz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qiingpbb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ueqefsxp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2yhulsuln.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eprpkpap.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2byjecsuk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cmoyckar.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uygywtrf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyoorxsx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhsgvkc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oipjqgnd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbwxlcc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dxctjjwc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qnbstwvj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vmgcxglr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vttccdme.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fyenboye.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ppydedcz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2skojedxb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrzpazgt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnapundh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2htpnhjjp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2exsayxuu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wwwcnmtg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mikembvw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2djdgcvfq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lvdbqjux.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2weuejijj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lcjfjxye.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qpflzwcn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xjipaahn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vspceiyj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lausemgs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ljtacdwk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2uclatgis.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cbtqefot.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2liljpzic.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2eaoeopcx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2miedfptt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qtwuptrc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2limygtnn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vyfplfqg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kbmnilhk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kbhjtlcm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cluxanxq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vikaemfg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2adyuhdiq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jfblbkcq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2idigfnqr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ftysotdg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xykctvet.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2svczehof.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mdjmdwlm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2twhqhmjn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twqmdgow.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gobbepuw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dnusbzpd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ybdrxlum.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pxkhlalf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gxxwrieh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwzfjzqk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ieaysmhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hljoicmd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qisdndce.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vsgfoxya.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ckfrtjxb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pvotllac.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bxghgtlo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2emlckfor.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2btllrvux.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jxygopjw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cewpgwja.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2esevsytg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2syrtkdzh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aptvolsu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yoopzbrj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pbaaovtt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uwmqksvb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bqjezvxe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikrkczxw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uxqyhfjf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lzmwezcx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qflzzyqg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gyerohdk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ifwwctuu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vrvqdlhl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cekflvda.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dkodevor.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zdlacjjq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ycpaayux.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gcjxwwgs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uatpexjl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhsqtzfd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nzpevenl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ldyrpnvu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2whsbgrxi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2uboajbix.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lmzdwdad.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2yvocnnla.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fhddofzv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wpeechce.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtznksts.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xtoouaxl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vpcfszez.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2agfhotfa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxghqtf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rasyjiyd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjdqcaov.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2yimiqmlw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ynlqihqy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcmtkj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jkyopdpi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vmtgxuqi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzcdooz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zwrsaccr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vzpfdadt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hvnlhemc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jzpnenoy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zscridbr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2twhdplzm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qwiywlky.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hczvftwd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2upcyuqjq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pmdnpect.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kmdaaqbh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2utsjtsag.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gmwjfobw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lamssuye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jfawrvnj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2yiefylrn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2snnqbbeb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xscqccrf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2bcyjxgzn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2sttcmjyh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lugkptve.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2exasbouw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ucoidftk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xpxwvqez.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zdrkgioj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2nqdcrmea.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ddkkzake.html


<!-- 参考信息 -->