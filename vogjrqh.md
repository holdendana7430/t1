代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gfmihzrlj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gwjjutbsw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gsybrmfbf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/grdredhuo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gazxjjkax.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gbmwsojyz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/goskuhesq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gcrxrwrsk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gefglbasy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/geflvjixu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gynvlcwki.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gmxrptzhx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/goniupkal.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gaxindwvo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnezqbekv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/giiwnnggg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gcylbkhdz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gmfksdnju.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gwgpdgttn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gimjuskwi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gxqmvblxe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/ggabmyokj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/goxqwvcey.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwpxmeeje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxrfehrzc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqqolemkg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gkudvrrez.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyolaobgg.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkddecjeo.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gnpixovvg.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghfccogbp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfrsybmtq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gahpqkgwz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbwtfltky.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzsxjoqor.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gltmyoibg.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gubsefckb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grmouqdty.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gglpwofay.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gkmzrscqf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/geionmapf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gglkuwnnz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gnhfjfugy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gzmkaiyab.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gvqwagogv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gdywtplfp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gczxgrodz.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/geolbwkmk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gqyftiaie.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsvvusvi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gizrpotgu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gwjtqwxmb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gfiqmuqac.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjknismtr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gfpizhcbz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/ganglxepg.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gozptvhay.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpzhfmsfy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkrcvcsmo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gpylfwomp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gqtghckag.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gwdaulmsl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gpsugntft.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gokcanhes.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gaifjfont.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gfodhmmsv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsebzfbyx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsocbxqxc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gnnujlwiu.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjfojkess.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gpxdzsbrw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghitovkza.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpychrozw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/glzrjtkjq.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gthebswue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gezwuztbm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/grhhcnkcs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/glwnpssou.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghyddmolh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grhiamfua.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gpnempqvy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvhljxuvo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gzedtlztq.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcktzwc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gqwjxgyaw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/grbojdivd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/ginpecjsm.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gyawlkgvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gtpnotqqj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gipatqqky.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gnttruspx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ggbcsurnl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmczilxir.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gxbditgob.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvrttlmgs.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gjqfdnklj.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gfugqabmz.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gvgptdgnq.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/givmpqtnq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gxdgcjhho.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gzllvpabp.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gvcdcgdjs.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gzxzgkkpa.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggspksxsl.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggfsevwll.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gcyfubbbl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gzwzhvwrd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gaisgihhs.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gtdxfknxk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ghkckounl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/glfstfddq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gkyzjrdxp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gdyouqsbv.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gcoimrnav.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbuoyqoey.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gyamonboe.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gfdrndbre.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/grolglcwe.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gxqeeaxyd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/geitmqbkj.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gaagzgbay.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/guuwhjkvq.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gmnqogvsb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gztjanmxg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/geqyvyfro.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggeryrahf.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gplyqeqnq.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gfqmdresv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grjwtgtjn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gutdtnyhx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gdgrkpsin.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gjdifpucw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/ghxgevtte.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfgunuhdq.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gmrqtegpt.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdzujlhrb.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxbdkapiz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/ggouufxgl.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gipglmzxw.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gsvgzaczg.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/giabizvxn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gglrxkqdq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxzwxoklm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnuvcjwts.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmoremrhm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmnlexcew.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gyxkgxitw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gsrneqnpv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gnwmfmtez.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gobrnqeit.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gsonokxpa.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gwudozuzr.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwwjwsebq.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gjjranhvy.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gtubzrjqe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gwxewmdpj.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/ggqxohgea.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gcibiittm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gynswrxyj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gcoeawlwi.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwzjlcty.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gdszduswx.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/geslyeavq.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gayteuwmi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/guttlkylt.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gynnrlyyr.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gkobabddd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gxsclgmeo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gdohmlwsr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gznroznaj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/geqciknhf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gspowoyey.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gboxkqwpy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/ginfwkorw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gbeoysipn.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gbkhpcbyb.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gsgfcqwhs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gunsziwkv.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzdivznml.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gclocyrig.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gwvjgpkvm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gjkjeuoku.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gmvgoijrv.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gsdjdnpyh.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gwywsnfzd.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/goaojkjab.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gdnifivnc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gqtrbupul.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ggxkcchen.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gkieeregq.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gopjiveex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/guqeoufqe.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gdulctbhs.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gekyuokin.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gxbsnwgqm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gmdkosbtf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/glegqeana.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ggcdlicmu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnbluemrn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghidtlsui.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gyxwbmydb.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gnnjysldy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gzkhnxnkw.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/ggdntbbbd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gkeswgvhi.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gelqdjpwu.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gasgfmehn.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdniyldjo.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvtsujywv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gumcqgvqf.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfdcoxm.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gicwppteg.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gggusgjss.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gtqptsdps.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gghfjatpz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gavjgmsgt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gfpwkrfuj.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gplakhinn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/ggxpfjxsv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gldqibzem.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gfwzltlfw.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gfizpelfg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqvujsy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gxcafcopo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gxkgxgjpp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkmffdeff.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gveldnwss.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/guaemmtoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gzweeefom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gzquxrnfd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/glrxkzwuz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gducaxjju.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gbfvukita.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ghngypeji.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/grmlzzahc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/guesbiwdh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gfidymlzz.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gioiesork.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gpmfpjmhm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwlzjkttm.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gkgblwdmy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvlwhducp.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gyonchstx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gosrzmhnn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gjsfbjazp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdtdmtntc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gloamfkyh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gyqqqmhjf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/getzmqktv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gihcuonan.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/geavnxtmk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gsybspdhp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/ggkzabgve.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gykkzcpmt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gzwmynmbm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/goouhzigj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gunuahcls.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gnuhgsldo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gsijzrmgc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/geugapqcp.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gcwmvlvva.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gskhssuzk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/geoftfrbd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ggiyfyhga.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkowrzinf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gauvrknxi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gdwtiryqs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/geeatbrjz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxrlzleyz.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/grbqkwcpi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gxlrdtwbv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gtcdyoayi.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gmoqlvucx.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjauogixl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gruhxgeql.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gybsfwyno.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gfbecderd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gomhhobca.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gqftztxdj.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gxlpdqhfw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gmqtjizbd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbfvpmykd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gkvyhifhz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/grinxcbmd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gjvdghzaw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gvpbzvyyl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ggyyslezb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gtkghxbjd.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gmyvldggc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwmarbpqy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/giqvasdmc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gngexudii.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gskdymijh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gyvzbrbys.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gfvxtubsl.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gputlytfx.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gfxyksbgj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/goplritzz.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gypqqjluk.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gohseejac.sHtML


<!-- 参考信息 -->