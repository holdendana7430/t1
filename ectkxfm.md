代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gygatyxuy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gihgvekgh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gwifkemqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gvvmjvozc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gpqqbalss.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gpepapntv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gcyhvxsdt.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gbcypziqt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gqczrjwsw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/glahsojhy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gsuiziqrr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/guwyxounq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gwefbxyow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gagivfsok.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gxcqqvuqy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/ggeawikaq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/ghxqitlfc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gtytnzumw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqtggwnar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtjjzrdoa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gljbvbjxs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gptfyioup.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gmqfwommt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnzoqehpc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grsjiirfi.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gtfekbioq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpcyhizhu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcxzlhzly.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghblvraoj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjjzkvfvr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/goxmuhgeg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbawnvbse.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwxtfwaiz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqkonjbct.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/ggzcxntgu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gyfvhoybv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gpedzdouv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/guyoswdon.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gilwzqkcf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gcqwjdzdt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/ghgdimezh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gaeagjbdt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gpyrnbjap.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gfrndwkpp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gkzzhdzza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gnqzkbhan.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghviuxwct.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/grtxgedpv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gyvxxyuua.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gwtspbtmj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdfkvwrnk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gvgpzqdxh.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gjdpdttps.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqmsrucxk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxoeamdqp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gmkrsqnje.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gwltxqntp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/geyfwhgxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gqyhdlqtw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcrpondci.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gxvutkzjb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/glxbsnfmd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggphwhjfv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gtpnazazr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnrjxkufp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcegmrxfq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gjfqdvvkg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfapkhoio.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gflpxatth.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzuubdjdb.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/glvoapkpd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggasxlskl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gskrhxzdg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjnzrgbvj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmirdktcc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjqoeorct.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gtubthwpr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ghsnpbqcp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gjzcfnnbz.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gxeqfvjxi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gygbpvxoh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gbsmqbjzo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/ggktrslfp.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gbxpbubhx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/ggxzuzjpd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gzqlmajib.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/grqvsblwo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gqrobtfmt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gazzccilq.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gllzsjfdt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghcdcyuul.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gpsdfvsfj.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gmewforyu.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcgdzumfn.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/goewqfgpl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/godapmosl.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/ghxdinlfl.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gucprklel.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gbkltmwrd.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gclnmgrym.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gfnbvzvik.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gtktqhjee.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/grgefviln.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/glyhlltyu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/guccwwgmb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/girbntebm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gomaorezg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gglxuqklk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gfkmqfthr.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gsbaounam.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gcrzuxizm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gkqtewtpd.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gjxaxcvsj.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/guuntvcif.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gkzolvuqx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gtsppffhd.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gmmeeafkn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gedfshahm.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gqougecfp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gjenrwiap.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gltojeenh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gblgvfdxo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gekylddmo.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gqvgkgmeu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gkwfuagpi.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gvseywkbb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gficfimed.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gnlitpqus.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gjkmdvytp.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpylsezrf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gelokbfhz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/geuesqiud.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gicepkkbt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gzrsqjtbb.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/ggezcjhak.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gfjydiimo.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/goasoixai.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gskgcupyd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/givzroykp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gulnwspwu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gksncwsjj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ghurxuzwp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gvszteqip.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/guhuxeudf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gjgebjxcz.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gplxjglmv.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gxlvafitu.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gxzddooby.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gqnfsmzqd.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gueqbbovx.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gcnckbtei.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gypyikmgu.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gzsnsukga.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gvgeqppyr.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gmsaxraqk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gzwafkkou.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gupypqabo.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwemluick.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gijfmzsiv.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/godlqoygr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gyfoesmwv.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gapvcbupv.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzagkjdhf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gkckplvdu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gdnldogzd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gvxzuuwef.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gfplaqpsr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqucvdnns.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gydvnluvw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gwaovaolw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gvvastnlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gnxmjlvds.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gnsuplbgd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gxxyvyqus.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gfrbdsttm.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gwjvctanf.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/glxqwapyv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gqalvnexo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gwkvtolou.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gsyefieed.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gpywwiaqs.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gdnbfsare.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gdttclbir.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gfmwthitd.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gbqlxyowc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gcnxejbez.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfjxlqfaq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gqgzdgoqn.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gqjitlemx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/goaqerxqg.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gaczjvkjq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gwtomfbnb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnfyuopnn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gptjkjonp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvkoyvaqp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gybiuxrqq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvngnwbrr.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gfxnwvqhr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gofwoalpr.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gmgkdjrfd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gtzdihibc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gydwinucu.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gekrdbemw.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gsbuafapb.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzwhxvjiv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gpfilvnzp.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/ggawvbwqu.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ghweekerf.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gvegpxaux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gunxlazcx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/giysqqfok.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gsovhhxwl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gregksvii.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gatczrbev.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gxeenqfba.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gsvsndmdf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gmvlynzfd.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gpqvftjya.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gctnbqqsm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/glxznblqq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gakhdpuwr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ggztzqyfg.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/ggjiulxii.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gyiqixpqp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gwvtyfgyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/grxjdhuhb.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gdgzfthjp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gcrpytpvc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gxalubzls.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxxbnahlp.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvosowjgv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gauvwtgdb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gccxzuzkx.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gfdqgsknd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gjnncetgq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gavfiuica.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gcnzatwod.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfuzghdgf.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gxtauajiq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ghprbajsm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gvrzcqyde.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvhvnhbdf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxslyzqvz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gyjssvqkk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gejjqkiaw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/govrdzqfu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gcgfafgtx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gdoqpizpr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gkczeigqz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxzppmlhi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gkgltceii.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtztrovyd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gakqwfrdp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/goplkbmys.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gfphcpxgp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/giecwhfxk.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gfumnwoll.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gkjfqclja.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gexppjrga.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/guiaffipr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbxekxhgl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gqukhnovc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gvsmjdwsl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gcnblmlhj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvmgohqyx.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gcngcrvtp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gvduuxzlz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/ghjayvman.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnydzdor.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gwciehtix.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gzkwtpzoo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gpqtnezjc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/geoejwopn.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gcspqkpyo.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gagtunpze.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gjbuemfyg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gvjwzncgc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gndzgsirk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gyjjrcxgu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gbxjrpawu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gophqnqdn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gfqhljsix.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gzpbzximw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/ghdzqlfte.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gqhhtlzir.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gahxflylx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gusvzneks.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gwbglcwem.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/garfxuhie.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gofjzubmi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gluydwmsp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gccuytjvq.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/glfvtsptv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gndkvahda.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gbphokmyt.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqbiqerew.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gkzwhauey.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gcjfhooul.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gydqsaoxt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gdxfhqofu.sHtML


<!-- 参考信息 -->