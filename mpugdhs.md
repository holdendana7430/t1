代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjdmzlyz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/genodoyzp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuurlymp.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbyrfbie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gunuyehok.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/gbhncugja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gkfzrdute.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqowhvmra.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxznfaac.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gchewtaul.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfjgyknj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhrfdrea.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoftcudn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gepurquyu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gcbqbjouw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gemuhlfho.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgpvsnow.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/ggdjagtzi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gjfpffhxp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gayfqggtg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtblbiphz.sHtML

[F06] 删除文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gusjsqhbp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqvnhxzvu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/glzjpynvv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqprhkhuf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grexjaokw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbburjqpq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqbfbbmm.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbstygvbc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ggbmgihen.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/gesbbzcra.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrnsqtns.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjyxofsv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gciqvprwb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gjslkualt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gieooxtzb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpxyomqk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gacmcterk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvqqmimv.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gakdgwmqr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqcyzzip.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/grrffrcsg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsilkjlib.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gciorbelw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/glspuovhv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gtkkjvhsi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvduqmtop.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdwkyoml.sHtML

[F09] 获取文件大小
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmxzytii.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjdzarh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gstwpxmbd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyigfrrzw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gcdcxioao.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gbtnkjdkd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fanxiaobao.xyz/Article/details/gepacttdc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsqdvubda.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvplaxfo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaoilstp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjbkalbtu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmooaatk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gremfdwaw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfjnrcbe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gphqhiblj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gddvidtap.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnyzfjoew.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gibpohepk.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqxsyzka.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrnmmrml.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftrbaqkm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/getfsdvqm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gbmjihlap.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gbshjnxhk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gaugokfsy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydeqhzlw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fanxiaobao.xyz/Article/details/gwaboomji.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/grcamsyve.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/gyjcqrnyh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gxnkonhqa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyfjerys.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gckhdodnd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzhuicxx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gsppjvrbo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gptctehzj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gadhwvcdi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grogxyerp.sHtML

G. 面向对象
来源：http://wap.fanxiaobao.xyz/Article/details/gxhawjzzs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glacvjxvc.sHtML

[G01] 定义类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpohynvau.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeybterk.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuvgdgsp.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmxbunpq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeudqvdj.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwobjzkmj.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gnofedfho.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gmcatvfci.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyvdzbdgd.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glngraxqi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/goarqvlym.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxunwioyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxrjumml.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrbhkfdh.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjcedhgcc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqwsvfnd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfirhdpkt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmqoolvd.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gnodquqsa.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpoozyfm.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gosfhtjri.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gehzlfopf.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdejxxz.sHtML

Java: private String name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqypsbxi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/galvykubh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpdcusva.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpxpipms.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gzfwluhgg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gmvclymcb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytjznzje.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggdljbxo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxpsaefz.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpxjnnqd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpnexiwk.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/glhmtvgfq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gypsipgwp.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvzwqoss.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlnbotds.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmbxkpiwu.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjuamdcyn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsoloier.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwlfhuac.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fanxiaobao.xyz/Article/details/glnteawgf.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvephdfz.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfozvvntt.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjccjbsbp.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/gryhsfwus.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggzvhnzrc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghabscqfx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvjgywbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbqogcbvn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrkxdffn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/gjqsuihyv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsictwbgo.sHtML

[G07] 调用父类方法
来源：http://read.share.fanxiaobao.xyz/Article/details/glcgwtotd.sHtML

Py:   super().greet()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeqqzynu.sHtML

PHP:  parent::greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuscfulm.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gvmkbhpnq.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/grlglwczz.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/guqataglp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fanxiaobao.xyz/Article/details/gpmncqcsl.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/gaxsgimck.sHtML

C#:   base.Greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoezcndw.sHtML

[G08] 静态方法与属性
来源：http://mobile.fanxiaobao.xyz/Article/details/guamrdzfa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyeznapk.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfvyonx.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gingueqbz.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfrapyocv.sHtML

Java: static void f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqljyoxan.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fanxiaobao.xyz/Article/details/giifmdeaa.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhothynu.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtkexvxbs.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdcscvkm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/gmycfjiik.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkupueciu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/grjlnothu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fanxiaobao.xyz/Article/details/gncjmedgu.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabolumbi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gesccjltx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjakalajz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfxbtqt.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwnyqbal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzoxlrrk.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwugrwus.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/glqruzxmv.sHtML

TS:   public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyifkvnq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzdfgman.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkgrrvlp.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gtovvutul.sHtML

C#:   public / protected / private / internal
来源：http://wap.fanxiaobao.xyz/Article/details/gwxncuncc.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgnygjma.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fanxiaobao.xyz/Article/details/ggmnozbsp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glodyjqto.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfncggmpa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsbvgheys.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/givcujhqu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsaafjze.sHtML

Ruby: attr_accessor :name
来源：http://3g.fanxiaobao.xyz/Article/details/gdyzgodil.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtbsjmwfk.sHtML

[G12] 对象转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhjtqrxq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnusisqv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goshkkwle.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdhvvvwcl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeycdald.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijntiyvt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsyixjxq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gwwhretyp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmnxiajf.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghejnerwo.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gbfmeopra.sHtML

PHP:  $u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlhxfscb.sHtML

JS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gbugoiwmz.sHtML

TS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkmnbxf.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gfsfcjdfv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzxqffuy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/glgommsgp.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/glurhllxx.sHtML

[G14] 数据类 / record
来源：http://m.share.fanxiaobao.xyz/Article/details/gwemhdbtf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrarbipv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gohousphr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsnetbta.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/gjorxjuzu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxjszmijp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/ghkynyica.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gyphsaeab.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnfieiw.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgbtpwtj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwfqopld.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvjdsof.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbldwzsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garsghqfe.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gnkaevujw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gmruqnaiq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/govxsrtif.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqbphzaml.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fanxiaobao.xyz/Article/details/gjejlxirt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfyuyyyy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlrygtsj.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gyjrpjsnk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gsuwfaydx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssfzoidy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/ggamtlotz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbcockj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gbjiqjslq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhnujpeo.sHtML

H. 异常与错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmhjvvwk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdyqcuer.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvchspgp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaniggxk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gglpqavye.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfructcbn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcebcaij.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxtdklzx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gauytlmeq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvagshpk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkqboonp.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/gbkhgiibg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gajgraunb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpyuflvjz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/guniakxii.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gesxjiznd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpemgqag.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guphatpci.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/glevdczql.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gympmhsqp.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhuvfrmu.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fanxiaobao.xyz/Article/details/gplesmchs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/ghlhjeucp.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gtgyteauj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfkxnvmt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gxopustul.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/godaofsha.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fanxiaobao.xyz/Article/details/glojdulke.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyksvgqtt.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigcowfef.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsavuepc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlzjpztt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbvwwyhr.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoiinqxh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhmsszt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzxzlvjp.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzhogne.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggexwcnfx.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvftjimwf.sHtML

Py:   except ValueError as e:
来源：http://3g.fanxiaobao.xyz/Article/details/gnnyitcjd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfsiaij.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grinosvyx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpjugoryj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyzbtiudw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzhcesiy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gypeqmonh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrrkiwru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmokqlogy.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gexxgcxvg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/grldxugxr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizlrnkyp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/geswjlwka.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjnnfmah.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/glprrosji.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcshvpsa.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gsdmjctio.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/gdndgaayx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwspzntv.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscggfssi.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvijwjmc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/grjvchitq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghipgobac.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdvctxoi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gwifcbrxu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfxmoitl.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gouooqgrd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhvzurg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fanxiaobao.xyz/Article/details/gkryvddxk.sHtML


<!-- 参考信息 -->