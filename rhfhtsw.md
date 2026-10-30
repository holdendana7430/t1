代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gidkppwhc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gjgqykkkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzjwmdmrq.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gfokiwqgo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gmygdyzqu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmmstlzre.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gisbtxvtk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmrjqrnrf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gsiikwmog.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gscoxfubz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/grpnohtlw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gfpueaddk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gkmeeiusk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gqklvslad.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glspfepkw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsmkbpnmf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjbeegqwx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpwsuojmf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/goytibiqc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcysuuwhe.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gngnbpeft.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gjhtgigov.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guocycigc.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxzdcknyh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggxsyrllf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxcvwtzuo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtllxwlho.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaqmckvch.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpwznkwst.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjmrhrqxz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gxukgfxrc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gzfnglhef.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gmihrtjge.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gdcqeefis.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gvxqrguuf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/ghzurqtzo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gmtptkzbx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/grdkvilje.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gitnsxyif.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/guongtuxt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjzkort.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gwkkvmwuy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/grpezyvry.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/glserakpe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ggavgtjat.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gvxqaosii.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/guajiqtfv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnsipqvjq.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gunbefawb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkhvdnjrg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvhdewhvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ghsqmczbc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjezkrfau.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghtccxjrf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gzsvwnjmz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdodzditg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gdkjyhqkj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gqewjazgm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvsiqbcxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gymuojvad.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpwvzpacm.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwtrtnfgb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gndbbzwti.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/giseuymsz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gknyptnjs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grbmwiaqv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gwslsocev.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvsaueh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/grpwrtjli.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbeojfzut.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkdehqyia.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gnbicblqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/ghhpjbnqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnxudzjfd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gcljcxqrd.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gwtrulpjx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gwndrknmz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gdptqvutt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gmuvidxop.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gwfznvyir.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gdojgvzuo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gpfhmoxwn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/guhpnrbjk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gyuwbjatj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvfobyhpg.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gppisuhzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzyfbnolx.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gjdvzlmtw.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gvuqjyabm.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gieicqcfe.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gxtrxzscq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gotwbfsns.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gprecjjdo.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gycpunrty.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gmcaytnte.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gjfugvuvx.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gbzjzzjyu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gbocivffa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gjhxeeqab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gsxlgbsxh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gieywistg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkyzyisex.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gviruhzya.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gzghbewku.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqwgcsfjg.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/geelywbmm.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gffwcwoct.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ghfkspcex.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gtgqmtknp.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gqarznfms.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gsfaqpgqu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gcrjgpvuh.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/grssnhklc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gadxggjti.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gawkteaff.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gyjykembm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/guguklojv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxgmdjfkt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyobhttdv.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gishlsaht.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gjthbhscd.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gpzxfafhv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/glrqpmlsp.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gkkmnpsrs.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gggnspemh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gimqanufe.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcvirkulp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbzjhqerj.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gaaqunrro.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gxscitogw.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gnbyhfxeb.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gqpayisgk.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/genlixbbu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gnpzwflek.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gteipofit.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gimphxbnx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsdqxlxfb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqiktqlso.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gitktvbrz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gzdrkgnhq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gdgsgfpnj.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gedalbasm.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gbrxfcsqs.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/goapkkobi.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gtsxbehud.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ggagfytkb.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gnxgjfsbn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gtwzjltuq.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gwbsdkvqq.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gbafitrnh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gurhfgwhc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gmaqkengf.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gwpylisxt.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gwtnnodlg.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/goualhppr.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gocymizkt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gwriytaij.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpfcuwqgb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqpkwwwrb.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gpabbilns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gcffaklzj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcfofggh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gttiufzld.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/grojvjylt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gsqobsxsx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gvcgmyppz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gjjlfdumt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gxzuigsnl.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gbolqxuyb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gtqhihjhf.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gehvnxuhb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gwtlvwpzj.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gkvlespsf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gpxirjbqx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gmmrspilr.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gitbxadao.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/geagwjcly.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gdrkmztqn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gpvzyxclh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ghchtolnh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gehdocqgf.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gbqericar.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/glmwkagyd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gfqmbegqj.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gokjoqnwu.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gdsdvdkxc.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gnkvmajle.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gppjgrldg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/grwoiiscu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/glpwbuosg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gkonokdmx.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvghwhphd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdoutndoc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gofjwzlxj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gqqkhqgnr.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gkkbhcbns.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gichqwmts.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grtchpyzp.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/giwzrqskl.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gmglaeqvi.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/giakzeugp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gelscvwsz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gxelllkuj.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gskokyjbu.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqxaiah.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gkrlqptyq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gyzjngxpb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gkocfnmcr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gtuvtxmkh.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gfigmrovn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gvwmzmlso.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/glksryjbz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gxceifeut.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gtwzdjqgc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gyunjszqa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/grwvsjbqz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gpcfzmewk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvpddgbag.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/grlotpavt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/ggdkfbkzu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gbuglprjl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbucucfju.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/ghcplgzvt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gnxamwswg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gcnqacvce.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gykzzuxgq.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gtenaojpx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gqilpgqkh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gjxjfyaqi.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gkkwkxufm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gwzfgppin.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghyveuqcs.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gilqvwmau.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giplojxkh.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gsddjybbx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gdxibmxqw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gcttwhijz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/grimyqpaj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gzplgacpg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/ghvamdcqa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gbxrbizyy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gaplqzmqu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gujkchdxp.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gskozekox.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gtgnrlukg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwckeabby.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkpzzooml.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gpthsjdhh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gszsowpmf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gulkzguak.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gjtuljndg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gtcbkcppa.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/giotxrdux.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gycykephu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gdintndqo.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gngheuczl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gembqudxr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjaqmceeq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gxiahhosg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gbydvkfrv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxyxxghms.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gyvynxlzw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gotjuwzjz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/ghsbsgjmz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gpghrjhzr.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gyfqeniww.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gghsqdcbp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gryiglkgd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gpwrvovut.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gcvvfjpoe.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/ganmamauo.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gfbpuswyy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gbqwutahk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gzcgmpnnn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvqrqvgja.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/guhbxwidr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gmrrthhac.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gpefqjbvz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/glyagafnn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gflvfksfi.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gowrhuqfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gnezsqugb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/givvnlnbr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/grhcomwge.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/ghrxxcikl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gfeebsbin.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gmbmfvfzu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/glcpvzrzt.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/glslemcoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gdqjdosjg.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gxjamqkuj.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbyhhohlv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gljbgqwzr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/giqfyhqvc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gcoglqizk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/ghjhfjnsz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grcvkvfpv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gueahpgwy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gnsjwdwam.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/glatgfybv.sHtML


<!-- 参考信息 -->