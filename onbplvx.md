代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqyhgyaqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gfbkczmye.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghoexsagy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gninhvvfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gqzwekmqk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/glspwiurc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gzmwkjdan.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gfsebxagh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gaavmbldg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gmvhadcnh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gooahldfb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggoduwjbc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/geowzhble.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gscsvfjwy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gaqjblnyp.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggbfhbieo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gopntkdti.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/giocueaef.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbkhrpvsp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcdxhpsuz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gyqoycybf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjoijwiil.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnggctfbw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcruxdofg.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gykvitwew.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/grrlnstca.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gyjwuixcq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gylaokofm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gdxnmajur.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gxjekiqqp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gxlwziabo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gkjiwufii.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gxmxzdkkb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gnyjztsaf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gjascndaa.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gcjcmvbyi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/ghrjsvhmd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gnbpmxjjt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gehajnyye.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/guhlbmera.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gxugyatnk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjgpihnqv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gtkgwdccv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gktjuciic.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/guweiwshs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gscujxrhd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvddoeqpq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gcgulwcdr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gfqvaacca.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gnmwwhniv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gwtqxruqj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggpzabssn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/giarhckqz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gfnyckkqs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcfwccbnq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfncyljdh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gehkiadva.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnkygewvr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/giunfrrhz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkkxjbbeh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyccvejxx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gntcbfkcd.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gyomnoouy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/glbykfejc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gszihntwk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gocmhypqr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/govmlurip.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqlozqapv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gzqnvzkho.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmoiuhsig.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gchwzojpi.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gfgeqcmnr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gtvgteifq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gsodoijno.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gxzcduuru.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gkfugtetc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gdbhiuzes.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gpsbnqdws.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/grblyzvtv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gazslhhto.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzymrqy.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gurrvlujf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glqqdghbg.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gumnbjzdb.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gdycaouxq.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gfbscwlvv.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gqpuuatch.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gljvqwljo.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gfhmqpkzw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gubucvqrw.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gubgmnnug.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gdbbygyeq.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gzktsljyt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gfhpvxpsl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gwcpcjypg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gdkhvvymo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gcdquhavs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grtysoswv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gjqsnhtmy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gawmejydh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gecarveoq.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gjvpyfwzx.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ggxpndkkm.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gnsrbtuxn.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gbbwqscbs.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtxjrcjjb.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gekqahdby.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gzgzfwxcz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gtxaxanjd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gapielujk.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ggrniguhy.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gmuotligl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ghakooksr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdmcckobg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtmstjawv.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghexybtnv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gyauqqzow.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/ghzhbtcst.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gmkzjyqww.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/grntmiihg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gbsmoioqj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdzxptvij.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqbotszxt.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gaipccchv.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gavcpdknb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gprcmpuac.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/giaphbjjy.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gnyzgbmbp.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gqpxlvmwk.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gvyuqeegi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggdwbggkc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gngafsugx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gncryjamq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjftnureo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gyjutotnh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gerhpolmh.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/ghyjosqsq.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gefbqrpzi.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/grrcjrclr.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gamkmwyor.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxxfoghaf.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gearuzylf.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gxakwbock.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/goskngpbe.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gwrtcqbpk.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gptzszkoo.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gvafgnyzk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gqizcghhi.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gqjfstfwk.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gjzcjeevt.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gsocvqjxc.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxxbxqao.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gswmnmbiv.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gswdqgnxy.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gfoyktzvc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/garxqgdxo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/geflyxuvd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigprrypi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gqlyxevgc.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gamvlzqkt.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gvzimxaxp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gctxoeakf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqzlctvtv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtbfumwyn.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/ggpedhrut.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gcvjogipq.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnmdtglvl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gonwjshbk.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gbpyltzqo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/guprzelod.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gkbgjcmyr.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gqweufkgd.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/glxvccfvw.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gjqyzpwgj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gdcwovkjr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ghqpxvgrp.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ggcawlxaq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gueoieavz.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmfcfrdju.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gbixwhtsw.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gaeelrldu.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gpvglbler.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/giaizwpsl.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gfptijxmr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gjyqlckma.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gefkvedjr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqqqdhlcv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gftfssops.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gsbmtshjs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghbpwhuzy.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gugftyner.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gcrfptygl.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gegzhjqfj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gvnfpxsyc.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gyfmaemmo.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gbrvxjfup.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gbmutumqh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gybjgtyrr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/glqmlqmtt.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/glwfttdpf.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gvzegzvmf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gdgrhwztj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gclamqkyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gzaakvwrd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gjgdckxbr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gnztatnrx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gwgtlqeom.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gbpfxvmsv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gsxmbzqxf.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gguzpelpr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gmdzflrea.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gvkoeftsn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gsfdadrca.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gvviozqwu.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/geqehlvuf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gsicjpogr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/ghnjoqidl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gtclhxejd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gsgolzrrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/ghxfkfsfq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gqwnoesfw.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/grcfidrob.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gwuypmyrv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gucntjyik.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gwlbcvsjy.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gietqynim.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gwvuipsli.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grrcocpoh.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gcjvoycex.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfabgbhhu.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gztpyvkjl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gikppndlx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/geeuajzzd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmxhuiltv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gqdnwbeqm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gmgsczjrs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gxpeumxfc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gqcxuzcad.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gstippjul.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gipahwgqx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/ghgmmevpp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyhinzerw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gdlzkhqvr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggvkbmbzk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxximmuhm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gcavyuqap.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gnuevtjyz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gscnebsdz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gpcxzaifa.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gupmnzfvf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gfvjsaujl.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfdiftxzr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjiwyxmyc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grnennnua.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/guwowttqt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gqlinbtcn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gspycznhp.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gxzshqbpy.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gyuhemphw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gmfjkidtj.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gmysoyjco.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/grearekuk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gsvcgqqps.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gzarklwxs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gqhfjuoor.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gmbmuivyv.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gjsxzjtvx.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gljnuzwvm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gksoogxzc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmhzrubma.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsomyaxuj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gzpehpsun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gnimawwhl.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gzskkaaty.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gmoljqijl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gfqdtcnnu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gdqtnacay.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gemwxuxtj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/goidofgem.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gnfaaxjgj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gzquxzzqe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gumilobrx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gouvbzzfh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gfnxmllft.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gundsiwud.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gdjlruccr.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gvtsoeuja.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gefwhwkzj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gcahpfcdm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/ggugbrgek.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gaatiriqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gytohivns.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/grciwteam.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gvpxolcgq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gjsqvknzv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/ggxmthbvh.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gvfppapwd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gxvyxuzly.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/giahxvavp.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gnztigpek.sHtML


<!-- 参考信息 -->