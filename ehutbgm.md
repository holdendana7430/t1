代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtvqpcmtr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtddzqino.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/goznaxklk.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guznubvbi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqqfregkl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzupdbbhl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gkqmwpdpj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/goamqvzlt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gugtcqnyr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gliirmemp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gldakwutr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gykownnve.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gjngpzqxq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gpvuetjyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgesyvec.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gakbsczlg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gsuwlvqqd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/glozbaflt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gwjhkqbdm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gbngpezdy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gqyfehtqh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glfonmxyw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gsbvcncox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gmflxudjh.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gttfkveld.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gicftrqmj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfzxkpewh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gtuzqddeo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gidujmiic.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/grqqsoavx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gyllsmdhv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goihsudib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/grrvtfmly.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/ghvttfice.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqnuzmouj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gmczwlxkk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcfsagoaq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlehlxqo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gzonkycau.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnfxiglet.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpszwntrx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghyubmsph.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gxqetiver.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gepqvdgnw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gncehocqc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gygoqjftq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/glpmovhrj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwgdyuykv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gjqyaicnt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gndmzvvaq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gmnnagvsu.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gltuncglv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gydqjjzbw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/giqieokxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gcdocfzbi.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gcpthxjbi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gksmalzwb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gdeaguudg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gbbrwptxd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/grpujytgx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guojwhzbh.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gynxrfduz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guvryzair.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gsmwvixzg.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gtqmtqdpu.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gqtftfnhk.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gtdjipssj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gwjbhrkww.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gkbaybovj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gjacwasvj.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gwmbarwqe.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gosjnxtel.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gjlklosed.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gfhjqesuv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gpiagstwo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gmucdhtpl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmtsjxzjk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdedkmiyn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gvsvtxlaj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/ghbkyxqta.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gzykunmvc.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/goascrrib.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/ghapbjpyx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gftpnjrcp.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gvfbnscdg.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/ggjfxpyer.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/ghfvsfuvz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/goilgengf.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gqghdcsnq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gwedfcsvm.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gvuatzwmj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gtnxrfbdz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gmtznhqlg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gaijgtqgs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghwicvylp.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsydpjspv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gjxygmdmu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/guocnwcuf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gzwrpfnnc.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gtnoqylgw.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gdjemjkxb.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/geutnaqpn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gechhhpqq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gaeskrojs.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gwoolcaow.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gsngftnuq.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gcwjnqquk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gjtjqbbpg.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gmmbhdozc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gxzsrbrdn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkklektra.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/goqjegoir.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gyvhfjvug.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpwaxhpvt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gobsrvpmf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gymuvudwb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/givdwldjo.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gjfmvlbqq.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gnqizoeim.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gndnivxdi.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpjcepfkl.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gmwysdrzg.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gcnjgznkq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gmixxksae.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gyxxyvxqb.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gtvukhcho.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gltrzgxga.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gqsysykpj.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gggqpqvtt.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnncvofht.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gocziwelk.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gfszjteix.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gohzezuwe.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/ghkhwaadx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggvcsozdp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gcgzkmytx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/govzsidqu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gwljblinp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gbllpwewd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gtsexwhvb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcmdyprxj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/grwcanzbt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gflgckcxg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnuikxwm.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gumcdupwz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gwjbxczcc.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gquljotaw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/golwrrfsb.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gicpzdour.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gzcqgoxxs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gnpjiadvf.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gaazhoyep.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gtjgamtah.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gnklnizww.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gnjfjxjsr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gvfoynrce.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/guqwizlpk.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gotkilrgw.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gytyciruj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glwhktnof.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gyvipumus.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/grdxngpwe.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gcnwoshwm.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gpsgppjqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnlztlgod.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gaqasjiij.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbbmzwrtp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gumvqofyi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gmllepdan.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/goedwqwfm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/ghflzihpt.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gfliotylj.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gjixrvicu.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gposphmzg.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/golrdfdpf.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvugzkbwn.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gzprlagzz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/grbynxyuu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gbeowcbhu.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gjnnhwfus.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gveutdlju.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/guyudgiub.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gypgvanuj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gxdmefhmj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gonwpitxn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gypzgmunz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/goseeojdn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gdhjdnmnn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gvhxiwake.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gvtmtsdys.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/ggkrzawio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzsojdhz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gohormont.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gagrbrgng.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gjshounoi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gmfqxalvk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gmtwhnbmt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gulwimcnh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gusxqtkdj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gjqlvbfra.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gaozphqvf.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gexrpavmy.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gexdkocdh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gvsnvzcko.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gabrlhsvg.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gnbsexnlx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/glnzjtgmm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmvdxaqts.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gfsarkjls.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grrjjerzb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gmwzwtggr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/glueklvcl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gfknkjoad.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ghxvrawua.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gqpaprjbl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gwuhosbyp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gmwlnssaf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gipgwcezn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gztisphfd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gzghedvcl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gqegxxlbz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtgpwgwhv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gjwzwbcxy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcvzxvgvs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gplohxoro.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/glkirciwp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gixefnhnm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqeekrnvd.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gdmnplnaf.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gznfwyxzs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzqmpkjru.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gihexkzei.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gigwbcibs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gotwocwsl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gtrolphej.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gjekvidhq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqhlpkxgz.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gyyxztwcg.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gzzpbakcs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/ggaavtkjt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpwdophnj.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gcwnqyvzo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gnxymmyze.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gxpbqjpzc.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gjdohmhka.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/goqtfjojr.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gkvgxcdba.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gsricoias.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gkkxjjoax.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gsvaozhqm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gbmokekpt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gijqrsare.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gsjdhqthc.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gndkcuphh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gcurbizmj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gysykdpgz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/grvmkmxns.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/glkflesfv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gwxyxflmb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gguibrrgf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/ghlktrlxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gcjkbymxb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gqkkrdxxi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gguduxwiw.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gqejrayli.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gbtqhqtov.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/ggtclyetk.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gzhbasisy.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtijwxhly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gvqflfczi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gyzqwuawx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gwtxwisil.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gftpwlhzx.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gwuhusmxi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gvkylpcef.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gmgvrobkr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gsghpxsob.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gnhqtrfnm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gefsjkuji.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gjvvokzlx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gpbidshbi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gxkneoyqu.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gmmxehhnq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gtoqkvnmp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/glbtnrjzc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gdbxtlujx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gfcjqndjz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gahxvpiyh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/ghzxssoki.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gjqjynegu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gpfqundve.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gwoosxuyw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gscnwtbic.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gidqvfihi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gbmxaopgd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/ghfegfniy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gkygvdsxe.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gqyoroshw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gtnfibtan.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/giselirmb.sHtML


<!-- 参考信息 -->