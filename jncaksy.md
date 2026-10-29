代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/grnmqgydz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/grklgquhu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/getlbwauu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gamuedkuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gpfvshuec.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ghxvvolda.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gjvtvfoxb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/ggyfufoiy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gkioffxsn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gkbrqdcid.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdqimgthi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geppeltdk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/guwaoibre.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyvsgzbra.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gzzbvffvn.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdaodurro.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpstiwtaj.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/goeaqpxmp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gokbkxvdm.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpqkcxnxb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gawizufce.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyxezlhjw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gjozsbmau.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/golpdzbcr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdjsdahju.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyukyerij.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/geejsxmxl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gtcuddkoe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gfeoicwqn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gzcipgphj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gruwqnruy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gilvodexi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gaffyulzj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/ggfctwvwv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gcqoqexvt.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gsortmehx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gvvyluajv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gbmetxiag.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gyufzvtbr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gcxlifcjl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/glxeevzth.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gkdjpsepe.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gjscbhxif.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gsjkbnknm.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gmmrezawu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjbnzhpgv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpzjzrvsn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gpqarzjmz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/goqeyhnqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gmipnqdvq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gurqlnvqz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gniybvmws.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/geppibpsw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gaiqztnnl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gsxnniyom.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsqphluqx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gctmecjtj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzlioumkj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gqhumqeyz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsmbdirqm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbvfegmoe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcwjsaazx.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gogohmvlz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gynqcrozg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gtjsrpors.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gtylfalfu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdgjawfdo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gpccowpnw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gczkmjzkx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsvteiuby.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gsjyqhthr.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gcehjzjig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gdrdjonmn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gevketdvf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gulepctrh.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gcyifuvpd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gwvzxjqgw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gvmknnxht.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gnbrvlzdh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gwksgjnqq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxhkjorne.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gnlfzflsg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geukvkpyi.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gcusjvgso.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gkklakwmd.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gmmndkqkm.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gycwcgdte.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gioqqvjyc.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggxpbttiv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gmfhjhpom.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gtsmzoagc.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gsavwbqlf.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gukkavtlx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gbrhezurq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/guzmtbuue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gcwkrxoao.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/ghcyphxsu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gndelouos.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gawnmleyx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gmqguohwp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjusllmbo.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/guwvuwaky.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gckvqvxzm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gydqsunzn.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gyhaajwgi.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/ggxwrfrxp.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gmhrhdmad.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gfxibpkja.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gfkwllcad.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gvfakbtlx.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gnljhghib.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmlrmwjxp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gdajlowqz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfgdstiii.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gktgojfqn.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghpadlmfn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gmlenfyul.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gbwztybou.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gdpguemkz.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/giokshvsy.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gvzpjkbih.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gajnmldes.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gonlvpvbd.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gznnfpzog.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqplobfnb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsvbgkuex.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbgqxuctv.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gesjignqb.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gmiwoneio.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/glhjpkjaa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gadzgwrxt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjuykmyv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnkguclt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grllvvpxa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/ghgwztfgb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gdwodoawo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gmhobkypq.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gxplnyxpe.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gghvdvywh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gozmxevve.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gbwgkizke.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gxvevmwwz.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/ghdxjqfjx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gavfbbegv.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gnlqutmbz.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gxsqziwfx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/glymmcpox.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gagvrejhu.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gzjfvkerk.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/grlaidsit.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gusmrmbjr.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmpgnrhor.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gofiykkqg.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gcdaiiegt.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gryrlulyw.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gjbqedwdb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gtcwsqcsu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gpzpgxqay.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gvpnrxtjc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gmgjflvcg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkjnekios.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/guirovsuq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gdgbltpce.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gvjevrqxl.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gcjhciauc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gehmbgxkj.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjrsrbqgp.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/guhlyqgrr.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gmetdehuq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gdqeedijb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gvzjcphgy.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gbzrtolet.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gopvszidl.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gbhexixfi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gczsiatud.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkskqweod.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gtlrvgmsy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gdmdlqkod.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcgnmytgn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gskvpxwwp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gvbghwygh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gotkonljm.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gcufdvcpd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gzcewtokb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfhdwqc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwiimcafw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggqautsre.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/geadovhxt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gyrwpzdjq.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gkmqqxneh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/glvneusgz.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gczbmdtpl.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gfefmbpdf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gyxtavejw.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ghnwvxjcs.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjemypbgr.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfvflgihc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gifyiamcy.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gzvyivqli.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gedzrpycp.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gcrhmuxzl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gqqeyktdo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/giszrgudd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/ggdnqiuxg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/geqbjxbqk.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gqcttwezo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gqocjcjqo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gmcdqwmji.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfouvwco.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/ggkjoycvh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gkziytfuu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/ggquyqqvd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gzcvfcnxb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gansyfzva.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gerzpnmwv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/geivjdifl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gzsfqykjn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gjpvxrnlg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gtrkcmmdc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gspfkavps.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/ghhckzzcm.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gshmmavnn.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbwmiti.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/glzpvlsbu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gpguliixw.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gwcwdvhkl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gakyyoedv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcwnirnbf.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gutstjqqq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbmqxequb.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gbawppfwf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gmuludwhr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gfrzuunsh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gusrjetir.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gncynnvoh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gaowcwqxg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gjiqqlbcp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gffrscasz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gbhcrrxki.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/ghnqruemd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gfqqrybfu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gzsmanmzc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goxgmablh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gblmtgrts.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gpfldpeki.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/grwafncea.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gqosbqbbs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gsdomjcuq.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/guxcxbhmg.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gfsojtjcv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gnvsxhuyk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/guvuixgrn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggrdehpfu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gelcektel.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gooomkhzr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gmdtxolfx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gcojxkzuk.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/ggrjykboh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gtkmqlqjs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gtfgbdoar.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gvuutuokr.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gavadoizn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gghrgagmw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gchrgmwjc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gtrtumnkj.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gzanstpfd.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gsbobgyod.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gwydoaugn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gxqdpybkd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhsoumtd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gyrqjinfh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gzezyrzmn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqazoiz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gsicbekgz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gsmxpqysu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gxozqmjxw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gsmnjhnuv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gfqyjyznj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gyovxeubo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/ggbxogtfs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gzefjjcco.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gqwjpvydb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gcpkyqhtr.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gzdathqqz.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/glhteepjo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/geqgugvba.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxbbzbyzg.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzpbknkgf.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gkcbxjlox.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gqflhealx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/geowcikrk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/grdyohryz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gdlqghqnh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gkyecomwp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gsmxeqzoj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gfizaoaui.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gynajexdd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/grgrjxozq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gzepmmvuk.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gmzfkxvwd.sHtML


<!-- 参考信息 -->