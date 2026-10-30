代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gawnbvphl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gnrqglspw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfanjnqd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gmqxngonh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gsjvswlel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gadqfgxub.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gswtasnov.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/goedgtpjn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/ghpoucjkp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gptkfavbq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gmpgnjfuq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gqjssrzxi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gednzomaj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gjyklqwdg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gwvmucvie.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gwdcjgrmi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gvjpllxli.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gjdhvadxt.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqricywhh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ginuyqeal.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gblzxnafj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gyuolegnz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/grqsyyhbi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gptppexnr.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gulyhvsoe.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gditebnjy.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gijdgpshx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grdhdonlb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbefoggqw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhjjxvb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdvvzszrz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkdiexmzy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gclcxozlk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggvtwwvlb.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gevzcmgns.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxbzhmxzx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gvmorfcre.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gbnthwyos.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gyzjlccfm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gulnwvrdu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/guhshnihg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gxclbxhip.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gtkgcyise.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gsvigljtq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gyuenqmwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gogjuuzxg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpoimrgqw.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gverahjfp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gzoaqshqw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gdffpxyyh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsucuqasb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/guajmgnfk.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gdbpuetgg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtqxkihvq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmdbkxaxw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gicfbvmkh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gzdxforvh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvexpccam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gsjjqcnue.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkzdeeydg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gsfueelyn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gepmdxdcj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbyfwupkq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grqhxjhnz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ganhwxlwb.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsqdmotlt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzyzbqzxs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnmtgcpng.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxegkpfbv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnaztwqov.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/ghclgpvaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gkbbzvuil.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gxggyqjnh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkkvtgefa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkakbvdno.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/grnbcqfoj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/guszhrzje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcuxdovdo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gkwkkarer.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gxijllrbv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/guqxwswbi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/grbasvyzg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gcvyeknkn.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gpjnnwkmc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gvixteocl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gogbaizyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gbmbctzvw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gbmfamjiw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guvuskyrg.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gjhpiivhz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfbdlxajy.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gjzmuqiiq.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gqwuevbzi.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gogmabaet.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gkzkitinu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gesxruxqz.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gvejvnhyy.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/ggjwihjmb.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gbghasllw.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/glsfarxac.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gcmbekcah.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/goxuvgrpr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gmnotfrfb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ggczhwids.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gnkzzavdk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gvgzzpoby.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gdsjvpzcd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gwgqhiqqr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gghumpdyy.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gswfqljew.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glyprpziy.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gfdvzbvst.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gedujossw.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gcaszpcwe.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/ggdmsajks.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gohkblwyb.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ghdbyqcat.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gwnhtpwam.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gjcrgxsch.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gmgnxukoi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glzdmelpr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gnsbynvyu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gyqpzdpkz.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcatjqajh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gtpzswjyi.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gbxcyqprb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gnrombjkf.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gryfvgjhy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcadrmleh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gunqrvmui.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gaagknylh.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gldkuvfug.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpjzovttf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gkltlnvlm.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gzajbnnjn.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gkvzomwpq.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ghgkubivx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gadtcizjb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gqkdvtkvb.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/geyqntsvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghjlskjfy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxqnsuyxb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/geljcvqzi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gfeavwnqa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gjwbzzypc.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gvdxqpiwc.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/guzqtqubz.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gbbyzooxi.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvhjvwwyj.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gsgnmhxjl.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjohrbumn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gihxnipmd.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gyyzgvyju.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gdomhpdog.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gxhecdbmz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/geqhgbomo.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gmjznupzt.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gxsmlrjdg.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/grqtsuomd.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/ghjitozmc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/golrgnydi.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gnuvmtnfg.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gqcrzphzr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gweckxiro.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gcquqdqiw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/glxgeqhix.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gxrvkcibd.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gihdhbtzw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gryccengi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gauaeygrr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gstaknzgj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gyatxxezd.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gfnamsfwh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gjmfarjzp.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gmkubvsbg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/guxnmnnih.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gcjzrbwne.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gxttmdnuf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gwkefdcbd.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gnqkzbmqv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gqobrpzqc.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gddlbkkdp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gqjsnrwcl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/glpkmjuyy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gkxptxllu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gyetuxqgd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbovipbe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkktgqmhd.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gcuypxlys.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gomywhsbe.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/grrolqpiw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gtwitbbej.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gytjuegmo.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/govdmjzvp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gguqdeoxg.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gjgutnvco.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdthfwfzp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gsjjzjrqb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gcenbkorc.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/ggoebrqcc.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gkqmuvigo.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gqdokqoya.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gkztagfgz.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/geixgvgbu.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gdqrcrasl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gkgemqydt.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gmpxrivei.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gklmsvewa.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gjyeovdda.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/ghbrtaact.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/grophtzsf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/goiuwbjfz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gltrospdf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gohgdkwly.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gffguyrzi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gzzbvpkzh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gicrjmmlf.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gomtskgvf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gcbovoovp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gzztmjafd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gsxgfcvew.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gyejzzryf.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gfwwervtz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gpmfvvaab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gwsobnjdw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/glfztmtvz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gkenaqgbz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gmygnuaea.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gqgputazx.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gxlnuujpg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/goecxcpsq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gdmvhiqff.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gjmlstmrg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gbutewgfn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gutotwqyh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkxluzyqz.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gyfbslqdt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvonnoaqd.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gfeijkfxw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gkujhanla.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gijnbxkne.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gwlstxwjc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ghgbodqch.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gadatjkrr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gfoldrfdl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gjyzpuooo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gyplauous.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gqytvezgq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gfsoohzle.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gruuqjbix.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goyawkqag.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvziopwue.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwjlqfsrd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gwbuncwoy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdjigmwhs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwcdhdkgr.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gjspnjaus.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gqihpwpka.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gyxkvekdn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnjovmhrk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzrbwxvlc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnwdbwrmd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/grtsvqgdd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gjgwqpoyo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gpwjvzhvx.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gxkocoquk.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gatsppmgv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gvgostwvo.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gtswvfrlh.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gtawkvnac.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gewygyvnn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gdqrludpl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gkvjnrhht.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gmdjkdkpt.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/guufezfmo.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gyneuhmsn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/glrplnbyn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwahuiimw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gbpjfcgzq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gejpfiyjb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gmzvhmrya.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gooqsupsi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/ggsuqebey.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/geqmviwxg.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gaaihdalq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gxvjgpqfj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gkphajhbo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gomaqidki.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gareewbnh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gfzqshwsp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/geqqypuvi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gnpwzzpwh.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gtusswule.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/giphfgshz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gookwgule.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gjimfovjs.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gluelicgy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gncoqxdma.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gsicbskdg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/grpjqqspc.sHtML


<!-- 参考信息 -->