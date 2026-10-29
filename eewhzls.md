代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gdcmhzloh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gnhioocmp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfaotrdpi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxtasekwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gafonnkbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gbinlrtoa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gthkitmkn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqitigl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gwgoqcbye.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/guyyztwjd.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gchgbnxfz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxgtgdgni.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzacpijnj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzukhujoi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gwadqforv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gggfhehiq.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdxlijloi.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gihuoctpv.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gomrtkffm.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gedcgznss.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjcgrakek.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gudvalcwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gwxlmsdvt.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzkmradga.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxwkqmhob.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grleemqzx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gdovrstmb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtodcabii.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/genofitkm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggqqqxrwu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gzohvmyot.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gfsdrqwrk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gqooimrib.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gqotbhwfl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gfxqohljk.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gcguxektx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gityxomth.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gppsbuhik.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gskfvblmg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gxrucpfcq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gnuwuradg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gkgfgiblk.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gumfqsifj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gmqqkkerc.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gqxwdhtip.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpurtmbmm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glijvctjk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdocxczdd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gayhpxzqx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gdqweuftx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/glambnfkl.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghdcfedxs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/ghrnlynmy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gampcfmeg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdyoifutq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkuintlip.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbwzitlaf.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwdjyvvfo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gjrjpjvjf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grbixwcxt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glmmdwxou.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwaqadgrk.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gekizmhvf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gzplchujm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gyskewjcc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gutzalrwa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gavuggaem.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/grwjduumj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gencwpacz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfmdlpmil.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gnwgcaxgj.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gokdurvur.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/guauxfuwi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gkmpyzgmn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gsfhohrrv.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gitmohxhk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gpmfavhba.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gbtfzxamp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/ggcdagagb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gttaqyhkh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gozxgqkdr.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gymsrtmhu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goojminjb.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gizqhvscz.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/guimsvjtn.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gwhsqhqwl.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gerwydcal.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gmphvlsci.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkfladfci.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/givmdqexs.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gmznrtktv.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbnwzajzg.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/glefueeat.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/geigtzwzw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gmsinomnx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gqzyfupcq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/goigywrfj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gywjwbdgl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/greonfwxx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gozjwcqcg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/ghzerqigp.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gdcpzrcpe.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gtjhdmfmp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gbgldbuus.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/givbkbohy.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmfruanss.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/grcmfcnbt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gzfxgdebn.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gxundisko.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfudtqhlh.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gypsuayuo.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gsampdiof.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfqcwenpf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gkdbwfijh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfdahlmgj.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grhpnztuz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzqehzeup.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gjtjyfedc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gzetfmdam.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gbafcfwxk.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gbemoqrau.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gndvssygr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtvieobwm.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gcernjmew.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gkrphnapn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gzrjsafdr.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gnktexcpr.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gdiwmxjuw.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gbgxsqkgo.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gmdkqywfi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gocoahdyq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gksyqpbof.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkizmlcog.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gilflrxnh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gbhqltwjc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gopmgrrjm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gmwcxcfbp.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gfitkqdyx.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gvblpjbim.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gibocnmgt.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxvofuoxu.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gfxruzovj.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gjlkexhzq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gaqlzadvq.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gigmzwouh.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gnywkgmgz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gxabvxutu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gwaspueah.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gpdxywmgg.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/glshomrwi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxtuosy.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gfkrhtuub.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gyanbpmow.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/guckoapzc.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/ggapmdqyv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/ghhdelkan.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gsypsgbbe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gdnsbgmjn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gtaqoigrw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gcgpdxwpc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gplbodwgr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/giuozxlbt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gerwmburn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gndxiqzmb.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gabspqyrt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gcdcecgws.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/grudxijra.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gzxchsvzp.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkhtcxgoz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gbynvbjud.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gvckxyaeg.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtmugyohr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gtfdukqjh.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gaqcebvuu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gjyyygbrw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gvejvfazi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gysgjiumt.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gkjrnfxdo.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvxqkmdzc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gahwolxjb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gfniywywv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gycaaebeq.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gnnakjkeq.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqcjkrlvo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gajsectle.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gurjipmzf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gcnijhlwy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gkviudcmi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdlkzknnj.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gvndohnxc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gktevdesz.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gptbgwnif.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gisdqbuer.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gzwuxdthp.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsjdegqvm.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gyorurrxp.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnndwelop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gfmflegob.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gixoxsjbh.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gbjmczuke.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gjhkfvhxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gmgsmfhiq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gzenskeoh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gmniethph.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gfzcetqha.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gkiuprsho.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gxtcrjxsh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/ghffdajfu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gkignqdyz.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gojhjponi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gfxnaknpc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gvysgrjiz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gdsvkwdyv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gkepszdta.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gglmyilwr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gzxrauljv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gqozahnsl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqqpuenif.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gecloetmm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/giopveskx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gptejphps.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gpjitbfiw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtletybi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gajvtvxbi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gyhuwmzkd.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gohvrlpjg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/grmssfiid.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxmdbmdpl.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwtvaqpaq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbdikskum.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gmumukxdq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gygehuvhj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gyeonnkla.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gwbmyvemx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwpawbgot.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmmjkotq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gcvjhryjc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gwaorzkqf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gnbicjndt.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/ggdlkwoin.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gtgezfxrc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gijmotaeu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gmpzspwki.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghfzppqgb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gularlirb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gvuwfyhcj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gujjznytr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmhbgaxyo.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gsfnokedb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gxpsqafrt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/guacsnice.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gufcdyuqa.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gaykvjykb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gnmoirbrr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gncumvwbo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gzdfuuane.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ggidpnbnf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gqmmiciip.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gojmvlxit.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gplgtwtpl.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gkykcpvvd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gcnzzkspv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gcfphjcvg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/grkwjcada.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gbqldsyqt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gcujemfhx.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gjrjqazou.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gmqptihzz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/getgdeexo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gdgzxqvqr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/ghhsqmkjl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gjkhfdnhq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gtwzywbml.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gtybqhlml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gczvdtrkr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gdezjsgzt.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gsvsculhh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gyuqtbvae.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gvzbzqakp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gkzwwceqt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gjthanbjd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gzidbapwc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gjfbgqoxm.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gnsvnyauh.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gugqncxnz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gnbbzyaoy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gdlaeooqp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gdnoqelez.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtmtnjlyz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gdpdgnszl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gzdearpdk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gijzkcbuw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzwhtrvsq.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gejlydxhw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gdqqbqcqe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrxecih.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gltkdazvn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gwpxbfund.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gypkdpzqv.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gaenewkyf.sHtML


<!-- 参考信息 -->