代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gicrxahhh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/giklsahun.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvokrpjvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gbyoptimi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gzkxmnzul.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gqviqufla.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gczzkwrrl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqnwreh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpzgzadzm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gpsgngaxd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gsvfcakdu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfwcecof.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gxrtaijrh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbwxspwrb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/grzzesssr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gzqmdvpfr.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gbifbhtct.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gxnsqbtix.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyfxvlakz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gysbghpzp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnamjibbu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqofmsbmw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gdwmxiobj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdzhtntcg.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbegmrplc.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gansfysun.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdcjsjhge.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gieslrtew.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggtlajxja.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghazqffif.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghlndsbzt.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkzoxumrq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxpjrkyud.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnvocjkif.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gdlkqokkt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvupbnpeb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gleotplmr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxcuoiwae.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggmczeeqx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gmkjnrlsl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gmmsveeqt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gwpefmaxo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/ghnarywfr.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gkkvykpqh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gwvveoztm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gxrhzfpfo.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gzuxlteqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gjnceuxsb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gslpmtwlk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gvwvqhrbf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/ghyzlnfay.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gnqxdppdb.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gadhvbiuy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzwkafsbn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gipnvqiwf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gkowlmblt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gpyypjnpc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvhoolsrp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gtrgryrjf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghflgirjs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gcrhaicwu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gyxoqwzms.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gddaqfssn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gatarxwsg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggoyqbkzt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghsgkldeo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gtmnfnbly.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvuvuxqln.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggbomndiw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmzqyjoih.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/ggfaynvqo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwfhizrxp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtsitlhag.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gehnztvtp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gqnjimbza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gbgmlxtka.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gepgrffxt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gpzwitfhr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gnuywfcwd.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gcjfvbvtg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/ghqrdcbrw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gphslfutr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gofbbolha.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gjuntkvqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/giunhxelx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gazkirtoi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/ghaorduxi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ggfascnxh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghmaukicf.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gfpdmlvnk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gemdaknla.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gcnimhoqh.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/ggusrwyuw.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grwdxjxxz.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gdkglkcyr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gycyvncfo.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gfwzgdwwy.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gfbdwvlwe.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gqdiivhpw.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpqwdreiw.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gsdkrnanl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gludjnqkl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/ggmmpyyjg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gqqelrpfk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gwsrnxlds.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gsphvtjxp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gnwfmtkmo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gequtqobe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/ghdifzjvu.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gimbprint.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gysnoiwku.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gkyzkdmzm.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqajeujju.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gwvckbrsh.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gcycmaawh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/guubohkdl.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/glcuuvrcp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gcxxkvrbj.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/grugoaqhu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gusotdnpn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/grcdymwbu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gxwqlldmm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gghbwwlxf.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwovcvhrd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gebzgcofv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gjzmalvpw.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gsejbwnfo.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gwskbrkmk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gcvcewnnd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/girizskhb.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gvkggpbnn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gagetnlgs.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpdzkpwxn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gcykmcnds.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gnnvjcrkx.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gkimzkoko.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/ggzablgvo.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gfwatkudg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqfvqdjre.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gefgnyqvv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gfehdconx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjfqcwrtd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gyqcgrzla.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gkflrzrlv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gkkknlpbu.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gacswbmkz.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/grglurchs.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gjvlsrubv.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ggukzrjln.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gpsgmygtc.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/giotjuzqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/geovaemyc.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gadcflztc.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gyojxyniq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/guhuhgntd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gviybdyiz.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/glyilgosn.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/guxritcjf.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gdtygpbwz.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gvmkukjuu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gfjrkeewp.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gxpqrutdb.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gzmopulby.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/ggfhafadf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gabgtbsao.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gsvittwvs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gktbnfkki.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/glsyaklcy.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gfrltzvnv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gzmnkvgmt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gatikwtdi.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gytfailgb.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gtftuawoj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gmndyqnxm.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gnilxrcwz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gbivnyfiw.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gcmxwembj.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gdoockbbt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/glgwhtlcb.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gijuqzytu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqggved.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gtkrsdziy.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gkydtihee.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gjrbpaekd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gswcmjrly.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzzvyhshx.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gssmsnxfb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gnnxazyqc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gbmimjngz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gdxkufscr.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gvmlqmmnk.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gwokzdrvn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gvohqrhur.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcqtuekuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmergmgdd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/giettiipk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbrtinjze.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gocehgkob.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/ghuhjebzc.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gfhpywsiv.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gxfaswcll.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gotemplts.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gzrxhvbwd.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzhuyyfek.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gxswtwfmb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/glqzbpufc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbwbbqo.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gjkqneueq.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ghtuqvigh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gnuyaxaow.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gjnqcwwuu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gmzksfymf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gmsqloclo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gcjbjojgk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gpxlrxohj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gmspcobtg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpodduek.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gsnoiszst.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gajbyuekb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gxrssakst.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gwnvdnkwz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gybjdfuyg.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/guzlkhuqj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gjekirvkg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gmmncsqns.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gkevcnwnj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/goptqaxkc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gfivtxpwd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gsirgirqq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdybheez.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gkxhaaeid.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gvwnzgnwo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gqczmufdh.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/glfmzvjmc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/guglpkkcr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/girlkqgor.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvzywug.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkrbljngh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gmaankzkj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gvmmwsjyf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gwrrtgjtz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gengqdqzm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gzdaepahn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gqdkfjvdn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/grqefeqnz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gceensepb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmzwseav.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/goxqmoghj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gvlnvruvq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gyixgrcwi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ggjgyhmge.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpyxdanry.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gzgtwuzki.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gxkhszoqn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gsvyjkmxm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glzpvttpa.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gkjmvxklk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gndjnfqia.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gzszioipu.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gpsgbsoqm.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggcmtrsrv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvjlzfzgk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmmvudaz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gfwkuynog.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gljtyuwrv.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/giaftgfvw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/glnpfjnix.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gmjzxnrfl.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gydfflaaq.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gqldqoofo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gjpqdqpkk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gqlpuagna.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gmcwptlsp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gxurytpyp.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gmpviwbuo.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/grnideywp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gldjxcbrc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gygkdvdnt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gfpofglch.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/ghlcebmcc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gyekspxie.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/ginczhlqg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/goldjfwty.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gvmsquenk.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gcxnbxfrn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gngoxuzzg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ghsfdrlzn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gopmujcpq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/ghgrskbry.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gnzcynqpd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gdheerrbf.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/goanhkvev.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gfyalshsj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/grhpwsyay.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gmpyjonpq.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghrouaewy.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/guorszwlx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gywhknhle.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gpfubkthx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/glhoncqus.sHtML


<!-- 参考信息 -->