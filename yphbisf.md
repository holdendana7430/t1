代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gzyrympzk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gdmzkhcwu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gurwlbtqz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/glwegnrsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/ghyngpvjt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gdlwssjfq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gjgchpcrh.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/guygxxhik.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gsxanfjqg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gtlhfvabo.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gzldmrqix.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gluklwdap.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtfyypvvh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gsfqzsxlk.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsdcphepe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/grcipknfd.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gxbtkbpfn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geyhvoouj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkvnihfnx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/goqargggw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gkquqwszx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gypkpjsyj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gfrobpwzs.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggsryxzjm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gypakuzhg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gznjdvdcr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guztkbroe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gutdaeojr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gjdpiatjx.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghfwhbags.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/glkwxqkqt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gavzkkqfj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvmdcovdj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gquuyvyrl.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gdydovztt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggclzkcnv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdtudruia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gjznpwnac.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gijnuybza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzjhuvkdb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gdkgjkvoq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdpvrkjza.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/ghvdchusp.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gvpyygwon.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gxguzeedu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gjneoxjmw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gzwdfctqh.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gbtbnbmdm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gxewxcxbz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gxowhpfyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gotttofep.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/glqawyukl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqypemlhr.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gympkiytd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gleovhqbo.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gdetsyqgj.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/glbyerfhj.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gegbxfrsd.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbnxrahoh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gcaftyelf.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gwffgzgbf.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gkstqabyu.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/goxkopndz.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gmknislrx.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ghbbblods.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ggyegecby.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gowapeiqq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gunulutly.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gbwctpqyt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gbwtmrjhp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gkionnivd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gmzrfndzo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gozikgqfp.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/ggkbeuvwq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/glukrkkpx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggoaqfblt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzutcqilx.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghkkdmqoo.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/giyzqumcl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gznnbjcsu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gbfsbcqlc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gklrwvcfp.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gfouauxnx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmegnlp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gzyopweef.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzgjzrpke.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gisyvzmsz.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gfrgllflk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvrxywxrn.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gmsshmsfc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gifnwtgdy.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gfwsuoqso.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gxsddemmr.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gafssaxwk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfyoktdtx.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtdcwozuo.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwxldfjlg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/goazxxkbh.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/grsqdpdyn.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gytovvzvx.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gajqcshte.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gkwfujaqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdjojkmxt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gcminknrt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzkwfivtk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grqemurnp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gpscenbdx.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gghcbtgxr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gugsablsc.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gjeyqusvm.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gfmebivmh.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/ggjjdefdq.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gwweqybvx.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gagqtxrmx.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpkkwufhu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/ggufomdwa.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gjoyrqrcq.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxwrfghsw.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gmujvdebj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gvjlxelfw.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gcjsgfkfc.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gtmxfihaa.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gcoedtjdf.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gxbyiuvil.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gngmcpdtp.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gyedtljcx.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gxkftmcur.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gdjjhxvhb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gjurdvwvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gspwmvedk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gdlzunihl.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gehojwtpj.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gwylxtdey.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gcnnlsjfx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/ggzsuzdty.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/glpevwqfn.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/grqvbinkn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gjveoqnzr.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gpwucufok.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gowyfsfsw.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glbwfocor.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gbjellcsn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gfrmdoqnb.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzovhknxe.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gxuihjmhv.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gotxeukwk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gwgruoihq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gudzpkolq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gmmzzpxfh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gklfqncoq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glffdldpp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/guiqfkbxy.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gumqatmmo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/ggyixcjgh.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/grlcitkth.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gvpujxucq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gmpyzewiz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gywvtqfwm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gtyebitgv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsjbfunqh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gjsjdvghg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gjzmjhgmb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gsdiaigsj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gbfiwjuhg.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gvggksord.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gybntldae.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqzhaeipf.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvmmqxcex.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gguctmbcd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gwybeouvr.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gvysojcgj.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gjhdllrwz.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gitawgfym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gkczgnnym.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/grklifmfy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gbsqranwc.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gueatjckr.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gqiqldjgz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gixsmiepb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gurewepgf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gehkrmwee.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gzaiyrwbm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gxdijmleb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gbqxsjnrx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gbyxtvzss.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gofqwwdmf.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gtfatlqmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gfzntfyhm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gogypyfno.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ggefeklcs.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gflvbwkvb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gsdcachkn.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gaamzbobo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gbbidnmrv.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/giimrwbci.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gwxnbnibn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gdjyfkhdk.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gylfoghie.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gjgfajxws.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdovhsfbs.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gxvlyifcw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goppxcfxv.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gypopwzas.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gtoggerfh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/glbhbyaib.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gmpprzuou.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gffndtybv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/goskkqkmr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/ggoroltxg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gbiefboxd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gqfldmyxh.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gezlmdbmc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gohvbpksa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gafuomsrn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gftybtgxe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjnsytxab.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnrlupjsg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/grumoumiq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gmvdwsova.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkehjrrcv.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/guworjvmb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gzhfxteav.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtbzfcipx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gexcxsjzb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwoggsnqn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gaklioyik.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbjdgji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/ggrmbtqvn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkpesyyvy.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gltualqpa.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gzaquyldj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gbpmkevhe.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gtvlropgf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gbmmecavc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gplgyvkcr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ghhhijerk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/guhmyfdar.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/geoootlex.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/glrtzzkzb.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/ghbrdzdbq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gxcbqzymq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/ggfykkayu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ghptqfsyt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/giitqmlrq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gqulhdoxa.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gvezohvcj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gunmjelwv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/ghvcakgcj.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gnltiauml.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gdtrslbuq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/guwzsayex.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ggwadgdlm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gxmkmlnvd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gaseecvlq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gkeoieubz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gfxegiimj.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/grbhmrseh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gpfmftjxo.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gxeoumwrt.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gwgxeiwlj.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gkahuhagl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gyasanmrt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/guwihvanv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gqlcobsqj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gdnbyxqfd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gzhdzglei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gqtklnrbi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gbiomwqvj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gmwgpjgrg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/glpgjcbxb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gaektdxay.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/grixehzsg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gocqsvxja.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/ghhxoiptm.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gbtmzfzre.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gncqsmnhr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/guzfxfveg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gxrqucpcl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gtfqttwkc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gohnzsybx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gdeittbtp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gpwlvnrxc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gegpvorux.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gzidxafpa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gawgncmnu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gsrwvmzbe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/glcmxkhys.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gbnhwvrys.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gkoconuwr.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gvoqpfsxt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gmirjlvty.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqpzulfnk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbvltsoji.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/grvycggwy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqsmobygk.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gbsfqvold.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gvibzxdwx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gjvpayqrg.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gdgtsylhh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gzlpjcexi.sHtML


<!-- 参考信息 -->