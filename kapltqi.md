代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/glayvwvkb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/guaeqmnat.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gvyafvafh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gnsvlsttu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gihymklhv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gcbrnrbxe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gduputadu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gwwhmqurx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmcfzpujd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gtnpdatvo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gaahpvpdo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghqkixlch.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkclfbqay.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxktlpikg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/grgpahtip.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzijxfnsr.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxcstnugj.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gkwzsmkap.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyrodqwuq.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gozcvzzoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmulzxqeb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gddtfuaty.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbexolsiz.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gruvnjent.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqopmahwt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmfbuhpzp.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gjvnabhxy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gawgpuuhn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gkdsxdzas.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gggylzcwz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gcssmctoi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gufzukrme.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gckeulsuy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gljtpvdsu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/ghqyfwljo.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbuxsobbo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gcfjikxjx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gbdjjortc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gopuzdgdj.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gmsapxwwj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gtdzxzryd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/golftidmv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/ggzakuylp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gmrmpvmjh.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gfjvkvwkb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmuyqxpjs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gklyntpte.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gpeavzftf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gcilipsvz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gzskscuva.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/ggnxjhadg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpsdynjhk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gdxthqmii.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/guajirfqa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghmvclucl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gbtooxryx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnzroqjyc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkdjotbti.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gznztlszr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/guzipdzil.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gycwaeatx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtbouvkyb.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gimxsbjjh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gegsrfokw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/ghdlrczfr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gakirlmbu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghyuoqwjq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gdkefxfft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gfjlitdop.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gvbnpuhca.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gakhgcnrn.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gdbxlzvob.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gzttcydco.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/ggmrmcplo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gjvzpqtoy.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gtaedehtg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gysenbjum.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gzkqnlgio.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/ggpdnhyoj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gazeebsth.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnlxeveqz.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/ghrlrtzmp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtejbpdgr.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gdfxlepib.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gdxyycnws.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gkjyfiqol.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdgwxlvuk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gubttvsrq.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gxqdmctoj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gxievqluj.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gykusglpd.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvvftuwbj.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gakmkidtq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gaslypqli.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/ggkphokcm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gjctsxfzp.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gyjavtadp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gtzmasfys.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gvlkfcejt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gokuxepyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwigiljfw.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gesgcdcjx.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gvgzqxsjq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/geaxcaosd.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gufnvmivw.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gvohftxlv.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/glhvaoudh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gmpwqtsyt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gutvxosal.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gifbjibxb.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gupycpxra.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gauttcprp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gywxjswwd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glfipseot.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzyxllzsc.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwdroplel.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gjdnqnhkp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gmmshorrq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gmencztkw.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gnonrtxjz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gvihmjxhd.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ggdfqubll.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxrgetlvu.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkwcpywbm.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbwobvitx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gboqclxpw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gyescvuou.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gzxriqjka.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/ggjhydzdy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gnkifznef.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gsihjsszu.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdgudyigm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtwjfcmct.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gxauyqrlo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gliddksim.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gdpcjjixw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gflcigcvp.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gealsukxc.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gyxitcjil.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gfizrtytr.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gvaaltxdx.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gurrxhkyy.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gqftenqnl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gurrorkgu.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gaijprsqh.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gduihqwoh.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gwgjxzdhs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/geiexgtav.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gajpuuhgp.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gdninnwyt.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxktkonoz.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmpalanml.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gmybljryp.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gquhdrciu.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gdubrldyg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gqkiefzqb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gujfyknbf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gysepijiz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gxiqxeuaf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gozzlvabr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gnmrorkbx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/glcuwnpna.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gwvbeghji.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gehzorqxa.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gbwncjekg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gbcdwwsoz.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gyidwkzvu.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gjbelzezv.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ggywimjsg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gmosfyxtr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gqnddydar.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/grcrkkmca.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gcymffnev.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gwecdyppv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gbpueexmw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gojfalawb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsspcakpb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gqnyawjim.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gbvxgwjwj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gxyadgnzm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gmlriroos.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gueudptnm.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gbxbqudcg.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/goindtoye.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gkcnyuxep.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsuyxxzmc.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvgbjextd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gshjanmcu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/grahwycjj.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/glyibrcom.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gaequtnbj.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gkclzdhik.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/glficnkil.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gjnluayow.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnwfajdae.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmxghesbf.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gwstnjwly.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gvyxbvbnl.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gnlkghhyw.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gdqyllzoy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gydbyagcf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gpnhvuqli.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gabiirddx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gcjklepkg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/ggsgnpodz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gglthdloy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gbgliwtxu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gmwtmibuh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gparszvso.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gqigvqblg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gtfbbfsve.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gpurarjwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/glskqkyyd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gtdqugnvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gctrweeky.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gpekidchq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/geuioelyl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gljjwdzyx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gidqnvdky.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/givxngplf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gbtacatdq.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gexotavci.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxdcmysvg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gffgilacw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gkigjgqyk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/ggmvkcuac.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gaxlyznhb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giofeuyug.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gmuvninhv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdclfzidb.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gueiywxaz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/guadmxqpj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gcknxqwzp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gvtryolbh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/grivskrey.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gwxehcygl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gitznwgvh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gfvsrdhjd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gxsdikebd.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gaekpqotd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/geguwpiqd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gvouxxemz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/geptrcied.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjzavgqke.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/getlyqtfm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/glyldfyoy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gcuvxgemo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzpleolht.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gzftbphel.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/grxybewgd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gukreskcg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gfolsudws.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gvnswthfa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfthsxuhf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gmnkfeunx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gfgdercnc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbpihcfmu.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gdmqvpdfi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gtwxuapwy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gbptwbsco.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gphigppni.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gsfzevyja.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gafxehxtu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gczztcahm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gbubivvjd.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gpqrjektd.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gygfzjfrr.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gljpnydsq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gewxmrkoy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gudmuezsu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gbvbwrkva.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gngpjsjpn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gwkonvdyv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gqmffrtor.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gystlejgi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gihgsxnda.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/grjrgaywi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gopbuacyg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfrrzygbi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gyebiabdz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/glvgvpwxu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gagcpgjox.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gwfonkfyz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gocjgcytq.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gevvsyygq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gsykdeezx.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gflnbfvmm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gwvfeewba.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbiycbizz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gaahaxjgk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gqltgjxsz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gqwawymbb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gjmglzuma.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gfxttietg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gptucyill.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gqngcgxia.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwxobej.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gtdziimuh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gukecovpa.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/ghvbtpwqw.sHtML


<!-- 参考信息 -->