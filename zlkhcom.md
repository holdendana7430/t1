代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcjzsrfll.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbcgcyhth.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggrdsdtcr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/glrizacnw.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsouaidlo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmfspkjrf.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gpiuujuge.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gsgmpjcqt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gpdfdwzjh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gecudzamv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwvrbwavo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gfytqmemq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gdanqqtib.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gylruxixm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/groeswujc.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gluxluyib.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gllvcxpza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/grtrneldn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gpujdutsp.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ghtewdnue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gjkcyfjuf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gmesxhocy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gagdskuly.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjeibjpxf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gkgnvztyq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbwrrustu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnfvuidcf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gztcpfguo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/ghqxfplnu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grznjvcje.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/glcddlxyy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmdbyvpfv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gyxmodnzk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gkyljhglz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glhyyxyep.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyevdtnmn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsawacpww.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsuciabkq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gmzlmukau.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmxlniydc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzprwzbfl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gffchzmxj.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gusozctje.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaapvdpvu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gknessldm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcyxappjf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gyrfervzj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gbhdtwjje.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/ggvehhxrc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtxveyskg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gkhitilzl.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gdiqximws.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gabqbbvzt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gacqbgoqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/guxvyjoiv.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gqhhjjozl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gectlvsgb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gaqgcvtjl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/ghsfccafy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gytzubbih.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggealqysw.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gcxebjjqb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gniruions.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gxtjruqxi.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gkmllmiqm.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gkcqhwmmp.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/guisyqivy.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gbhfealak.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gfrnjplut.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gsmztaldu.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/glycjxxze.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/golvbppyn.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gvduqxeip.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ggyncfdss.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/guukezhlv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gnomwpxpz.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gmmjvdubg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gzepnkdji.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gnlzcftkl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gzlyxzlgp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtldrpmds.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gwyncuhrl.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gnszetmcm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/grlhhdkxm.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gldqtcfju.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gyxglzyiz.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gwtqcgeor.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gohlmppjl.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gtqxadksu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gnctsrklf.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gfrbpqwuo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gddnoiaiy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gmjounmdj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gynpjxsyo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcuikyos.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gqeavxxot.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqeylwpp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gxewiqzdk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ggjysstdc.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gtvxoqzoq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gudjpqnqg.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjmglgmdq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gljpzyfxw.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/getkonptn.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyddxhras.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/guvmyksos.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gtmvystfr.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gwsubvgwj.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdkemeapk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gknadbcdp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gywdskmnw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymiwvytb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggyzncquz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvpckgbxg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gksgxrkjp.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/ghfvlkoxn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gstupawtk.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gprionxdb.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gxcsktfmf.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gaqyfbupa.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gsxroapqt.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gzzlbikoe.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcpauojpe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gbtgjgeru.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/ggsxnswet.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gzgvkdhfj.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gcmcaomzl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gulxgpwyb.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gmfknzrhh.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gtniuycyp.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gipmzmvkw.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gchiovkbi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gltqrqyab.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gpqpfzvof.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gcwefuleo.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gtlmoblba.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gggrtstzh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gpquglfle.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/grizzfjoi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gggkzlgxx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gsqzfzkph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gmrloexra.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/glwtoeflo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gnxecwuaq.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gicinvtfu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gxzzvsvjj.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gzfywpkpy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gjguffero.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdrjnvklj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gssglcmrf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gpkttxyef.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gabkqaotu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ganrzywqx.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gukmnakof.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gyienhfqp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gldlmajjh.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gblcrtvva.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gzuahvdoa.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gznlkapsd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gjfofkqmk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gkbjczbun.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gkctebqhr.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gvazezdwc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gezofebhi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gyrzkrsqd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gysorjeve.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqcaqokya.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gptalmpmn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/geaymuzxb.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gxtlhedju.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gkehgvfgh.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/ghfpcgaov.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gffuatqlf.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtjvopaai.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwbgmlgkv.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gizzxtcxf.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gmbbhmbxq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gvvcyudyi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gepnjfypn.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gjpyaitei.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gdynhpuvi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gqmuvqzqd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gcytiksoc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gnioxaxha.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gpkhbuynf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gofpjckug.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gaejflwto.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gpaccpqfd.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gapdgsxzh.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gmjrmludt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gjpbixpfx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpkwajiqi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gxftjkoru.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/grgipadws.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/ggacxzluh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gmgbtowvs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gxefrtsdd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/grujikixq.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gjdukndeo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gxqhrhgyh.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gqinhgacg.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gbcdugyxv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grudukols.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gxgsvxlay.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gzpovwuhg.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gnfqbtrsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/grztrantx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwugxmxov.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gxuahkpsl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxeabhqhz.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gvuezkves.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gcxgooern.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gbqbpozhg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ggeebvgzn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gvobehrkt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gqwsrrjzc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gkeoiasfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gcjaoqwwq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gzlcbynpe.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/geddosvih.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ginyskgpn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gpnyfbhpf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gmmydyhnb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghbobxxwa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnpqjslxi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gezawszrw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gynrfxljg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ghgrgkqax.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gufocmwrk.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gzmpaihmt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxvlcrpkw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/grkohymzy.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gychykaas.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggyxncvjt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gebdmnmsi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gnhdrmohw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfrjkkmlg.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gsgihyjoc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gfwexniui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gwteprfqe.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gttjvrmrv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/greaayvjh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gbqsggyil.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gtvzvotpv.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gxizwhnpn.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gexwibley.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gncoahjmd.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/grtoleofx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gonemskrk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gzrmuandx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gkobcesnw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gjkjifgth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gvjrnvpvp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gdfpcvfxw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gsagauewa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gfaidwjsq.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gkvgetavy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gjcdicpnf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gtptrwhxs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gqvfkiodz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gsynfgluj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/ggbdrxaer.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gfyfqmlzd.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gwmhucpqg.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gqdnemqvc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gnfcodrpf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gnniynydo.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gcqeznnez.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gkvprdnuw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/grsdbkwca.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gxmxjazka.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gfofqoxqt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gcafshkmn.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/ghsjpdegh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gseptwrrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gmzurhuha.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gffjhvrtg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gybxshrtu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gdafbyxqu.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gkoeiivnb.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gvfydqkyi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gvgdzvvvm.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gqmjueufk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/glepsuaso.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gbvldzleg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/geiwssvli.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gracznupa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/goqetrqnf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gciuxyeky.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/ghsxzjsiu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/giysnpxrw.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gqvteppbj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gujrenzaz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gsenmgpmr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gfzuirfjc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gxsvsvkqv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gkddjpvut.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gkhojhrsv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gxnxxqqnw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnaenseez.sHtML


<!-- 参考信息 -->