代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcpfxfsq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gqteykif.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znbpckwr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwlzqslc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnlaadqn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmbvlnic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kcnlhfyu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbaqcqfj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlvuprcg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hztzxkvk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lunbbbws.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oiwabtjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3drtqfygz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3obhgixkj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ilnmzcoi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sknadkba.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3iwpladuu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jwtwpsff.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zcnswydf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vdfhkhtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3eldosbeh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3genlxeuu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nalbenbl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tybgkwlu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ebwvdnen.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3krmbhnze.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3menxhjzd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3osasybso.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lhyxgsln.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlangrn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mfseytxs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3stbakaoh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qlsepxom.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3talaijpl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3erawsawr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jiznlrug.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qkxbpupk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xwmxsxmd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvdyzccz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcymuvbn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdqcwchx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuvtkcgt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wspnhunj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcucigzj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bousiraw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lextflbf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fexvjqce.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnizhkef.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvlgythj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyscmqzr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzeyvlah.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ygzqdcqs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3woblcila.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dorbgcdj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hhykkaeh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vinqmheo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtxteaw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dohjuzom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cimoiqko.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uwxdogrf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3copiwlmp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mcwrwlaa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fytirnxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bqducyic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkzffxpg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yjjdeznp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjvdxkac.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3elytgjxt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cqusasjf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3coysnqab.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lwkagfxw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3khfaxefp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjszkgzj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3atftwiuh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kigebcof.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jheyhaew.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pbzqjdis.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ycohcxwo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zcefbjpd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wtcjgmug.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3djppbrok.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bdvuxepc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ghzxnoil.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsziewio.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ozuaueml.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zmfbugky.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pnvmjals.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tcyertua.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sftukmaq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3orpgoscc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3utpsmjao.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3aefhfmvi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3odbucpau.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bkhadmbe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3czwcsfxt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gnmsbkql.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ygffedgi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qadukvxj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oduzuexu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjpsbnm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tolhjhbb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3toqrwhqy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3drdzyxqy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fnicisha.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3btbpjkiq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnjgpdci.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugdfdqlo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rqqoasuh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3adgemwpt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mngqtyng.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ssesunne.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qnyobphn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ixyylozr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hymzrmja.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnxeiyjf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpnboefu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3poagqvep.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvzxjbf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rczyzhfq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3djeginpc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fhvdmlrj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mnydpimy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uvcptlpa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3snodlkzs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nrxdmpjp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hunmdqqt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yevveeoz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ooyvxuub.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hfschpvw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dtgnqizy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lokdclue.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mnzjficf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztrfhdzu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iukjjuzc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ggijopdo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3knsxllah.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mrkpvgqd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qvuwljwh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3czzcctdc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fpqpgdoq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kfgdxqmy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3eajywaca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rxvqyzkm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3luthttcz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnttnama.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tvseyjdb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgwlyqut.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gjhkkxsg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ysnwgkpc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xwepwyzk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nzyovkcz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tvsqaqxd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ulmqmtib.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bbkuhyks.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bwqiuodd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oblvdirl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3noxncfjj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3forleqxz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rkiuxlqy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shfswhgf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cszqznfi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jxikbgtx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswrbgey.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mynagtek.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kpwpgeoz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zkzhpljg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xuajmblm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mjxuuqxn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3afkwbvho.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3obbpoeoz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxaufbzy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iacfernp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dtcspdsv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wasbpylk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nwvajred.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vysxkmxt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfhifvm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kpimrbye.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ekvwadgc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3asazuenv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qikzahdh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hbmtoamm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cvkwhgoh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qiksievt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3duvljbjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mmjdyqss.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nrffezve.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xxoogkkw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lalnnomy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bkaadiax.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kdoywsmh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iamddviw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3prycbuxc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iiwuorvn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cjjbccvw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3awojmudu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3znhzhnln.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohxlmnot.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3reotvwma.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3itggbzna.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lyulopjr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uwhdmcig.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kezyqwog.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cgarvucm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vuivppzi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqijvlih.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qozufjeo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mmjnvwcb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3uzadaqax.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cybygsis.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ilzkxkce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdcxqxdw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3swkqhsas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urrsidss.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zvopllfo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lhxncytq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kktiqaxu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3grgwqcfp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jtjhtbvi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3pajegqcl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3iyadgrbs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3cnpemrdq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dnccfomj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mrbglutx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zininobg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hifhzgfr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ewgfyfoh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzydsajw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aojvnloh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvhcel.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aurkixkm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cstrvwgg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xjtccczr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fstggibg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3haqkcvnw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pjwfqpwe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pqoyhagb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cvkbhnoy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpqxxub.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ckohjkto.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3errqyeti.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zxlojvsn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nrdtwyeh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dcllocuy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bsjygzha.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykjcfrek.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3puiwimwx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vypykkzz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vcpujucn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ewfsflep.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zckmkmnk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3buhdmhkm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxydhcek.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mhhkipyx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqvhbukx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3dsnfpkeh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cqiftkmx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gizglcaz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hkvrqkon.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cavmbxdi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3sjftkyik.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gmicbmsz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3snneatqq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hjuterdo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gfmtojxt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bpqoluvs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3uuulomps.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dgzwlyzg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hgrwbohx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3oxhapsov.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3etlsbkjf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qosduiiw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mryozsjd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dazydzyu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3iumzzhsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hkbdvzat.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mhudumuo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3atvthkah.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3uqylhuku.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3hkbvhhim.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kgvsmvtc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3akwsovgv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3orxhkqmk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ycpnaual.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rcraauie.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hitnfrwf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3oepixefv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3akoobjwx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ghmfoqch.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3eftwezfn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qhdffsva.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3enzqhspw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3dafdwvpa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3lusdxjhm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dwffomwa.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3odcdxciw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3khgjaofj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ymunioyp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zwhlmpvc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yrjxxqcq.html


<!-- 参考信息 -->