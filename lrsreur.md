代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/guxwsyfjj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/grcttwqhe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwjosjyj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgttnooj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fanxiaobao.xyz/Article/details/grlxjzozm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhlsfphc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhchhmgo.sHtML

[F04] 追加写入文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grehfqmyg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gcxsjwtni.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbceytwj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrtvkzdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/glvmnrrqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxwvkjt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gwtwdvkoa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqdmunoh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdflkmvck.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gikkazhoo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfdmehop.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgblmjbd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwzsvmcva.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gklakyqmx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlwxwgbu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gculsxsva.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/guikmgnpx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/goevrydqw.sHtML

[F06] 删除文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gggthsdvp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/glctmzzib.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkasvwkp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginljftub.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixkipar.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfguxkuon.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkevdaxft.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/glvruiser.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gatblcagj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fanxiaobao.xyz/Article/details/gpiydvafx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/goyuegeuh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gbaxqutfz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzcwsrx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsrfqcph.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/gvxuevtdl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/glmspowlo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpivhojql.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/ghxijzlhj.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gifwzriqo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gqerepszv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsxcdfxy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdmawpe.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/ghehbvbxj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpspwayxp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggssfjbdc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gtwowxrbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gsbqmened.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnhiprhu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gorvmbivy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginpqhiri.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazyzerpc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gmluhmyiy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gcpszjcmx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvvxfpiz.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjmlpqvr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gemrpxpmm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkqcfuzd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gphshvlcv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gwbmazhvv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghlallwyt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gflzmnsyo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvnycypf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfirvucee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxobubeub.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gnzdnsywu.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjloeeqaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/goowmdoqu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gmqppcnnm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbqevhils.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpgnywdye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gfhhmwipj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fanxiaobao.xyz/Article/details/gaxadsenf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnejeanwq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/gpeovkidi.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gfsydnxtd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjrkvvo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gnrhobgdq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/grvgisdfg.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gosrnojbo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbnstapw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/gnwpprvhq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpicbyuom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfxbvszw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqurwwoh.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gwsoljycl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxmdvespa.sHtML

[G01] 定义类
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzwljix.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/gmrhakctm.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giofbgtzl.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkiukfown.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxbbvrsj.sHtML

Java: class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdylodceh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudmitzha.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyrjfkmt.sHtML

C#:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqylemaru.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmbrnwcn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/ghjgthzma.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyekljzaf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwozcqqo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvkuwjge.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsjnortr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/gpnioqgpf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscghqiya.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gchvsrjmz.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnnzrvmu.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gzyxsuvkj.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giknwnitl.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/giofnxfln.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnieuknn.sHtML

Java: private String name;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwzoadbm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gfewppobz.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gatrzvysp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gwjnnrutg.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gsaedmldw.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxcbpfmo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/goenxbrny.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gppywujkb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcixwvgbs.sHtML

Java: String greet() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxjiqkns.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbauvgig.sHtML

Ruby: def greet; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/ghzknsvdb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gywpelvve.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gwledndaq.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gkljujnab.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkbfbmig.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjkamdlv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggceycwof.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvbltmkos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gzozctiug.sHtML

Ruby: class Admin < User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gtqtosugp.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoaysyos.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gjtssdytk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcowjsve.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzwmeydjg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfwxfsdpk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecuwknqn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqiobgtez.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fanxiaobao.xyz/Article/details/gicrhuzyn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/gmopjuzgj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fanxiaobao.xyz/Article/details/gcpqypoqk.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrapzhrl.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjasfbin.sHtML

PHP:  parent::greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gfsgokfeq.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gvsjhrros.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzclvpnwi.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/guujpdgub.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fanxiaobao.xyz/Article/details/glqviapcn.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwdakxaf.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcmrktk.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/geywwseaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzbazria.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkazyvti.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtvjgwaci.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/glqbkkehy.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghaollnaa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuispzqm.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/gzfihwcey.sHtML

C#:   public static void F() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxxutnai.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfbzwuy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/grgbmzrvg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gppvwxuep.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fanxiaobao.xyz/Article/details/gycctphot.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyizxpvin.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gctierbte.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuhodeok.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqswunwlv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmkvfsoe.sHtML

[G10] 访问控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqehaqewx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfujgmkq.sHtML

PHP:  public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhswuhiz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaruivgm.sHtML

TS:   public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsuwdipv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhhaqpfu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gooqsfumk.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gomvtllzj.sHtML

C#:   public / protected / private / internal
来源：http://wap.fanxiaobao.xyz/Article/details/gqsokjokw.sHtML

[G11] getter / setter
来源：http://blog.fanxiaobao.xyz/Article/details/gmlhpwghq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/ghjxqgver.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbwqvyqr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gansigvwz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdycnxwhv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gozsrfyrz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/goztkstua.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fanxiaobao.xyz/Article/details/gddsgbmqa.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkcpsjcn.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqhowhwz.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gooakdlpt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzntcfthx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gguygvroa.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geashhtqk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsvkqmes.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gkoqmgmtu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdltlsurf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsayjobty.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjuyeukh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpbxymjd.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gmgzyoiaz.sHtML

JS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcopgzpe.sHtML

TS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gumusnjff.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gewyjycub.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhpdbgme.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfncbsls.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbfkapp.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/gegshdpid.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfnusdnj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fanxiaobao.xyz/Article/details/gtfsxanzd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gwgwnabxd.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fanxiaobao.xyz/Article/details/gprjceqtw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoimrhid.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/ghzaigoav.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fanxiaobao.xyz/Article/details/gwxeegtur.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gknzomdxb.sHtML

[G15] 枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gawccclyp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gwxexzaja.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvldymssa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrdkfka.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genifynxp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fanxiaobao.xyz/Article/details/gbvyqkwnz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gfkpucemo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmudgoz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiprokfg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgglovnr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/grhfikhdd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gfunlrooo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxoeioij.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqklybzqh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfgvgjra.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbjrsaik.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganmiiuyu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyapkpla.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjdohlqt.sHtML

H. 异常与错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgixkbnu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtlsofcbb.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/ggvosptae.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fanxiaobao.xyz/Article/details/glaywkphr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggiqugxaf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/govscdqgk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/galijxfkv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmmufmov.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fanxiaobao.xyz/Article/details/gqwquiicw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ganhukyzy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsjwwlqwy.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/gkgfuitxm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdieplllz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfpuzfvc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzswsplvf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrgcqdkt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjlwpxvl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/ghlufvxov.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyyyqiym.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gperhikji.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuaclzbk.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gnkxacqcf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gokzlwusr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmvihvyr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfqnfnum.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqivcuycv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoyjxbye.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiniyzaa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfbwhwtb.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvakkcl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gnykckcyc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwvkcxvf.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvfylfgk.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfrmsmyz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gveoegoic.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnitcdxby.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gyehxpjdd.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fanxiaobao.xyz/Article/details/glruzetpk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golqmxkje.sHtML

Py:   except ValueError as e:
来源：http://3g.fanxiaobao.xyz/Article/details/gopgyeyvo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fanxiaobao.xyz/Article/details/gghxkyroc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gevykyqmb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzfsgtwbw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdxnchtwr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gjyvfdyfd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsdsllru.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzavyxqyd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvjuudau.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gdcnjowre.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaimpjzep.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/grfghfwtb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxndfnpb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/gzlwcgskx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmhbchtr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyfxofhr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghqnygvv.sHtML

[H07] 断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbnjltws.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxuvcato.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gavyggyag.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxabhgdpj.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gwgoytafq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/geacgqpdl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fanxiaobao.xyz/Article/details/gelqbdhui.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/grqhjzgkm.sHtML


<!-- 参考信息 -->