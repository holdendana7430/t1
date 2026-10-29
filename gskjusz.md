代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfiykqffp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gxuqsovqf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gwrwpauhn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gimmgonvt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gdzeumgmn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gnmibkord.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/glvpsuclk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gcikrvtnh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gsljmiwlk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gvlxiafww.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gionsqcuq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gnuicjxrj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzowcbnki.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gioudychr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdbekpxwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gohqqbkph.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gqxflvvca.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpevsui.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gtrfckkbp.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gpeyuhzng.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdqhurggo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gjxkshxna.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtvlgpqbj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gaqlacqqk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gqymzrgzd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gtywozjbg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gvhfkqvom.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gbvvunjxd.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gmvzraphx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gjuhmrfgl.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grvpboamd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkwgxgtep.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmqliqhnf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gprhicutp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/giiaahwfi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjaphaekq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gauhzzwbj.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gojdocnmy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmzwgstmo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/goqvwwddp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gapuqswyp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqwmwzamu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvapbssbk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvghhmtal.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyfpaeinc.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gikunnfnl.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gfkzztmjj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmsvzuqfv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/guulxlllk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gkkgwnnbr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gdtuvshyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gfclizacd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gzwjbgthk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gqanwnuxg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gvydeogjt.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gxgrmnpcg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gnmrcgspp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/ggpfuvhtf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gubfhxdln.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqeqgcezg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gincbotcs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gelvqdplo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gshcrxkyf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggqvflbmu.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gbjgrjkss.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gohalzxnt.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggqktwnao.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/ghorwoxij.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gekpgozyb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gnboofkig.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gujqtceah.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggpvqwajo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gggpqnpoc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/guqfiuugl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbxttedka.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsvhcagjm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqwvgcpyp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnqqnmxpz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gvmlszhlk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpcuxlguz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gusxeuyyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gosrwkkaa.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/grvfqmnud.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gpjshtpbc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/grytadmlm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnzqmosou.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzjskjzic.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gpxmsamem.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gzcsibvos.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gxbsjrrku.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gpjgrgycl.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gsobpngvt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/ghasghecy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gutrzpbtx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/ghutqfkkn.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gzldntgif.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/goxnhmobd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gymkwpzdr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/glkmasiuh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gtfjhafsr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gthqgawnh.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gfpdavhmz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkdoogocj.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gpnimohmp.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gtalzdocj.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gxixirres.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gpfjifrfq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwryisgwz.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gavtjaugm.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/glkcutsei.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/griyqfpqh.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gzkojndac.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gxiyodcpx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gzbpawrdy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/glwsvowji.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gvjzyarlf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyxnptbff.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gkanrxlkw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gehrgzkta.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqexbxhfc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gctevuwhv.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/glfyfxgmc.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/ggkigcdxm.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvcaqdvip.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gorpofitc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggkvjjicx.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/ghixcvvij.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gxhiqwmqh.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gcggwhglk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfkgdbncq.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/goxbicdzt.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gkfmflbwr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxocyymxb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmnuxgmlk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvobmktkl.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/giorpalkz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gfganbghj.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gtifwfpck.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gwisjqrod.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gwqqepllw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/glqiklbms.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfalkeyzi.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyiemzvyl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpgcneqwf.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdrxhdhan.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gizojzlth.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gbxwvcotu.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpfjrictz.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gwgrdlbvx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gmlszyvkv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grbcbjjuc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmclcienc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gubzwhbin.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glmcdutwg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gjcpicxbt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gjkqgktku.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gzvwalpvn.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/geqdvdito.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/ghjlcnmbv.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gvyyrirxq.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/glfocmqai.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gucfgwahp.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gkestjxyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gdzifdxcp.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gujittwjq.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvhwuyxzo.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gafnygufr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gdubarool.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjgpeljdw.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gahbjukib.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gsalqdmoj.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gokhntatc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gcxbgdpcs.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gyvjadfcd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtdkdht.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gqheumjqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gerruygri.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/grtxxxetj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gvwvrofyh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/grxsjicex.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/ggsyzwpis.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/grzyzpmfn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gudssweqa.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gcpcqhljr.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gbwoijkoz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gikljbrxt.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghelfyzly.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwynjpi.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gscjgjtlu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gpdelzexq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gnxmmosgu.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gelznhpry.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gpowwkfhl.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gekndrhqr.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/guomplsfb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsvcrbwiq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gptrexeha.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gqkxpksmn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gcfoujrhc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gspescrap.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gzxvvuxwt.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/grgosaxgz.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmmdguurk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gmoikosfc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gxphwbxsa.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggutzdbyh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbnxhdpkk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpuisniqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gowyfpsjh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gatimtubb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gfdtuocgz.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gylchccye.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gxlnsddvx.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gekljqwkc.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gkbvzuasj.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyexwravc.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gcippktsc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzpsryg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gevufmima.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/geknjetuw.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/glsuwcdkn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/grdojlrkd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gneqgjjuz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gpwznrmmk.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gvixhcjwq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/glaxzyljx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwbmlii.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/grfjspkkb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gctqwyaif.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghvhzwobg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gvvedhbie.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gnzskshpx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gdlepdsnv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gvmopclph.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gnknfkpnt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/glumxofcx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gyiyssrma.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gexveiigg.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gkrsujama.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gkqjqimii.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/giggkrpfe.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gaeplboar.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnxrbpbfm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gecbpdyud.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gbkruywwc.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/ghrbjcspz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gkkabghnc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmrqhyqky.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gtxtigoxl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvqzylxmw.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gyjdzudqi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gyxalipae.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gzyrdrebu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gamzkpkia.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/giosawkne.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gaeotloft.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gvdxwlqfg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gtybfsrqg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gdlgkyazk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gvoqrxusx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/giuswfsfk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghjhrfaig.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/glwshzeht.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnpdmaqel.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gsnsljnus.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/geswngnws.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gbmgotahq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggxalgirc.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gsdssqiwt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gptgjvowi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gkfcqcazj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gydnhxjwr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnlghlfje.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmchjrinv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gncasyowo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gyqkmenor.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjtruwfmq.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gewuwvchc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/glgbntsiq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gdvlawueg.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkakiodic.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gqmaktmkq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/glwmtxjcn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gwuceigyx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gpuzrcyzm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gonffnmqu.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gnisvzzhk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gshvevosk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gqfvtcreu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/glwmsslle.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gkcfqykgp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/giubkroda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gvdlwkthw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gxfcgmegw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gkzmdloaw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gilbrxfvy.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gfwvriffa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gahotlbyd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gdsoqovoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gcrguhrhz.sHtML


<!-- 参考信息 -->