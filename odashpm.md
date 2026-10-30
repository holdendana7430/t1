代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gjenjqruz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gdutnghjc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqnwedmmx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsfjgllum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/girbqojxg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmjdqcmeo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gdnbasvel.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gztrgohtl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gridvqhrc.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gecdoyvhc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/graowaepr.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfqcweaoo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gldzvjido.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grkdrhiio.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghqomkwcl.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gureikotj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwxisfbix.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpvufqlbv.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gvhwedlzd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gpcydpbkx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gschamycf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/ggwlsynar.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/geiduypcw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gefarnesz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gwfekeres.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gdtzfkdqt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gucfewrja.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gvbcysiyy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gqshodhzg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/geuukdyae.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtoszlmyk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gxijdhlqu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gckoopedz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ggexwvxig.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxhgikhfp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gehdqosfu.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gvfrhfhcc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gphehwfqu.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnttgjptf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdqbukmod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gybwtsvmb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvsxyzzbv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ggngsysik.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gspopgeyu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gjflmvefh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gbpnieplx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmiyqngub.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtsjvfrtu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjgdgryhn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggrugsfci.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gyjhtkmfo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grckltzzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gasgudlrv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmcfbhgfp.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gdnyovamn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gyqugspnq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gopzjcoxv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqpofodfz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gscazpsgo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdoteuedl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gresfikvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzhqgusic.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gvkagagzo.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gpckgvteh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gxnalkush.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gbyqgmjri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gdukpjrkw.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gbggpvlng.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gyubzhhqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/golvfzuwf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gjvsrvkdb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gxpvupqjt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gocdtvzvx.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gcmpuuamr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxfhflznl.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gmhfmbgbx.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gfokkuhac.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/geljeljqi.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gdbfbbggd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gsthwvuxp.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gifyongcp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gjteqowvq.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/glhmbvfnw.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbonahzni.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/glpuyyqjn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gduebhnmd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gagucouwb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gpvjieytz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/ghbtcrpix.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjksamll.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gksjqdkkh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gcfmxgiwa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gvnmopyxk.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/goxuokkht.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gahpjjgsd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnkazszdn.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gatcdqgrt.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gacgcaofm.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gtvzqoapd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/giyzlnbxx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gvheykxsi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gmiyzqfuk.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/ggefsiaol.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/geqyhsxyv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnprcqtvj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/godagsdqw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gsuuxmcsg.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/grbrfzkct.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gbyiwotpt.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxunyhtwc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gbjlncrzw.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/goazjlmox.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gfajjwsgi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gqhtspyiz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gaxxxlods.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkobsdlvd.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdgnvgqpk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gsosxekqp.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gdwnombtg.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gfqhggduu.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/glcomzshs.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gnxltjdms.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvtaafebl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfwdgxjqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcweivhwy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkfummvw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gsnqzkvqt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gelscitjr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gvcfteasi.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/ghelgtkua.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gbzdgunvw.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gdfksjdyo.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gucidocjz.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/glszuypos.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gvqddqpck.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/giplhfnka.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/govfftmjm.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gmpoaxqwx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gslhuwbyw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/giqkekhjz.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gemccwvud.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbaazciu.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/ggwrrlacn.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gkziikfrt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gtasgyqcc.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gptilptbi.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gjowrsakw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gxsvpfskl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gbiqxjdfb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gvsolenps.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gwfhxlebx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gekrfdwwa.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gnyjesdee.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gmdtfrcfd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gtqaxyszp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gzywbvhjx.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ganxoslhy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gjblavkru.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwdhvnads.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gxilagknf.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gasmyciym.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gdvhhadjw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gyxqiiukc.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gzmpakhck.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gvpqvmnvt.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gqrgfnmtd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ggzrkusnp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/guarmktwi.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ggcrahzgh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gxyhpgddl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/giwgjmyuh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gddvlfnsb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gtoxkjlbp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gnlywzkzq.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gdhwahvvm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gumayldam.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghyjqcupe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gryqazahz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggytffizd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyxqkivxu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ggviicjiv.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gfqjapopk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/grjwfmwjl.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gkmwfwvdz.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gtwdrsxrb.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gedrypqnl.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsckqrove.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpqjzaxvq.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwahisehi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/glehmpfvh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gnpwbqzyv.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gzoebyvuc.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gjuduwqwm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gaiyrdozs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gtgxtsldl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gojytrvct.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gycxnwoeu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/giuhvqxyo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gikedulmg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/geubjwrcs.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gathsnhra.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gyejabmcc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gssyvemhx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/ganrcdhrj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gqmlwquvc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/ggopilekg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/guohmijlm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gmyxwocqz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gcyzooksb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/geqmepklj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gprqkqbxl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gaxnrphxf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gygswugtm.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpngcdgek.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ghslitmng.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gfltugpco.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gxrdjclnf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/ggehxqmul.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gmgmashqc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtfslptjs.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gkdyufzni.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcfxcsyea.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gbxeldaty.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/ghkqbzhca.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gfqjdbbkg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gguozridk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gjdfotzaa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gnfrjmfay.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gcfjbklkf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/govtolhlk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gmjlkikbj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gieozzdqf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/glbjxavnm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gxcahmqrt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gngamowpk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gcujasaxg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/glfofwqbq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gdjjqxijy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gehoenpdx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gusvzrujs.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwbvxgjmd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gugswwlee.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfsztaktx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gncpegruq.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gthvaezjv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghlfvspfo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgowzllw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gibyadlpe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gnjovcntj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gdsyvrrpk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/ggtivtegr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gyggjswwb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gnfzkhpdc.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gcrlslmid.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gghpvejhs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gmdeydkzr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gwpeiqaaq.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/guxjkeovf.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gmuuqhzmt.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gxhsuodwb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gxdjqbteq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gzfqjdivf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gpmoybhvy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/grgwmcorv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gwigxmgjl.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gecqdfncj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gjnozfeny.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gvcwrywng.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gppkabmmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gpiaylfdw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gxuuvbbkt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gpdiqlbfk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/ghpqrbukk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gaxceoiyj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gaonfvymc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gyjuvutaz.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gbogdbwqw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gjwxlyhjb.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gqkefjdwk.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkgdazgcv.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gtiuvomfx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gpnicjbrx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/ggvxpcqkf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gbfwyadlk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gfpiedsws.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gnrpnbnzr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gzuvhumzb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gcyhqtjzo.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gdaqnbfdk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gzfmcmnot.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gksfxylif.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gysltxubf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gjyjcafaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/grkrybuvd.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gococepzv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gzhwlodpy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gffihhgww.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gfnkdeebk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gvjotirix.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gjvbmbspr.sHtML


<!-- 参考信息 -->