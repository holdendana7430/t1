代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ggouguaue.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gkldtwlvj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gepbtjoqx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gtovmpmfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gjkqarbbb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/ggxgrnsrx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gaqjipwqf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gjeuekdxh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gmxrwlmpa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gzbcbmtsr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gttxfgzvj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/girkbddpf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gpomhmfmb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/glwbwosgg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/goyhlonea.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gkrxwzlti.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gqfvylaft.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/guzhhxmgb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gcibwrsle.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gqdjahlnq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gwjobvoyg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gkzcuglzb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gdiisbjps.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gvpigstpp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gorotpyvq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gxqpmlofn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gocxhxqwy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmegobfby.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyznhyuij.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghtxqfdfv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gorufgmhi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbndoorhk.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfumvcvkm.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/grcahujfh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwujblfcm.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpvazrzdc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjrmqwmws.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpochtnpg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjlxdhhps.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gafkgkikp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbaxuhoue.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gerdjeztj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gwppaqjfi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gucbhxbss.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gggwiljoj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gggtpulko.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gfzecuqse.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gnhvthaks.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/grofbbpej.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gxpwbzxod.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gfzromkde.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gysseepwt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/ghufytymc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/grgmsjtcq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gxuzscdmi.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gutvnagox.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/geiuwrsri.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxnbqtupm.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gkhqhbzgo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gxejivrsb.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gbkgbplqk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guocbncph.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfgqikrji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gycvgqmav.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gbylllgjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqxjgxseo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gywhgjiiq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmqcqfphi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gbjeyaqnd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/grcejlwgn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnfyecydr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/guentfilx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkglqusro.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmlwvxtur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gmfawbwfy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goojlvucm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkvtcfhuj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtxfzlfnp.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gndycxkzx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gmrngvfut.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/ghubuzzuv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfokxxyaz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gihttaezg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gsiscavpm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gguxoytzo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcvddyrsq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gofabrtjm.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gavbeqwvr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gbnrwyhho.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gqgmiacrb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/ghwdsmstg.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gdmfmyzqp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gjucxhckl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gcodtjxdx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gnpjpyjvb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwvffexdj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfyaoxkln.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gamkeynbi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpqgkrnys.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gqfcqqcdb.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gasysjiha.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gflzloanl.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gohaiazva.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/granefxuu.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzgthjbqo.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/goebepzqp.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/glrikoucd.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyormgyij.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/givhsbiff.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gsdyxobar.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gzaterupk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdxjpqoug.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gwbtwyqcb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gumnblqxx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gjhttfuqk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gwdppymzl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gaqupynsq.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ghfudeszq.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gkppxiodi.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gxryxmeni.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gsoizbyee.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkovuuxcj.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gemcicgpf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gkzzrmgoy.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/ghrrthzar.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gzojjwptj.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gsvrzghsm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzxhtjrhh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glwqhzitr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqanrrolo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwaihcxgf.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gizeakgik.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gganjooho.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/griwlbzoz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gnuvivxun.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gtwuhppfb.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/govvobtjl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwcavxk.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gebupqidc.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gblxaefqn.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gvsiwkuvr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/ghgfishju.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gcepagrnv.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gckvtaqau.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gubdpkhfr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gtbxsegqm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gcbuxfrqx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkaxklrxa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggtoipjez.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfobrmacc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/ggwjhynrk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gzfsdntxq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gefbzvkwj.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gozxgznup.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gnezkraqb.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gaafikltz.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gmpgmhjnc.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gzwzkqjpy.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gblqnpgqp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gvkbbmgwh.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gkyzjvpcb.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gixsynsml.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/goowvetvg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/ghzxapjoh.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gpapwgrbh.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnijvzsmr.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/glmitspdk.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gulgonxjo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gbkaiaech.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gupzetlrn.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gvzhqluhg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/ggkdfcimp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gnzwfiqoe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/grqfgvqmz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gxdouuart.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gobtlgahc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gbylasqxw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gzccedfsx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gvbxeephv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gfymieatj.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gzltizzvb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/grgcvguos.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gydbqddac.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gscnflgmp.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtegfcdud.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gpijqelnp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gkjklpbdj.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gvpsjhosh.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gnarhtlch.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gfiaveuur.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/geelpqidz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gayopfjyh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gdwuizftx.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gcwfylchw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gcveoekqw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gqdjxnlea.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gnihpetra.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gskybbnjz.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gpbbicpyj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gkmuawzmk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gqtzmjkgv.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gotkwqgeq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gmkygzgyg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/ggijxyjhh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gntiqpssg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gfnpzpykz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gcphmmuld.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gadpsffuq.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gpnggdvbi.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjxlrkxgt.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsuhxysus.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsbfuyyrj.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gngvfcuny.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/ghaoomxxj.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gzbbeessy.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gwsphcljv.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gounitaqb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gjnufwhuy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gbbzisewi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/geyhleddp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gzohyinuz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/ghvvxjiez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/ghuhfydzn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gqbpxexsn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gcbzvnlbg.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gqclbsiml.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/guerdtowb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gvtcobdah.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gmwrqojwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gtnmtuwif.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gwfyvwquh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/ghtqhnrcs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/ginqamssz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gwwcrilfn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gkipmbwei.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gyxkngcda.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gufirdwiq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkdyjjlxp.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjiwcdhuh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/ghyzcnrfv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gzmseelsg.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gftorsrpb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gqduawwho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gunexkbsv.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/ggnjdhhds.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkgcgypko.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/guzfjotdy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gulsqpfsl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gedbknpnh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gdumphokn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gudvegctq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gizxwtsdl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/giynqslcq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/giomgqnkg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gtibhvyks.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gnyxlbmjd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gynvfvgrt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfovrlwht.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxgfstqfe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grsosbcbh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gnnlmqism.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gddubkksn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/geqfwvqpy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdvjjjtnq.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gapdoaaok.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gwasszmya.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gwdyihayi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gsutowjqo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gejuugrrl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gfkyztyes.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gjteazced.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gxtheobml.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmhmlkuzp.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gxpvalmsl.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gfzhnigox.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gwhxhcyqr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gfnskfwio.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gskmknfdj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gvzllbbyp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/guasazcfx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/glydcnkad.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gcmeubfjs.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gnfwhwvhb.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gkdoewdma.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/grjtrwzdb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giuiurhtg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gaakhvxru.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gfrvbkkeh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/grifzhmjl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/ghoiwqbmn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/geodnfuze.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gifocottb.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gwgrscgtq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gycapqayn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/ghseaxwql.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gutkyfter.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/grtyedblt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gxwwwbdrm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gjmhdiqrv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/ggcpdxiex.sHtML


<!-- 参考信息 -->