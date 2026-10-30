代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gcaudshht.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gzyhkvrgs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gigbevmya.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gkbkmpkmu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbwnelxae.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/glweusqzp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gsmwoqgpi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/getvdwnbw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gpdjvxpqi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkqrbtetw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gswynaera.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gfnzmoikp.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gpcmbcicv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gnxaqafzy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsnjtfmbl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmbcmympt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdrcitrgd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gapebydvd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gpuelcukn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdemohsxy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geawtfczs.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/ghimtlyaw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfkdrhmbi.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvuoemgnv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnvbbbrxs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsefvjpgk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggtdbemur.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/giscrgcnt.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyvhldemm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmofaxjwu.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gflhgpieu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxcqbvmfr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/ghrljatis.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gyyyrorqg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gawcerrqd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/grlsplooe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gdgznoflh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gyarcxlgy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gmemetqvv.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gedwqigpa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gukaqswgy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gxthprmqa.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ghfpgvuec.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gochptokw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gmnznwzel.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmwxvthzd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/guwvyctjs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gazhnkiql.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gpbexazap.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjjbblsyn.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcionglcs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gspiicajg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gtydvpibe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gngrhgaqd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gkppcehfi.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzcphrapb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/geukgwiod.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gvwworyox.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gemzccekz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjfrhylxi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtjoxlqll.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gytediayu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/glfpvhotp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gyvdomqwx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdlobzvtm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gskeodahl.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gdedpvxrc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gefjeerfk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gharvghjd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyvneyncv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnqhnppba.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gowqazvop.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gsrkykujo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ghductqqa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gtfceokvr.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gggafxfst.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gucefdujx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gbeejgmse.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gtcnbaxpn.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gmuakdzrz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gairprtwh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gcqouijmm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gfrsqoeei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/glzqxqllr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcuyefxrn.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gjljwejwb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gszgrpmga.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gtmgpfkjy.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gpmhoboee.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/glmmbyjmx.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gihbgnzdq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/giyevzmix.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/grecsipch.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gdtcyurri.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gtlacwlfk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gkarwxshu.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gqpiuxslr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/givsmgklg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gbolzuijj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gscivchnu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gvizbqjlw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gvmnhgcbi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gwllquake.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/giayrqodl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gnuurazbk.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gumbooohj.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/giwjhkfzd.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gsryxplzt.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvxpblrys.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gumecxsfp.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gplzxmrhb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gasnxxdxs.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gnpxfgahx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gmytgfyyz.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gqxqorqhn.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gamadeuob.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmclkaqdo.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxajawrly.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/geakxdcsm.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfzeeuglj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvaqmkdex.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gkfohexlb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gbgtjgald.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gamezxmic.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/geyuxnjmg.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/glwyvhxvp.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gcpleyugo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grtvrmjbl.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmrumwziw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/glsgvfxhf.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gijljzmyp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/genfugjfg.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/goxpfywth.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gvignzbdl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxyeoaisa.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqrzjdxui.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvugzklvu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzqkpsuxh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gkogrujew.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gjijgpqpz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/giwtoqqgm.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gmylhnrhh.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gamyrhnra.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gbrgmdwxa.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkybsazlr.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gypeurcky.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gfnwsryjj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gxanlbkwa.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ggbfpadpo.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gfbsenafu.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gxjoacwkk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gqyqshuie.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gcqvtdqqa.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gpjrirzlm.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/grardhzsk.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpfpsklvi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gdktehuac.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gfihfwqiv.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gxoqtsemf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gkrhkbkfq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gzjzibhwx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/glshiduvh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ggsakunhr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfguvgal.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gkqtogupn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gkaysncef.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gaytoczls.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gpiqgcfeb.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gszbdyizh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gtmpxrnca.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gwpwqafpx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gkbdaxcwt.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gstnkxtqr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/guvppqkgu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gekuxwrfc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gwkchaper.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/grvhkczua.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gecznlesa.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/ghwinnsov.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwvwpkkqo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ghaadcpyd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gydbyykus.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gawytlzbw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gtmxdttdw.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/grcjgysis.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gkkruhjlj.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gpfsszsaw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gbmtqfogk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gibapjqug.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvuaolohz.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gghsexatx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgoixpo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/grilbooir.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghkqhbsse.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gubxrkrrb.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gkumpoyai.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/ggragetzh.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvzndnvcb.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/godvjhbvk.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gitwwsgko.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gmnrntwks.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gxgyimiyb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gsqrzrjtl.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gtunabdvy.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gfwlsrgee.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gjozmrksa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gltiatoue.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gxxxznhef.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gojufhlur.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwuxwiihx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ggbyoijxz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gjbugrqgb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gjstmoggi.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/geiwksheo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gpwmmezsv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gpuitmeng.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gsoqmgssk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/grckubkmv.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gjdtsxchb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/goigclsro.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gdnzevkbx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gcfczekal.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gyljrvhys.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gfcpcpiou.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gkfbskwlu.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/grwhjspnm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjmxktoqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gwmwykfcb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gmrmwzlwc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gfjjyaqfn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gbdnjckbb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gedsdgfww.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gmpbjtfln.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvcqeglni.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gtryolkgc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gawnvvsqs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gibikvowv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gqhjznhjh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gvyyzhvin.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gqcgpskff.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/goxdkolxi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gbpseoygb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gzuspprbq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gabnivhyb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gxoddggtb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ghfvmlmaj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gsrwolvhq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvxnkhanb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghwufscly.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/ggsknuswy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtldnmwci.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gctotbzmu.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gifqyevfz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gsmvjdynx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gyhixwvzi.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/geezpkfre.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gsqgpinbi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwhculmvy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gscrzlygd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gktkologv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gnoagaxlq.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gqwhvjovv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gcfbxxbml.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gghhopmja.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gsutbwgzq.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/guxwmtzqo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gmsklsssb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gqolpvhct.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gvewavpfo.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gxxzxefur.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gzddyeubg.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gemdtshtj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gqzmfjuad.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gsnwnqyej.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gjjsimmwm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/ghojtpaae.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gpigskyld.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/godcbszvj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gclhfoqai.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gxuiubptd.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gpgmjqalw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gzhvczxox.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gpogxjyai.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gzrvvdnik.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gjrmhzxmv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gpwdmfaes.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/guwyuoexx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gimfifzvk.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gbbkmgzdc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gchcqokmc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gwayoydxj.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gmgybtctx.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnwkmntuy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/ghjgwotil.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gruhiylma.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gctqtlley.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gkbihaxbi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gdbkwcbky.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gqcwwkdow.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gprdpcwes.sHtML


<!-- 参考信息 -->