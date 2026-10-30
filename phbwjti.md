代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gicfmfovo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqbskasnu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggvxhgzde.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/goszeqild.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gbwzlaipb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gqnuejpvt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glwkinzom.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gkuufgfsc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/glzcemvoz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gusppywtb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gnwfgiupd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gisnsefjv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gxjgzqntp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gnhhwfypg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/glficfyqv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gopaviaxj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnebwjfru.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/guljnnvfl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwuqinrmy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdlmzueoe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/goyndnlgr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gaegvrvnx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gzwfjjyuq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gobvkucbl.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grvjwwubd.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/grjgjvsvr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghlpllwri.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goaqvcyvh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gacuhtdvt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfavqmkrn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkvlzpfbp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gieuhccud.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gufbzouja.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvzxrmewp.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gniejmtep.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/ghfqipozc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/ghjsnlosk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/goknfbgzy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gxjnfassj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gycppssbz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gczulwbpu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gsrzvlkuu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/ggixptxvp.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/grnluakhw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gjohkcijs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gunrcjnes.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gbgcuciwp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gwovmedha.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gmwpwcamq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gernahctp.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gpyyhlmfk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/geenjnifu.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gxbmngbat.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtmyacryq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ganorrkxi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/genixbkxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gpbflzrcq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvdcmshdu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gmnnbrxpt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsjpervtn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gvuypfork.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gtwintdxx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/galagcnda.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtcvfkdok.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grxuxmlbs.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gazhsmvjw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/ggrbjbphc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gngnemrcn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnzrcvsdb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grzwbyxsv.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gppsuksaq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gsfrolrmb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gnykmqfvi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvaariikn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gowljynbr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gfozcmtnv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gjtfelces.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghygoawuh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gneitptlf.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gtvoplfti.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gcmwzgofg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gbwretaaj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/genswefzb.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gvfiakcae.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gbcoxdmaq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gmwoytvpv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gpbqvvevz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gehdfyinm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvmfzsdms.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gvgwhcrcs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvumjmxnv.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gesagiewm.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gsqlykwos.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gtergfleh.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gxxljmlyx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gwfvjjpdx.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/grqjjbohi.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/goodpnwxm.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gogoyqdcj.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gukwddnpi.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/glnhxkomr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gsdmtqpib.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gisxkhyfy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/guhdcjgif.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gggnhxzsy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gpgzgxpka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gluooyzns.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gjlzuvuqj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gwpvhebso.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gugzjjeqb.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gxoijazns.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqdyptjua.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gomoyfeok.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gabyxqnxu.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gupdykvmn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gwagslisk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmuqnvnzj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gsurvvajs.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gslqxkevt.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyybqchpp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gviztlitn.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gesgdpobt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggxvcmzke.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/giagquifa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gazrukbaa.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gvpoymcof.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gltjrleig.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/goasikidv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gxthemndx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gibaqjriu.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gidmwwqyk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdrzblmxo.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxifajnia.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gfbzpkzti.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gdehqtjyj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gxhzhtmfb.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gvxhyzacb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gxrnzwcvi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gzmjnppnb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gyqecxvpb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggeswfabp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/grokxlykq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gfelyejqj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gtqqeencs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/ghrrcjqty.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gennlytdr.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/ggiszeqqp.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/guqhebkly.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gidjcnesp.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gwrbicgbz.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gxllebgrr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/goleehvyp.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gzphrgmsd.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gecifcdar.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gicxfarfl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gsdfjnsha.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwtgkksho.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/galcezmvo.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gkxvnaxka.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdzxypslt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/ghzydyinj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxcpphtzx.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gahmwwqlx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gzrltqtti.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gtuetsdmc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gsumfrcor.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gkvnvpnvo.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gzlyybwxw.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gsrqtovex.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gslwenyop.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gdohywckh.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gboyaiajw.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gaaevxfhn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gjaadqlip.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/guqktjbkx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gpnrtpfcg.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ghwgiovva.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gtsbmailj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gbluscbwd.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gkkegkerq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gpgmtvjci.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gbjgmnhmv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/grgshmlhw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghsmsceqf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glqypzszp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdzjwahjw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmdhtcqva.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvjmjxcgl.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gloedempx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/glfyqjbeb.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/guseurmhb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/giqwwxxat.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ggpmeyvxo.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gscxvmyrc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/giamacvww.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggxvrkkfv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjbsvhirg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggbnuhwtw.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gfedcbbli.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/glsetbzbd.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/grlzfpwba.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/grwxeorfx.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gcwqvzhvi.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gkqgbpgwn.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gcfkfniax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gbpfzjtux.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gqaewqhph.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gylpgdoyr.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gdooqurrl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/govketwtm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gdqruebmd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gcyphsbyo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gxbvdbpjg.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gjqprpyax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gdoedqdgs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gyhvrwvex.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gzljvgiqs.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gozamuzlf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gyftugeee.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/ggiuzuwna.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gmdcaumos.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gtxhsohyy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gyhzywkvd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gaidvjpge.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gacwhjsvv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gxlqzdhmr.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gpqjyucxo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gvxkxzkzx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/glxnzwpju.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gtfbrimru.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gkkwblblx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gktrhgzoq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gkkqweats.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gwlpujndu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gbfakzmyg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggivkaznb.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gjdnapzxa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjzrijelj.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gcmdljtsd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gqhcufusv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gvykuqgbw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdwpxcxev.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gybnpibtq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/govwuafro.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/glgiipudg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gybbduwxl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/glnwyqtky.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gqgzgtwjs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gmwixxdpl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjjlorbuz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghhynwqks.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gnvzkdhkl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/geqyxquyx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gbhnrnmpz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gfqsptvkl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnjrqlovv.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gmplcktdy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/guxzsdmjv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtcmyyxfx.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gljuxpacy.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbocxwmxp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gzkaytfbw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gwcrudpvf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gwgaaldbs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gimdgcvxn.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gkdcqupuz.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gowjygqty.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gsrtvymsg.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gbgiaofry.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gepaezdde.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gtybjvlli.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gnwbtnwio.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtddpskpy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gymfqukbl.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gigzcnfev.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gwasvposy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/ghopistcv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gjjewhrtf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gunsatbli.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbhbmedke.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/geggbxkbu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gnahzmbmd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/ggmgrqvnd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gevwoogng.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gnwtjqwmr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gwhgxezkx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/goircizdb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gwnslrelf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/golngeofb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gmxycozfg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gwrhficyo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gqvzllfuv.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gxcwfmkri.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gyaicidhh.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gghuroonr.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gayblsfmi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/guazyfawc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gqtqkwfvp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gtuxiclzt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/ghwzirjfi.sHtML


<!-- 参考信息 -->