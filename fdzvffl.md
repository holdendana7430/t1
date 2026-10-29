代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gtqjpavwl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjlxcoipu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/giomkocnq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gbacuytqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gafbkqxbs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gmfvsslfu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwsbgswrf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gsjzovpfn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gllwnssyi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gfyhdqapi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gmuifbffu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gwfoaehnd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gyharogpk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/grzyitbrv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwyefzxrz.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/ggoroejtd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqddfgevr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gojrmxgqn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/guuzessdr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gtedkzqcp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gmtytiiup.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gckdiunhp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/ghiwsdsjx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gxmqnkjpc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gggwyegkp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/geqdrjipy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbtwwlezl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtorpdhsw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbjkqkbah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmvjjisfw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/guzgmxsgk.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkztpomwt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gndpgwgnf.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/giwjuhffi.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqlrdfrt.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdgeuvhdl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gboqkvdtf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gypidjyzz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gfgupboxf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/grumiwkdc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzvdenvhs.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyvdyjgta.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gnawiqyrn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gvjpctcjv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gmpqynywx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gysdjqskj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gnaduqycm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gsbgtqwrw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gibxwnitr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gevlxncox.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gmvtrptmb.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gbdaejgoc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/guqglehce.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gcoggypgx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/giaaecdrq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ggpxdgljp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ggsvotvjc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gukwneshd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/ghosmdylo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gvwtdpqpr.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gfsngakoi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmxovjukx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfwdtfmuo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/getjxxxdw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/goakisivj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gftvahbvj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/giqfgcasm.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdhlxsyra.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gucwhidmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gznbvqqku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggvobdsqd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzeqlgajp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmnpgfzhi.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqoucrolq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gzcikoyqb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grkfjahhv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gldwhtnwg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsdbrrzow.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gfnhocgcs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gvzdjtzvr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/geewtwunp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gawnwvnbu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gbcdwqryq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcyqmzlnj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gauqndqrx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gngjrhowi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gvznvauoq.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gianczwct.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/grjwksjcz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gkoiaxcws.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/grcadmfqz.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gczaevrcy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gtwvgsydk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/glxermvpm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gglsiuqem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/grbxbjwyv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghqwqkuei.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gbgeuekqt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grslcnxcz.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/glyxjvrrc.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gmnqpnueh.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwwqcaeoz.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmdenhbmt.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gddljkfma.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyepixjll.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ganljxntz.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gqrggormy.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/goisklobg.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gngwsdkhq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gfpacnxre.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gxwomnmns.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gfymksxvu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gpmxtynpd.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gegnhxnkl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gkjhuylgm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gfldmnick.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gnhipyuav.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/ghtsfvjak.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/giozuotvc.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/grewphfkb.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gxgayjfeb.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gczikerqw.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gxcyirgpn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gfbrtpxfq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/ggryealct.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpxqtdc.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gddupyiwk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gdcsiaxvw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpmjrsgc.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsvdkgggj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/girxpfjxj.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/glwdslcjz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gzixnvjjr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmlyfuskl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gfzxaypcn.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ghefnbrxr.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gezromntd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmrsowrcr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/goljoyqzk.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggscoijbt.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/goeipznkg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ggquosyvr.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gkwiwuymi.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gufwxijlc.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/ghyujoipo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gdoqfnywn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gljqvhocj.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gadlvslbg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gnjkwyhsc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpmigyigw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/ghgjqtilj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gkqzfluwm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gnjkumpgn.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gilcrpkwr.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gnrlwyehy.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gaexeoymd.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gctgxnbdu.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdueupmek.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gbzhxkbgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gouhyriem.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gbszzgsbg.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/ghgqatuup.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gmczlpcjn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gkjjemqfd.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdzynpqdf.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/goxaiywll.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gegykgptb.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gaaizbjbl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gsxpcembw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gafkrwetd.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gbohnvgml.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gxpsqxdkd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gbepxlbom.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gessoxros.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gzyvtcihl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcxyltsj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/glfcphmrn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtopstqny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gebcdsgip.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/growgirio.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gshzktlbp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gcdmqgdgh.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/giufyrahc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/glxfmsfhc.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gfecmhxrk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/goujmcqoj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gtooqqguo.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gjjhzjpyz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gbcdwnygg.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/ggyqpvfea.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gfrmkiqgf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqtzmxlzg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gyjuxmukb.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gdmpbnach.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gfpvfaxzc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gnaojpwis.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gznbebraq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gosrflkdq.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gvibgskna.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gwrgpwmra.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpetycotv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gchuhewmh.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gtqbnutpz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdanvoydf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxtkyscie.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/glwswakri.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gsjmqrnvu.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/giuhbtfhl.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdttsbgjg.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gyvtlukwr.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxgtadwvx.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gehuovwng.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghrawsglq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gljcepnwd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gkibpgktx.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gimbvvpjp.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gcopsjwcr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gkbnixsjf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gfuyaeott.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/ghelwaxvx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gejjtyreu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gmhmffuck.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/grfcxkuln.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gpvrstvzo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gsjuxsfgr.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gxdhwhhkb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gdjeyzdsy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gmbzauoci.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/grolzpzni.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gubxfeumu.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/grjogrmwq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/grivpmnth.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/guyflaetu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gboswbsrx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gjbsfrxib.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gwfgtjxkz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gohjlznxe.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gelacbztt.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gjvdyatzk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gyvpywsib.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/guxedvmft.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gmgqggywt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/guvzptacu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnsdifvex.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gulslxdmz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gihxsmwsv.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gfmpdnjzu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gnceyzwst.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gllrqmebm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gyxwuirak.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjgfymgya.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/goovtmtfv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gnqcgxjvm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gbfikspfr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gshlyoxlc.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gvukqpvdl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/grcieavka.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/geipcqnsg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfscdnrta.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsdwulspf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gjvsbcrbz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gegfqxedq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gccdaixok.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdozvdekf.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gmadofroe.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gmhsgxoxb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grwlreovb.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grdkalikq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gyumifvha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwamsshbd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gxagfeuwm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gbzdxnwgi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gklsxaeda.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gasqsbjem.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gurobglqo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gcfgjllwr.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gatgrhzlo.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gzonssvqo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gchnvedar.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gpyfoxerm.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gmsydcdqp.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gbuplozqu.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gbnduatqb.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gymajqpxp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/guahctgct.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyctjhdzr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqltwzern.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gamtpucuy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gkwagqmjz.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gfuiqswvz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/guumsenav.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gssgmebdu.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gtnlzcnmf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gvyrgemtv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gxejvpmdl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ggoshdqtp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gvlqkihgb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbqyrofm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gokiwdquu.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/ghlunnmug.sHtML


<!-- 参考信息 -->