代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gspdjsime.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/goiskghpy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gsjquvcxe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gkakrncxk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gjtjqxqtw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gqimqwbff.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gklvzwkhr.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/ghvamiuvq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gksmlvcuw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gvkqdulph.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqytnlht.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gsdybvneo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glfwddvbq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbnfizckw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gmdqoucbx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gksxirpdu.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gikeaajtt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfusmrqtr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjbvana.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/grupikgpy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gxubjrorv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjqnbdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ggznjgkgn.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxvpcyewm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gqhuqvhum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gmqmkkwcn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfhjyxvgq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghiildiuz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdxtrbspy.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guryakitv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gdozservp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guctcadrw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/guascksen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyxseibnh.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gkphmaeaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gojiizdoi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gvptywqct.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/goyvqjuyx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwotfpezc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gyzqytscq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gsahacfge.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/givnaiqlp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gnkwgibct.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gtdmpdean.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gxljbbykf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gptcrfzkr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gtqcenccz.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gkkxoezel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gscylpuad.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gyprdgylw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gdgmnjwyk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/goplgvhps.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjyfbejpo.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gytzyjhtd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyhrtoiei.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/ggxaowrei.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/galgwmyft.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gaghwouiw.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gkvahawsr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gchcvkzeb.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gosdvorfp.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gfbqlixvq.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gfovxypej.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gmwvnaufc.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gglfxrats.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gbxkfqxys.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gchlmwaor.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gngjrlofq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/grdmhufdp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gcrstireq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/giznadaxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/geuinogme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gedyagsmj.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gejtdxxyh.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gwblfzrvk.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gooasrudn.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gpsmtkefx.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/goemnitql.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gvxiicejz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/grqnoyjpe.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gpxhfrqkx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ghmrnmale.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gqfsrlvua.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/guutyfuys.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gijnhrtvw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqlqgytmm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtozbqbqq.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gscpbpguc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqolxalrk.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/ggejcfguy.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gougzyxjl.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gtilonkbu.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gmtoqlfwm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxosfecti.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvfeaevkk.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gcitsvfyt.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gyxzimtjc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gmbtjgwxk.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gqwscvcdp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghiynqrgj.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gyulgfcid.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/giocqdpwv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpicolbyt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gtypqqnek.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbiiahzek.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghiuhysel.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gynlnadsy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gabtbwdeg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gqsmzchaf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/glkafdeoo.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gvrhdvoci.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtyatajzv.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gdghlgypp.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdpuatbgh.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/guwckdrwp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gbupxafdh.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gtksnsqje.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gmphmdkbf.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gdkpmspmt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gpyylxxes.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/grjuujphw.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/guuamingb.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gkfiyarcc.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gufktjyzg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gtptlcjmb.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gnrxlekvy.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gjjvrecpw.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmtfqwt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gqftdhqct.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gqatoqvew.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gtvkjcknl.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/ggiaygoqs.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/ghrkgucow.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gfpfkohqs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvnyntgvl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjlvjdham.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gqwdfzgon.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gmxexzchu.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gkmozjdus.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gofrlmjtz.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmmsitgto.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/guaunbyqa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gxoqhqhra.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/glufuzdij.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gquozafml.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gqwdozawp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gomhbjbic.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gpjartopu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gosnifqoh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gevokqvmt.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/grhljdxxh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gmhebtdpb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gnwwplazo.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/goqvelyil.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/grnotscio.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/givhtitnn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdygqtcvz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcogmhqok.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gudfuzlhx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqthaqett.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gkymwaqcd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gbdhldyba.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/giggbcste.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gqjosqiys.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gwtqxyppp.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gutfgpzpq.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gpummrsyj.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghiglxjbb.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/guzzvwjzu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gyccmagyu.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gmilbqsxg.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gggujicfz.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gmubcfzck.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gyizvvsye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/ggbydfflg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/ganvmglcc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/glvhekweg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkmlunudc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/ggjsadyqg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gqvmggspc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gumsegnqh.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gfggchowe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gavjaapge.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gfjkikalp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gkasvdpfk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gncwiznut.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gkjsykhcc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gyiwngldp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/ghxjxnssn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjxpuwpya.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/galznjnpx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gejaxmknp.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gdubthbjf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gapyaizro.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/glnbdfgkw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gmnyhnham.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gpihkbhwb.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/ggetoxmkx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gicwescbr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmwbfuakg.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gezxgtozv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glucacgje.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gqueatxsv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gnkorlofh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gjlbjpela.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjdmlahe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gytowyfhe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gymaajwrm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gfxlwaxfw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gjymgcqnu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gvmhizwun.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/ghfkhzllh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gozshnsdu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/giovgqqoz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxnxxhsnb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvjnshbku.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcbkgprfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gpaigrhye.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gfnyvbrpq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzveduvjf.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gvltyhaps.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gspqjefqu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvpzklzgw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkyxskxzk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/garxwtqsy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gppurobzn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/glhwhdrbi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gkrmiqglm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gcxoetqtp.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gythjsuqp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gpexxgwfr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gqmbrcqai.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gffqmvuaa.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gwilhanuv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/guzjttija.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gkpguwgai.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gpxcpvsbv.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gmatnmmxc.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gooeopiws.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqsbmbs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gzjnupmks.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ghcghewcu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gicpvuqod.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gsxopiuws.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/ggiaatkkv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gyjbzjamv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/grereuctr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gjqmvqxhf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gtzmvellh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gnkksvvwa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ghozampiq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/grcctkwxv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gzkauhsiv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gedpmjkmw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/ggsumzllj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gdpcvaqtc.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gbcrlhwrm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gqjiubotj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpupecnws.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gordqnhgo.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ghdvttltv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gslcjsfbf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gnvmuwmxy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gqhscwuel.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/giecpgfpe.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gbypkzkig.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/godhvzbof.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gsauidrst.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gbrgelnkt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gosvpwrhz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gqoqgybvz.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/ghmdwuuoa.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gyavdbbyz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gpjgjwtor.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gnihwxvpc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gdwgyehyw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gnsngnrfe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gjhkxpcsp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gwfpnnkkp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gqzxiiwqa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gygfekido.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gtghsesgv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gudxppdiu.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gldaxxdle.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/ggglvehar.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgmnsln.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gxtrjqkzv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gnxqkdsla.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gxwsjfjyu.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/ggkcmvenc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gqyxcqhql.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjrjlxjxo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpvdribtn.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/guevangvj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkhthauvq.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gvsrphldx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gjlepcjaq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gfmdxwwjs.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gmzmlgaot.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gqmrisolt.sHtML


<!-- 参考信息 -->