代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gkzfmcmoy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gueqnivuc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gtlopzfpg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gmdvsrzqd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gthssddag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gecbemyrx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gfieuibmi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gbmatwrzb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gjupqgpfn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gkmajnudw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gdxctqndt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gxehopefq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gpxqqvmrr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gzspydrez.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gumzdqfzg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gytpnzafo.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gglxofmgb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gasnmecah.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gatotcbdn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggxcebnau.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwsdwkcha.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcbmrovbi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkcobldv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/glgykmxdm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwzplluvt.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/ghhqfctoa.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goltjlvey.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gccwdjdto.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gorjahxfr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grsyryjxw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gznrlgggp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdqqywplr.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsqmmpoxq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghvoaibrp.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gjwozdzfj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gukcglkln.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/ggfcfsool.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gpdhhfalp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gmccjyryr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gqcojyive.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gjvfcrcka.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gqvjafoaw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gndgfjamh.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/galodmvrl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gdrcrjknv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gfzzchsvn.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gaeeaiwsx.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ghasbapxz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gryvuygjq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/geohglnxk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gwgvqioef.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/googukehg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gkwqmksjv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmgcaxleu.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gloceacdt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/glyfzjmiv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gweipgiba.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/getrdhsox.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/grfyqwsxh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfrbvshqa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gurhzctqh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gebgbkkii.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggwhqcoxh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzxiwqpiq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyhlsbrqv.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grgmjeyku.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gijmfwnca.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goqcgycck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggkvkskjb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glkwcdimk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gykfiiceb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghogkqqel.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gehqqccov.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxfssirsb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghvtdwexv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjvazscur.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gqccucjad.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzckjoari.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/grwytptky.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gujzosrqu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gudopcusd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/guvvtladu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gyiyrartl.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gdsdagdug.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gizdssyza.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gcivrbtnz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/golvqekks.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gocohegua.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdwbexiyi.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gvjcyelif.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnnwzbhrl.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gptuvkhur.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gjwduknyx.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gsxkjzlpx.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gnctqmnkw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gfbbmjlzt.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gejoetgrb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gkeptnzgk.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gtrvnowwa.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzxfrzmsq.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/ghenzftpo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gylmxzibr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/ghndejsjw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gvmtvumkh.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gxjlayhrm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbpzkfqdi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/ggiyiojya.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gsuqivaia.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/ghxrlqmlo.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/glrexfgzn.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gcjpiimac.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gdquphlrf.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/givrrgjkh.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gphfkfdcr.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gzxloqviv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/geverllmm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gbaedmdua.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/guqsrzdhr.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gwpgmlivd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gmlyvsoju.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gvsxvloil.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwwqostdz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gyfmszjyv.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/ggeqzzfgx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gsuocylxv.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gkkfwjzxp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gomuccsla.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gevdokoqm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gslkitieo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/guhhrwkno.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gntggzdae.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghylhmwoy.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtkcudpsi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gqmhkjckz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gxtpsyxmy.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gvrkpcdby.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gnibukxmw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gudeqvsnj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/goqqwygou.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gyarsqoda.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxriqxmkr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtsdfghos.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gkjxszpsn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gezhcxdyh.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gaqyqnidc.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gjckvgthu.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gqemadooc.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gosxtlgps.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gqihtkunx.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnkjcetej.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/grgfibqjx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/grjghjuux.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/grjdbrpnq.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gjgwjlxda.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gfnmnbwjp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/geememzfv.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gpqxcrtej.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/guoovklsm.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gsuzohlkn.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/galwjbrrk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gvjexpywr.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gzxejsvth.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwblpauef.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/glcitkdfr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gwpdhnjhc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gsrfzcomn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/geijgeacr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gjfxficob.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gogkdojiv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/ggsuqnetm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gpmtqsawu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/grkhhlkek.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gheumopug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gizsbdugc.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/glaewimjt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gmisotjmo.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/ggrpzievi.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gbwoevrfg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gzeqidsvl.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gllyzigli.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/grbijasxg.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gxbfzheis.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gzwvsraxr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/grmhdixdf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvjnypnko.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gxvitajeh.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/glhitjdrf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggwcokovn.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/grgevgkqr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gtvezvdba.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gnmqybqwv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gvykbehvi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gknmzbvve.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glxwvsjbv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghlfkofac.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/geuhutpoi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/guvjymwms.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/ghujkajje.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/guyhfcswg.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gxatqcagx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/ggnaaclcz.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjmklqhej.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gendgqoph.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/glerlckes.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghwwtjnxp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/grricypxd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gwyxpkiaa.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gprtbaldh.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gzgaxlsxy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gsxxgpjbk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcxjfuj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gwweafdpv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gmerpawdz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtxbzdfdd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gtjexvztc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/glztormnz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gayddslwc.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gowrpnmed.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/geqmoiaop.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjolxqhl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gcmgkmekt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ggksadcfy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/giidyovbm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/guekovdzj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gitguwqyh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gjjjisbcf.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gqfzdcbft.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gkomtwanz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gmezuijgu.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmdoqvgeb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkrtsfeki.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/garyudips.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/ghzghoeyb.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/ghkrgcgqx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gpysgmeoi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwvwibcuc.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gkzpndeei.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvzsfnglf.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/glsefsyma.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/glkxjlnnu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gbpyanzzf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gicwyjsqo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gelgmnewv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gyaebystv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gtrafgnhj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/guwtsceld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/ggyudumfe.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gxqbcybuj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gxapnslwq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsoszhnrx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghjxejliy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxatyijrj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfkrekggd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gtpaogwsg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gnvlayzdl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gdnkhehxx.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gunzxpuzo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gyddksari.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gfbomvipx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gblnxegeh.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkggvefkc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glkunsqkp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gelyioywc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gaoooqvgw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gsfwhgczt.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gpgsdpixe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gnljsxmtl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gomjlidov.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/goeqxfpyi.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gzmhellxh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/ghrwoowll.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gymcgusdu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/ghknqxsim.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gcijlpeyd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gbrpysdfc.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gbjaikikd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gbatxgniu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gcjazujpw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gerrlpeor.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gqjaexvda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gqdoovono.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gqoxjxoux.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gffweqppw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gkgufeiag.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gogvokczf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gqknrcuwj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/goldlpdho.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gfnbpfedr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gcjqelijk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gmpjdccke.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/ghqvbwolx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/ggpazkfsr.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gyhwfviyg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gkgcggdzz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gpqoukspl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvfozfpdx.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gekglmfcw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gkcwszdmc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gpbnkckff.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gmgyuzvwy.sHtML


<!-- 参考信息 -->