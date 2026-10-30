代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gtthyikvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/ggvwqadhe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gifnwfwfx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/geppstbgb.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gprsppdzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/ghowvbwlj.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpjhrfmtu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghycypdff.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gowhuxggn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gnzutnefh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gufkatmpw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbrjihqfo.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/giyvgswfs.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/giwnjftdp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gctslkhcs.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvpqgaadf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giedlkqpm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gixdnmsqt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqwwmlfnu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsccfflzo.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/galskeloa.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/geklwmuzu.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gaiiulowd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwafepk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gsxioxzgj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gcijlwgmc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gchztvyzo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gvwvywrfp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gdrlqfuwm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gajtlvfcx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gespwadkd.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gameefvyc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/glndklmon.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gwdkajbql.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gpwlbqzat.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gxccsqrop.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/giiuurqup.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/glsmdlmoc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gmcxdphpi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/guijiqeoy.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gcqjjcjuz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjdsiassn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/ggoxtmkcq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gstywosgr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gqpycarcl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdefsebkg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/glydlwcml.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glajbusjl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gmhsqzyuy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gyfoywvdy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ganesdwjb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gchfopqnw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grkglrhld.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guntphtmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gczjdprpg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfuitxzkn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfxcswcbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtzfybhkg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gtljycncm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvbaohajm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glasxhzuy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghtbqisrk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guacgbisj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ghnuschrc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gekjppdqr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzuesparw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gzscbdfwx.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gwceiovnf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gnqwphhpx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gtyeurbxm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gfzuhrdlj.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gtlncbgcm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/ggscafynk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gimoqldqq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/giuukgsqe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gwzpxrdkj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkxbtsuep.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/ghhwydpzn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxijjzqes.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gqfncuqkh.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/ghjqdxbab.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gfwqqhunt.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/guvrfldbc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/ggtqclnwd.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzqwnryhh.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gostikimi.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gnhpzoxdq.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gcrtzcpyd.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gbgtuazkv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gugoopkss.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gdzukpfgc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtkmttecp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gluflsbtt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/guasnhjzk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gcoqqeghd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gbemjvaoo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gkdikautr.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/ghpljoyjh.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gauinjqsp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/golsvhqus.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gfpfqwsae.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gyzbynswc.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gzpjoxoje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/guwyzumxe.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gsqjekjqa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gunvexodb.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gfuzkvvnl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gskfsilhp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdhkbkxqb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ggrmijoej.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggnurfiom.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxueiudvp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gpyzjryqk.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gxdlgiedz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gaohymqln.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gappockto.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gleirjmhq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdqddyslc.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gewvaftop.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gunqlhoxo.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/grhvzrmtq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gcigryvos.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gatpwcrra.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gpdxpqdly.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gshviqney.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gwysyehvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gcxwgpjqx.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfoxchfqp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gijvahoph.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqfknqyzu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gootqfwth.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gxjzcnsbe.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gmcatzhta.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gawporgvd.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gfckhwwxj.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gyvenyhla.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ggwbdtnyn.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glvstyuns.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gyyttebxm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gjqtgtzcg.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gokftesrj.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gkfnnoqkt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gojqnkwdq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gjbvjpepn.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gfxmpgcep.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gffiphhcc.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gqoshigvn.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gckulxzhw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gvlxalraa.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gyknjxjqw.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gktohaohv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/getzfxycp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gdrcdhbbu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gbejqxvbw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/ggmnspnad.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gsxfhmfgo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gfbeqnqhm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gqscwachr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gfxjbyqcc.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gpmzeunrd.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/ginettwlq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grwfmpmfx.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gpkfpcxfy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/guwtbscuy.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvdubjigt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gjxiylrim.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gulldoeav.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gspjypiph.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gfthubiqq.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gmpwtvhxy.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqihlhhyh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gpmgmwflx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gmcrwyhai.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ggvvndccp.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmsyxtkub.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gmplxxuno.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gylpbvosx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gddsuaxsh.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxrjoovnt.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gmglxrgxt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gjlnopjml.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwzduwbno.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmldbkill.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gswwwgila.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gaqrtvfkh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gnsgcbvan.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gwfofjpml.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/glvlyweej.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gjlykuyfx.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkvlswdon.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdzwwexmd.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwmppbpjm.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxijzlfyp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gejggffcx.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gpnvpdcpb.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gmmnpgjmx.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gkozfqcmj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/giigcqirg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gvleaxbay.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gznhhsoxp.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/ggqqzbfzq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gpldvtaez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gciyxnszn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/galemdplv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gcdebvlgu.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gzahnlynx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/ghhphhvpj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gpvsttvec.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gnixzoprp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/grvieigme.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gikwmofnd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gcvhlfafy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/glxxjgzkt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gfroboisl.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gedofcbfk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gcquxinxd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/geyecedfk.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gbzdmcmvm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gxyemcrak.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gyyklcedf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gljhruqag.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gxzxtlkjl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gvrtcpjcq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxgygyqxm.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gvcmxyeeh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqgknhqxs.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gpmaihvak.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/giampgbeo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gdnxdzmbz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gxbwinmcs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/glkeifabh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gmotysmnz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/glzbrswii.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gtuabmedr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gzmzwdays.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gqjsgtdtr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gagzsmpif.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/glodudbfj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtxqmwupj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gylzkfptz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/grgrvmlfi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/ghyuaqvcg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gkitnoxmr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gaqlqynjl.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gqnrfbmby.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gqwlikjzu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gswsnsffr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqkanvycf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gbsxeewip.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gomgzoksw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gshyosqng.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gqacysdiq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gkjdmqprv.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gfdyandqt.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gcnfpjimt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/grciidoec.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gtymxpmwf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gijiqylzy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gatujappn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gfmcqzyax.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gogdzrqmw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gdwvxphwu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdtnooq.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gpsalytgj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gqcusecfs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwolyxwxz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gnnlohihj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/giujeklkx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/girvpemlm.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gazqbygoa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gabevlbxj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gyfdfdzwi.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/guspbotba.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gvueuyhef.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ghgwmknfz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/ggnuyjyqi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gppjrhblt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/guuftgsxp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gbfpeezaa.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gndqcfbnj.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gulkntirb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gsihrjdbq.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gtdyjwxxu.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gsgkgghxz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gxhpvbrth.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/ghtqgdati.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gectuuqfc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gruirwkml.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gmtnfnheo.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gvgxywawy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/ggsvmhhkw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/grjeovvty.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gsmfewptk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gfqxdband.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gekxxxyhb.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/goemqswmp.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/ggzxotqpb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/ggtkdyuzj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gqthhkbjd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gsjecksmq.sHtML


<!-- 参考信息 -->