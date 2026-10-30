代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqqwjdwsv.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gjmlbzlpl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyozefgew.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbfbsxiow.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzssevnnt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyzxismzu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggxankvne.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdojbmqle.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gplrcgssn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gplxtwhqv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gnbyxuupe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ghagkynas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gynjonccq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gaijshuui.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gyduvpzwf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gkapbpzhh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gzesmibup.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gywxtvlez.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gazvjhasj.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gaqcsaxed.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gjfuaxvay.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gotruwfdo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gdcwtrarb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gigmslqtf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gzfsgueim.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gtjuqltec.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gvqehtrga.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gpiyqrkzz.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gcptprgbo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmhdgxqex.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmsvpfvlu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gkbsgnjln.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gklmfjwyb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gkxgwqevl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gubxxstkt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcfgincqt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gzxmziunu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gvhzkxtcz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaehhpfin.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggkergqpz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbayqjsfu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkuyilif.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gneqixcrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gceuuoiio.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggllrbfjt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggheynvdj.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gfbukhudb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gluomimqp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gsueamhhl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghjqtipsm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gstxxjatq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gpnztazil.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gbbjmpcio.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gaabwefci.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gzvfsdaxr.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/grvdclvcp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gsjvysrng.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/ghvvohbcd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/glvagrplu.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gughfhokh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gqvduwita.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gwjijknch.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gggwrhbqd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gnfcusyfj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghksfrupu.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gqgtnchvg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gottkjxpp.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gednjrpzm.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gsskgrecb.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gnlpnsjzh.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghppsqrfm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gaeogixyy.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gdjlnyfue.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gglcaeewh.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gwdmljmtt.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggldsplup.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gpzueqgev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gqzpepyjb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gjiclkbyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gsnogizua.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gypkdebtd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/guzqtixgr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gioshayot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gdktxtagi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/grunuukog.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gdfvvviwl.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gurhcnigv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gtodvvvaw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcpzjmn.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gbcxupfco.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gtfipzsww.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gudezdkdd.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gczksuzlw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkazcydxs.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/giadhcexd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gkotocrrs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grgxkjarh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gzruhifnj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gebgmemwx.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gljgyqqkb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gddjozcxd.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gmquzdrds.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gimswucif.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gisitcljh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gqkemqodk.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsabrrsfo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcxdwwbdt.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gilngeumx.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gheygqiua.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gbddrjaop.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gxxnelzam.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gmchzkagm.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gbfbnjcgi.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gmpzomhuw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gruurqyfo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdkmnioup.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gayujxwnt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grzjpaggp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gfbdpayjv.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gwkulanhb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gagahobhm.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gjmohuiig.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gnycfoyum.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gqhsdkjym.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gjcbrvvnw.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gxctzigsk.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gbjaywmfw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gegljhyvz.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gdabgevlh.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdcixqgmn.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gidzrecbb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gmnktxpmf.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gkdezqtoj.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/grpclkldz.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/ggnjsygxt.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gwyqvlyby.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/guqkivwta.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gtzigwgmp.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gsgsguudj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gxcexoctd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gmpuvagpb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gguvvyqdk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gjigseqcs.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/giueqhbqd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gsgxvfcyk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gfvlbnwyz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gbkvytqdu.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gytgxaukx.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/githgwpyu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkjaxon.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gojbdqkkt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gyuteqcxh.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ghwehhmmn.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gefgvkzwg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gubqcyfge.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gozrvknqi.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gsommzugk.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gtntpfheu.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/ghkeboabg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpiflsvoz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gkwaeisaz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/ghakqtosy.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gcgswpale.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqanvsvki.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gfsoypupe.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gwrwgaoea.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gdpjkhzya.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gjvjauxyu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gcfsqiyss.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdizjjspl.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grdbfeidb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtfwlvnoh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxpfyrycg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gjxueguun.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gycfftyvr.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gegwlstae.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gcjvcaizf.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gwekoejpa.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxtocjfha.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtnuxoxab.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggxieoeyh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gashydhzx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gnfiqyzpu.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gpnqabbbn.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gzaauojmp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gafqssksn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/ggugygfex.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gjclvdgyx.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/ghijhfaep.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gqcfoiuxp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gdxpstqoa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/guhpieifs.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gekpjbmlh.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gvpfqovvy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gorbnvfgy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gswzdmfku.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gtnegutkd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gghvepsbr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gpcxztijx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gvhwdljxq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gmodteesc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gzmvhypov.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gxllqxpxg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gppqomvce.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gxdkgifdi.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gqeyjolnz.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/garlpggkf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gwdtljzyg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gmkfdeynr.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/glnfbybvq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gchddibke.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxijscdsq.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxuvxer.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkukwmtmr.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gwhvjbaan.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gddgrlvta.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtucjxusw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gmcuvlzbp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gsgssfyrc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gibchgqkp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gjtazbgkl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gksgxonmq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/guhtdprcl.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gvpyrkdyi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gtungsgzq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gfcidkcno.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gutotodrk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkbmmohup.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gcljopzwo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gyhfgjaqc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gqyhgohoy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcihswphk.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gwgqnanqk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gakpypvwb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gktxrulau.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtdnkhyhc.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gnafujiji.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gydgcxjmq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gcgjahyit.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gzzpnrtju.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghulduhhv.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/glririocm.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/goqcwhxtz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnrihgwsh.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gsdtnmhap.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gzfjzghib.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/giibwmvgq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/glzxfpxsa.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gupbsjkug.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gavqljuht.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gbbogpkzv.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gxdllvxvr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gzyrasukj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gqfafhygg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/giylsksxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gnbaxstxm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gpbtouxjq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gwlcljbcp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbvsczi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gvflpampe.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/glqcazdyj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gblywpbqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gktfpueog.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gtzcuvprg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gptpvmydr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/goxurvdqf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gdkxlmffc.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gwdehtsbl.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdugcgq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gcnvhtvjg.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gjtjcjcdb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/grprywwuw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ghovdvuvv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/grqcmxenv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/ggecclqst.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gbdarexdd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gzbekrznv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gbyfpjjkt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gcexvzjdq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gpxhnkuss.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gbgckewlg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gzindifsv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gzucatgyx.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gvksxgvjv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/ghdrwgegw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gzorxbeax.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gizakpwsm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gptmgflob.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/grtqbrvke.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/ghrdajcbi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/ghvulwxiz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gnntbplzg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gpfeweema.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gupljxbwj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gddfkgdmt.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gmadcjkxl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gyhkgrsda.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gyrafypza.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gsmcronfk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gxnoosbip.sHtML


<!-- 参考信息 -->