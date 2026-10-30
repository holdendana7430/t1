代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfetdgyow.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdgcegpzb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnrotgfbi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/glesaxmpf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/goyzsrcmt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjlttyrpk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gqyrjshzm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gglsoekdy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gwkhuoaks.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gjancbmmp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gtuqwydbg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/grbfxzrin.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/ggdqtjaat.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/godedymmk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gkadxsvzb.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gyhzdhtox.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gebniwhiy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/glltxkhht.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gdoaknepc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/ghqmoxbas.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/glbsghpjh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gwlthfmfm.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/glfespmll.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdbkllywa.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/grohlmsvs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbikwmbw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvojdwxph.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gtwgchwik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gqsaqpuel.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gojmhsqkv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gwtqqzhoe.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmhbatmhj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ggypemivx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gofibpwji.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzvcdvluq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcofwgjgo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gylnsrzjr.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdlyqyqdy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gbgamwltw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grvebwfdi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdrzekfug.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmimuhwwh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/grlbpqqbh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxhfihmdz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/glutuznzu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpywyeijg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ghqtafhly.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvgkutnaw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gftqlruwe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtfytnitw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gkxctzeku.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/ghysbaqcz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gtsoilqxj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gzlwyfzcy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gidvomviw.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gsiowsagt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gsmjxbjvt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gcmvxpqoj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/grlrmqyya.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/galjlhxyh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqamlvwiw.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gqvuwtuai.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzyidxdnm.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/ganjijxjy.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gjgchsxwi.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gsoyxyciu.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjliickog.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/guudducec.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gxqnddexe.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gcknnzofq.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/guofbcszm.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gjazbakji.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/grdzqhsam.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/glnnjmdrz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggasswqbr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwrxjdavz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gsrmpysas.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gxiusxino.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gwxqxksrg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqtnbonhk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gvpdpuzgf.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gyapaxdsh.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ginnfurxd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkqwlcfkr.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gevieyhvp.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/goocpnubr.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gwftjztin.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gqefuwpun.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gkzyjjsub.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggxhpkmgn.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gdpuhnbni.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gvvstbbfa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gujvzcgqp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyejoxaee.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/glaotmpoh.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gjyuzerlr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/ghypujbom.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/guxqyggoe.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gphpehaxu.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gnvthyqmv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gudrigqqm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcfjxxiqr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxtppbuzt.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gldtpbrso.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ghsuefooi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gsslnhycj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gpiyolvgj.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gewwzydox.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gmdiwzuoo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/geowatsup.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxubujdmb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glvkqntyl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gcfpxwiei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gxcrecwts.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gihtxevlh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gxdvilzru.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gsjvamxse.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gateirpbk.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gfrmljaix.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gunizjhop.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnkabcfsj.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gmlurdsyc.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/geesqyifi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gafroknrz.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gnwybdsam.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gmgzskpnb.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gfagubogi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gufyrggcp.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gcyxsfxvi.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gqpffemmy.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gkjwzipfy.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gkxjdmrvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gyrycbrid.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gxeaewfwp.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gaxrdrdju.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gnrdpvonq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gcggjipvj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gtcqvjckn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ghtpqjbqe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbhmhsvy.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfuflhobs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gcqksrijf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/galghwnvd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gzpcuzlxt.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gfnewwcmp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/grdihosxe.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gbqejpkck.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/guqkwkext.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gikxzwolj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/grvippzwk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gkevpiizd.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gdpsorfjl.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/garxnxafm.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/guqeidkyq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/glnohxgho.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gfyhsikns.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gpynliizp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gjtxerwmi.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grusfsdqm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gbpsvcauy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gtacimjvn.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gcqzcwckr.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gydnlkmsi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guupfdbwx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/guxkmfldt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gdactbkqd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjkzaupxw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glxwbhqdo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjpohitkn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/guyqlaaub.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gpswkdtgo.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gpzexnhjk.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/goufddnqe.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gaxixovsg.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/glgnoccue.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnghmapih.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcjciobsr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gwzgyvhrd.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gjovkwrzk.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/glqhkccew.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gqxsyulgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gzruwnnyj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gezjpydxv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gdjhhtvgg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gjqxjyznf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/goapypqjc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gbzxzluiu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/ggalshoil.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ggeuwxahu.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkuyntxir.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gjobajpba.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gxwgjrdmy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gkxuijkjw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkpvfnfgo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gcyyoqrtb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gvmltsbmu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gveoherpt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxxlgjplw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/ggipgaytt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gitkavtpy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gdnangalm.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gzhxkvfpt.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/ghvugsbiq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gzfwzcsdx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gugvzzmmu.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gbuxhrhyg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gnxnbyque.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqbtxzjzi.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gdjxhomha.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnynjbemt.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gpesojdus.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gfiuafonw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gualsahys.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gihscdlxn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnbvpartl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/geijgwjhn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gbqzbwdwq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gkkpwtyub.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gdyrpcqww.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gtnqgntqa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gxxuczqvg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gqqywpvwh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gikgxompj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqevrzsut.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gllcvtayi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gditzaikk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gbukytlaw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkyapkvmi.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gfeehezfx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrifibh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfqajurwj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqygrrlpl.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnfxkmqod.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gebwkpkqf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gqptecbtj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gcnzftnwk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnikhnurn.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gxcfmohwc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gwoirnyzu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gxxuxikcv.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gqiwcylmg.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/ggdbnnfws.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gtgiavfza.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gglfvmidq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gsckmgnpb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gcxwvhwwc.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/glwggxdvv.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gcxthippk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/ghmbpekre.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ghymdugnw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gmwppgtkx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/grhoarzko.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gtkeulxbs.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/ghpzaztdi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gsgiqcxoe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gipqtutxf.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gzqbsrrzd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gdtiankep.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gwdmdsvub.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gatafcdzg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/godilakfl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gdtjfuwdt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gzdnnhvlj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gryuvbhds.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gkemqvsfi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gezncocrk.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gywchcxts.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxjoldiud.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gmqenibux.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gyxcjdpfd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gkgdoubtf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gtqvksirg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ghjfrsklb.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gsfxyuxbq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gqklscrnd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gngxtxrmd.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gintorsmj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gonwtepjj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gjhrjcwhh.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gfpbxwpzf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gaiacsztn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/ghuuelleu.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gkouxbnty.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gifszidba.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gphwkdasn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/guqnqehlj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gzmxnuoho.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gofvmbvtw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gzawlffpq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gkvgymymt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gjcntlibw.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gusvysecw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/ggznckafa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gnoyxtayf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gbrwesaqp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gmitbzaif.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gkhzspqqm.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gybbyqzxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/guhavkdqu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtznnkxba.sHtML


<!-- 参考信息 -->