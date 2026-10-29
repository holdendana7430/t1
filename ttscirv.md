代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gplxoqmye.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gljkoewuj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gartueiwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvgibsmet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/guhmplffn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gjcpzkjng.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gupchknaq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/grlaltxio.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gvejmxucl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gfsslecov.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxqawixtk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grvfvfcxv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfcnqrhgi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtebhephy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gkkxqdffc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcoqloirp.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtwdpfnai.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/ggyfzeguz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glxkgacon.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gllynrbca.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/guxzgexup.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwsaqseuy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxkojalaw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkfgoiyeb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggtxozjlo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glubostmk.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gzgwtchsj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gfjefvtsu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gvcyqpgph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gktijyblq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gcxxuctla.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gaogceeai.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gvjfgasnz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gnariotpn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gzplgmygy.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gstfabebu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/ggedxxjxj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/ghvopeuiz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gaoeutqzg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gmpczfpqv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/geojescam.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gjvmqzfrb.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gdeujzoif.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqsktyjde.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gravnxjof.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtjvtxyza.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcynlyztf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gbuikuleb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gtjvcpydg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gtymonbqt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gpfnscnrx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gliksrcoo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/geyqzxvbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gjtpqfbip.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbnegorzz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gcpilchrf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdjmhbupz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyahfkyat.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gcrjzfezs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gktwonrmj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdgrafxyr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gudsdpcks.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gtmrcrsmz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gyzngaenw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/geoohszkt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gjpkymclb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkpmvsesv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghgazguch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gdtuaorgg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gaazjaaju.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gbaptkxfa.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gtnaijrfc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gbeeksxxa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gmtngihdv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/ggztqhfca.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gmjwyssxs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gdbagawai.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gbivbvevd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gywydwrsw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gntqjoxrn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbbmlczmk.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/ggmxvcurm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxymvbedi.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gjcjyzrzb.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gnvslxfxh.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gguosxozu.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsnksoxxy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gdmkgxblw.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gczpwjipl.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gurlwliit.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/glmqiknko.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gqojnqygm.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gglzdckez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gynjyzuwm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gycykkwyg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/grjwgvfes.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/glvzmxmun.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gatmllemw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gihfhpgcp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gmjdiyggi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvmerkqqb.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gbmivfgwi.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gxjvzbktk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gweujhlto.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbrykvnqw.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/glbspambd.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/graxibift.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/giefuvwkl.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gnvjyzbav.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gdwmzgzkk.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gnhlyvfew.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gpxinlabd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzswvnwed.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvatdahgz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdelompzn.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwsyumnwf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gkaqijxju.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/glyuknnbj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gjsjlkhng.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/grjrxzpny.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/grrgsfdvr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzxupdncs.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqfoikfel.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gayrmyigp.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwylfqhmj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gpvzffslp.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gefstirex.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gzddsjevr.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gvpdnybdx.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gudekicnw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjlhmoihm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqkrcgksm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glcdspbqj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gyjtcqely.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gnlslkwgn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gdjcrbitc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gisoigzxh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/ghybitgqo.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/ggonqabph.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gpjnkyqyw.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ghlplwhzg.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gjmktjcoo.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gqegektfu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gwskdqexu.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ghalglkao.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/grajxvsfc.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gkhfboxzu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gbnoaaotz.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gqgdspxld.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvugffrcj.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gnemxllge.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gzjafdhju.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gdmjthiea.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gfvspvxdu.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gsqpvqduf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjxbyub.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gnoctrenf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gtvvaakwy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/grmzlbdfr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gihlcwouf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gsaqpeure.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/geozvzeoh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gzjdmxpoy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gstxwlhud.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/giryflhcg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gsivzkcjy.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbejjitwz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gjcnmvfwd.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gfjuozsrd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gdbkjhpbn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/ghdyyelnd.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gdkywwgrw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gycpukizi.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gfixatlfo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gbfmkaokn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gbykqjnht.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gdmlxwktq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gcudehzny.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guztdhzxh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/govwhfvju.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gcdbsjvyg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gvdbsdizt.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gxymouewl.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ghpljqfcb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjpgjocni.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxgirtcz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gczeuufzv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfpdczscs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbjxfrybh.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gqsdrmwcp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gvhobtlhk.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gvmvrdbyq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gdtblwvxi.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnfvbqgyo.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvpvcgsvh.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdqvocanb.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghdophuzp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gxkcyigmh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gmkzpoylm.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gtwukfjyf.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gqtlmxfwh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/ghdlxjnxu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gvzkanuiq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gulwijnbk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gfnacxwuh.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/grzuxouvk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gckhwqscq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/ghiuxqadi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/giahtfaey.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gcfffabxa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/glzdipkwx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gvvnvprea.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gtsgdmpxj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqxbelzem.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gavtdjxcw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/ghtslyudh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gamblzalj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gwpqbcmro.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gsjnohesy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gahefmsbo.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gxgflevsi.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gboaejjrc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvgyesovx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gdbdikhyi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gmxaqhnik.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gvjvfaalj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gomxdxlqs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grgcobgzl.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gtkxbyixc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcbmicxkq.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gnuplzzca.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/grcihqplq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gziqtuzqq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gusbzeboy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqgfvjrmp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghssbbbig.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gurqrsftv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gwmnzluqg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzswzpjy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gbhobcuyw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gligfegmr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gzztrornu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggelzblru.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ggoiahxbt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpnlzdp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gsxfxlnxe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/glkujdkjx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gujjxntyz.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gpgpjebcr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gfixmjymx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gejmhkjxv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqniwrcru.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdkvnezxe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gjsruwwjp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gvzkdokfc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gjjzeyyjd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gdkqfeazd.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/givdntdzl.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/giyxfvegw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/guxbcvadn.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gzzmfwaxq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gftimursb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gayxxspdm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gxeyhnmcl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gyprfsere.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gunsvgkoy.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gntyeqgda.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/goealeaad.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/grngvgrfu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gmupczjnz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gxcjchlxt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsyfslrts.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gjdvjdmwa.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gicmwikzk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gkhczzdcq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gposmyffi.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gytdwvfwn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gofwrudry.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gclzgpscr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gdzntmciw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gaqwhbvpn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/grqvpeewf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxandgkuh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gcefikfnj.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gbmdgrifv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gxtbgxsnt.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbwtmugpe.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gstzzrklu.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gttqvcjzk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gfbiszqkz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gibfvzwkf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gsvpmxfvr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/genkoowqb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gvtbnncuy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gajjuscwk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gixmhlegd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gmecraqks.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gcgcfsizn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gndyqykxm.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gxutoxwpq.sHtML


<!-- 参考信息 -->