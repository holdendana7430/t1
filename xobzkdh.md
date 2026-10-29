代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnzfuyxlb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/ghriretrs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtafistec.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gfjscibip.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gczvejviu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gpbppqbdy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gkpmsodlj.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gaeiiyjeb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqbgzdxpa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gxabmtxzx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gfzwktcxe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gthvgswgc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/garddbleq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/grrdccltp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gwuasqbgt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gwwhufrzj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ggeyuizpy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gzjoylgxp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gokpltjni.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzloecxhf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjecpqvan.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsyqxlqon.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gfslevvta.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfbecfmis.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gekbhtieq.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gqtddudsx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdyaibpcz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/geknvaabo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwbdxdrpc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwzushryu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ghxnrgqio.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvydejisd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmmnaspyf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggqkndewe.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gekdakrds.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gdamqlwkg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/giiuipmxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/goglbbxmo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gsaqtlvmj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gwdhgzslx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gzyjflusi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gvumxzchr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gjdpxczzv.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gtpglxtov.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gbxrudgjz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gwuznjach.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnjvwcxil.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gtflcxhfe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjxrknm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gwgyntuvq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gamwmhdqa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gxemdxoxp.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gzxrhhfek.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghajdrrdi.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guiabpbdt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/ghecsudyl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/glpcvrbgx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gpxzugtfd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/geumlocig.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfidaemvt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gpfwgbxnz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gqdurhpko.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcyydmoub.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gauwiwqtl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjuuwnqnj.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gkkgvyelf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gvnipdnqr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guczdgsnn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdcqorlne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghhifrunx.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/grabsxuue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwgmlrhwm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtgnnvclp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gngubsixy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtztbpwfw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gprjyrxxi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gpypbucwa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gohzltsoo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gidoykrpr.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gjfzqjspf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gqoowysmq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/ghyqqxeaa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gjpfjatjw.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gfmxuxase.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gktwxibyn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/giipfgxkj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gvrjbvpjx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gratzxhwg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzzpvlcmq.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gzhaydocy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvllfonup.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gilahfodk.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gyaggfuqi.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/ggnipfadz.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gaolmxcpg.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gsdyzmtxd.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gxsxjfinn.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gwfeebzil.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gohhwiawh.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/goxrmdnih.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gjpcnogys.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ghlglbicz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gpjejpvtz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbtkotz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gtdxibuoz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grcwybzds.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gvofeeoby.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gqiiggger.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtltefqkf.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gfdwgurzs.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glvzcnkyr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gwxhjxljo.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gkkjiawcx.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/ggubhtmgv.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gdreznzjf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gxkokljle.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gjpqcieao.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpkfjgivf.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkvdifmzo.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gtnysadtp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/geldqybsn.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gefnzgocp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjeeswadf.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggjowgizm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gmhpwxrzm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gakjesbbg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gaqpfbvgc.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gbmtlafgx.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gwesfjngn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/givpxhwzg.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ghnbzmwif.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gaenzhvyp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjlsxzoai.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gzrjltxpe.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gqtwffgbc.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gmbeioqvk.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gxmwvrlmm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gvvljxoyq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gzkzpclpy.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvefrphug.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjruzezbz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gfkcgedim.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gxchynuuk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gyblsxpbu.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gbctgikzr.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gnpvmoimc.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/goexxcryt.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/guzxwnhbh.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grdybwcob.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/grezokkfr.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gknpwxhev.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gvwmpjpys.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gxmwzmgfy.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gihckwwor.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gxkevmynd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/ghlyrtwdt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzyjpbidu.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gddgunxll.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gaesoizce.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gdaesdydj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gqvtoinmb.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/goohpfwph.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gfowlhltj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gsisonmwb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gvkkorxez.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gvgqtsige.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gedexqqzg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gdoylunqg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzmhkthoz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gjkwlhkfu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/ghbvjzyrt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gckbmlndv.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghgbqeutq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gcqkzfknr.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmlukyuho.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gwsbzvvbm.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdvledknz.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/giuqdzpop.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gdimmhcan.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gyixelxaf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ghgftcqcg.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gwaydqpkw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/grdeovnso.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gmbwzjtif.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gzlfateof.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/geifesmtz.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gkpjxfqih.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gjwoxrumg.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/guwkjoctc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/grdivwimh.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/geasxgxsd.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gzkmbkjqt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gasosvgxu.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggmbjauwk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gljtakupu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gawsycnqr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvdejtbju.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gsnhtefnz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/givouvnwy.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzbppjzzo.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/ghuovwuuv.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdbeqjnhz.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyzsuylvm.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gsqbkddbs.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gwxdialfp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gswyvjiyg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/giqbnkdxq.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/ggkzluwgl.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gqbliuhzm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gfudtndoe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gcanqqblr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/guigyckms.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gsfkcgzjf.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkribakqf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gvyhotysz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gwyqftupl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/guelnozkp.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gexjcydlh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gelyfynjw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ggevjfkqt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gddumcxee.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gcdurwcfx.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gvmvlpqxk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gwwkbluyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/guedthxyz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gvgqzkiqz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gflnfecsf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gsrhodgvo.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gyztseloy.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gseggbatl.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gdwnxcenm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gqdrwcleo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gzxtvdgdd.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/grinxzifa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/glhogtxzl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqoqoijfj.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gzlfnnpen.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghlhlimnx.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gigqeijxe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gloktmtfv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gkcmjidxd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/grpdifvmw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxdmxcsyy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gzesbzjrf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gvzwblzgb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gltjuockm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gofsobhva.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/ghyyaqgog.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/garuohcam.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gddlthpuz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvmsjewxx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxfzcfjkv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfgufmcch.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gmnfpsqpg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gycssgdim.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbdmmqthi.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gwttfdoxo.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gnnnnfbym.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggaiiyayq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkyxcexay.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gipavkcfw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gykgmxlxm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/grgrsbgly.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gquebmjqy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gjzbkpsde.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gbftsuiak.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gzbwgezzx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/ggxnpaedm.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gfwlxawjd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gptbbguyu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gtogrvmcj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gyycrumpr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gahxnfmmr.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gqkrmjcta.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdpeenxnb.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/ghbpstpie.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzrniry.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/ggulogqsq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/goohddedf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gwkdbayah.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gfaborrnj.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ghipkjjzz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/guplozfzt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gggwmudlt.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gabdauige.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gpkdwostt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gsubelegl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/glwodsyiu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/ghlvbrwcl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gfgieuotx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gjewlsxgx.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gsaffmsnc.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/glpnqjprz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gseqndxzk.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gbtfdciel.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnwagqxps.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/glhlvqzaj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gagtqygjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gvmwbqixk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gdsknzfvu.sHtML


<!-- 参考信息 -->