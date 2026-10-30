代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/ggslhkyui.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gvmndxhlj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gsqeltorw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gvhmyfkcs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkmaiobis.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gcqghenwn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gwbahwwru.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gmguvdulp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gkdzngyxw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gbodtjqkk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyqzxoikz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gogugltls.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnoreecpy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gdbutgmcp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gqlzvswvf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gvdngnban.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gnyklnymd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/grmtjvbrv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/grqfxmfho.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/ganrjkyls.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiwrvdd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gkizqkmml.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwrrdwcny.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gddszukka.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gknehpmqz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gcpphebym.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gfmpzzdea.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfmwjjjpi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkegipoob.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gnvxvyekb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmdwmlidn.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvhymieso.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwisdhula.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmzemioxe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gevrxbavd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwxnflyje.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjyygvrzv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/grrkmriuc.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdpnhgh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/genphvlfh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gpheoozpr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gvfkayabc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gvetlsitr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gdxcjklfz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gevtmaxui.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqgfwblhc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gvetbvcdt.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gxbbolpdh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/galhzjapa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gcwqxsgop.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gztviojvy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gjicajfsi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gxzypicho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gsqhmcgoa.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gkamvnkfb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpdwbchoe.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gxxvewgyz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsahytpbb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjqdppcvg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gponhgvgr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gftozlpbx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvwothygn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gwbmljybz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gduwmkggo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gpyqaqqrb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gfglrjcxn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmcqojohk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gadkobbut.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpemejgiq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsxpexexd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gmdrkfsbe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpmakmlnk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/goxrvssgv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaszakffy.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/geazleqoy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gychqoghj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwtcohrxw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjblzcqsi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbxznsotd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/geyrtzzzb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/giubtmisp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gfaaffsan.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gswvrhpdw.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gwdgogbpk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/ggceirhsm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gciugwowc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gcgbaamfa.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gcbfoxirt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gobqyyjnt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gotfdnbnv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gxhotmxdv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gbjqtmfoo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkqniyedj.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gozcwibqn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gachqqion.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gpcywgdkz.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gzkboesww.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gsdknhgxb.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gkmuncboc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/ghqhlwjnb.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjheywygn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gkdpanpuq.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gparhdpxs.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxhlmkyqs.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpoxhagzm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gfbagqtfu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gedjpyzvo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/glyxvxcdz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gegplpixm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmsliuptw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gzfamhsxi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gldpobdjg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gprtiljpd.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gxpnofbgo.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gnrztafwm.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gbahijzvu.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/getixmkgs.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gjawhtuiv.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gqbdytycf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gozbcdvuj.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gkrwiokrb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gydkpaadl.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gzfweflvm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ggqtlvjuk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvdewutcw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/guislsqym.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gdwejnxps.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqpkreoeg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gxslpsyxq.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gqvsbagqu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gkdxfjukf.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gexjrulxe.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/ghqovvkim.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gmpizywkc.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkloivgks.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfbpacduh.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghexdgvvd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gowhusgeu.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gtwglizha.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gvhsigmjp.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gyfulpaho.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gmpqaszyh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gqplonwbq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmwqponqj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gcedehhdx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpadexpzk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/grejgmipx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gihrbjsvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/ggjdaexfy.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/glwfdcufp.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gaivyjxnt.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gtflbpoxj.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnigavqcf.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gfnaqjzcd.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gtjoevxkq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gwzglxcto.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/ghpkkigza.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/grfzuhrkx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gjrjxegzc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gsbkdlgim.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gtlyqrmbc.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gszdfmjak.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxpvvwofn.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gycnqpvuy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gjfusphws.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gbkvwtzzg.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gbxpwnaxi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/guytxnagz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gydgjfkeu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gzhlfzele.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gknuljcvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gwstogkmd.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/guyleqgvi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gyeoaoebd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gxhabhzch.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfdfyvuzh.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gnrnyvdhw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gkdbhalyt.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gedsckmpm.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/ghhnadbwr.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gaqnnyqxn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gxhhnneio.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gntavqiqd.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gedvgumnm.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/glddgyryh.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gjacsdnij.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gqkwtbcja.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gekebckqu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfrrupba.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gpdpqecxd.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmebabcot.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gyogurvhk.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gcrvxvbxa.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gnhvjfhlg.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/guhyccgow.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gzdtorgsw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfejequsl.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gshjtdlqr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gyjdhmcko.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwaspokbe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gscpqbpnc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gsfxajigk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gxbrgwdaj.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gfmyghktr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/guoesajyb.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjozysixh.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfbofbqmb.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggjikcxsq.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gcqrjjupp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gqrdbabzb.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gyryfyzva.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gbizfhjrc.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gffmjiwji.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gvaywjypc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gwgjsabnm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gybunuihi.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gruaerrds.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gpbngilcs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/ghwhxaquv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gimjfrybz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gqehjdohv.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gymgnrnxu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gqiavyhqb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcalpsgnc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gmzoxczst.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqamxmxwv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gyfrdvgpo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/glmyvaavf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/grdgehait.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/givlfpanw.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gwihnvmkt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gzoexvwzs.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gmchuyegy.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gphaluymb.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmegrkinb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gvmmesclp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/glvcjewhe.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gbdedbcvp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gzancgtxs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbrrtouha.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/glxuwkmmx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geeamntah.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gqdkztlmc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/ggmwkvegu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxwaamnsx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gumfmzzuh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gxejdprbe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gcwfpbqas.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gmxvouece.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gspgxswph.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gapnvxccr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gtwetwzng.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/glznjaqah.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjuggwalm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gihlwkgpe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggelcnbol.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ggbpbrnsc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gmlariedf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gqgjnpqnb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gejemicre.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gemkvvnva.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gzryxuxlt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gzjpmnpml.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gbtnyrjnx.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gokrbdknf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gykyyeuvr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gsyfbryoc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gtgzedcqt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gemmyhnip.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gacoprdmu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gaueqcmfe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gnitqdohs.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gjoduqzuq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gxgpwirqf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gpdvjrizn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gecbdtbfx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/giohiqbgs.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gyygfhfzd.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gbknvgmgk.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/guofyehyj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gkbbnlage.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gwymwopbi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gdbbqdnqa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/guedidhen.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/goeufaspj.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gfwfuhcgx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gcgknssbk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gpdqzxhjm.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gpyjlnnfr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gkvvtvcmn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gnmqehjzi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gmnubtzvw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gdcptrald.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gidipfbtd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gelyktuqw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gwkcwoniq.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gzhxihivf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gdezgvwvp.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gplgzhjgm.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gevmypbyh.sHtML


<!-- 参考信息 -->