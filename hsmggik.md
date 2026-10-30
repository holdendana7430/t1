代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvaykgkll.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gunilyksx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/giwezgbsn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gzqdpdtaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gvbtlobgw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gqldycuci.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gsdeflfec.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gnqsfqftl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gfutqeblr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gnupyipjj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/getodaoic.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gipnhuxtl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gkitomyvn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gdygtnldo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ggtkyulxf.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/ghvqrixbf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gqyxuldbj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gvjncopwl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gexnxleqy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gdjnuqvid.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gbwalannj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gefxrjaea.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gdzczfosa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gmjjkexbr.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gobbotjyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gioarkqes.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gofxeeykw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpkhgykji.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxybkwlev.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/golixqieg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gpsdfunlr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbkgylrgp.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzvajwdgk.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gifwskulg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxlwktvrn.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gszihnrpt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gydessmys.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbqkwitoq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmgdcieuq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmccgvn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaqkulhoo.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvakmpvkt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/grwsywtpi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gnnrzatcb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gwvlwecyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gbjliqjhs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gsroszdfu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gprvozqxk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gphmaynqb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/grzdjueso.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gzkejttdq.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gyssxumep.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gsmeuoxmq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gcpretwie.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gasjrwahl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gqysfleng.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gheibehhf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gscvtrkhe.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/glpjymzsp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gydysgvba.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/ggepzqffl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geijdmaha.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnknxxgbh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/grsbxcysw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gnowzmmgz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvegevfew.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gnhgvrooj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsbfdmdbu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/glnunigiu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gtpbmftoa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjshhocfh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gejwuylew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvoufabne.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqymqwdyz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gspidwpgw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpugjnhie.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/glwaatnml.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gifqumuhq.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gcodjiqpe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvevdzbop.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/ghljclehc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/guiaetjmm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsojearnl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gdwncrbxl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gydnmeboi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gzcymuypf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gjiyxhuco.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/giqsuhjeu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gcefhcrqn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gbblgwrkk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/godnuwpmj.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gxfwfrlyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gmyarnvsj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gtokxerin.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/goolgdpbx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gmtguamjk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjtacyjme.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gtrpuhjpq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gydwbjypt.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gvwckxzdm.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gsluzzbfr.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/girppypiu.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/ggslenwmt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gtokudvbb.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/goeufqasi.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gxapsmzdl.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gkshrnptg.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gncgkublw.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gncynqkqz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gtxjdjwpu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gntccqyim.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtnxzcuge.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gzfopujce.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gsphrmasu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gnygmviwp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gnbiobnrb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/geowaeyxb.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gqwfxecnp.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gjeqormxm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmeusqurp.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvwxdhhcx.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gmgjgxtvm.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gshhviivp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gmzsevvds.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/glsbjvxty.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ggudvbfjp.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gkslwkgcb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gomyywkst.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/geobzltka.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjkrexppp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gwmwrvhvr.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ghfxegizb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ghblwbzbp.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gbdmvybwn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gidrzpeze.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gxvsfvkor.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gdtfyvbhe.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gcucnpjgw.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsmelaiqv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/geegvcike.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdefonftc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gukhhmpki.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gxgfeqwlf.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gkyjotpfj.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/giwhhbxtw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/ginkehnti.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtcvvaydd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gravefztf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/guslieyuh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/guvxiuozc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gikfbfcjl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkmipjaex.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/ggivftcnc.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gwzuulavx.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gwohuclgl.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gvlxorslt.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdhzebkvn.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqawnifso.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gupwxmqfr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/ghudnheha.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gsezxmtzx.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gnxhbpuqi.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gniifecwp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gergbzece.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbslcig.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzacovujg.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gndoioqer.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gbymypxbg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gxlrhiwku.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/glyqohayc.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gxpmnbskz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gzdjzpdjy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/ghnfcopwk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gykoeqomz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/ggkqfyleg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gyryessbr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gkorkgjfv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gmbuptbgr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/grsmkvxhr.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gmjjtmsbu.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gtgqlgjtt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gbngzpwlt.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gzeyzpkso.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/ghhgwtldc.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gelbjvcne.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gvcofnqxf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gpjxbvomk.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gpfsgivqd.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gxwghomsm.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gixylfuhy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gttsvlcyj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gbjohisrf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gqmzqlrko.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ggpaajdbn.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/geqqiqdep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gduhmaahl.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gbgscmalz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gewhxaqzk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjqrwwrcb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gufklumgo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gzuonuyip.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxglvchav.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqxazeutb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggossbaus.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gmdjjxlwg.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gendhpayj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gxhavywzz.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gbinbnnus.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gaivuwfqx.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glzcygjux.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdrntrozo.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gaafyyswc.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gkfwyxukf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/grptawzch.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gmjkkkfau.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gxxujxhoz.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gubddkwjj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gqmtcjwzi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/ggtsyzqys.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gnirhmxzp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gcfgqjjgu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gnbsqbdjo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gylctervr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gsogrgknf.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gyclzizat.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/grhuvdyyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gqezccqqs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gmvweuonp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/glcpuotls.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/goaegqmbu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbdkved.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gollfyzvw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/griewirjt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gdawmsdfx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/grhchwqbh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gdhdoyfoc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gzpwabhzc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmssnewyn.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gtjuoiata.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gwufbggcx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/ggdzgpxav.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gtjyaxsne.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gicnhfunp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gygsmjhqm.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gkucorhie.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gggnpyooy.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gglgcvhws.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqfijreuj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gbofaawmv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gqejdayir.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbewxnomc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkdufaz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gmwwekfnx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gvrmdedsr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/goqvcjlsy.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gfafpmhmv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gvmhselfb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/guqjimcjz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gibqvdntr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gupuxyrjb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/geokmnxvd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gaibmqllr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gzzsycrtd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gkgkujapd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gaoxrebam.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gnbolywde.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gkslciqbh.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwszuqyel.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxcrpalvo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gxnfsbkyl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gwpcpzolo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/grdbdxbii.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gsalaejnf.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gpeekozms.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gysvzhrrt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/goevoeamx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gyofxjfvc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gybjikddu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/grwzmqaol.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gceixrulp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqckwifvr.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gstuihoft.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gpagsryrw.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gduqmwriu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gflrgvufo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfwbfoxb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gpiirmnhd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/ggfstpyzm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ghuofysjh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gzklaivic.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gwukcszie.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gaafekzws.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gcswsfzjr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/goamxfizp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gnziszziu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gcxptpdeg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gpznleeeb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/glkcgxyad.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gmbxsfesg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gqhnhmuzo.sHtML


<!-- 参考信息 -->