代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggnypkvmy.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpadlsunb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gmptyhmum.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gyfgmswba.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gvzrviuwh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/ghrdqklkn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glbniyvgb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gtiqiksfl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gbaatuwfl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gmetjebnb.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gmqszwovs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gabxfzmcj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwnuoysjx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gytzwrqpt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gtsvokjiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfehpwnu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gunsitnwm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gowwcnbru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzgjklqgl.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gpwurnuvt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzhqpxby.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gswvttplz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gvicgvzbz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpkmnnthp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gppmfrqpp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gejzkawfg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gndpotexk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gcstiicwj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gqcqakrrp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gzuvalfbs.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpcyjwbwu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfabjoxps.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggkcvlcqg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpnitgwke.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gcqjndxco.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvtjwpsab.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzkerhcts.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/ghcwqlnta.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnoowgqzn.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnsqmnpwp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gexpaztsa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvawxxbal.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gpafvvhxe.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grwwkgfbn.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqvytolet.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwkezlwyy.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gwlnnieax.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gqdukjzvu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gplbtktby.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggyryvneq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gtxmwwydv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gytbmpgqa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gtdxswtpw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gjvlkkozc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gaxgvcfwn.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gvtyytxip.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/glntmindj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbkthgfu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbizxjoxp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/grsoexogo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gadzglgth.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/giyguxrjz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gdyolayxp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gvnzxufaz.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gczatkahd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwfpftfzb.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxnqbndgz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gojzxptqo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gklmbrwxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gudwzslqy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gfhzuognf.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcmzgwvfm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gsptoyrtf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gwitryash.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glaybfcug.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkznqrjkf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjdipkubk.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvwovayht.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gawkkgync.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkphwsdds.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxifnwbkd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gddgfowis.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gbdjnofuf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggxwnmsbe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gamgxqruj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghugizdrn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqnhddrrv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gsdbjsabo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/glqmijtkt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfzqmmiig.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gepqorcla.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gufegkkwl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gmwcnglem.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gimvqhidn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gjmyaqyby.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/ghvwvtvbu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gwwgbkuwm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gyzyiafvo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbrydikvx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gcdciwotf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkmrfdxyv.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gbmohysrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbubyphao.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gpgjiitov.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gfdwdyckx.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/ghcnebrvk.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggfvmqndq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gdeazfmvj.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gtavjrvbv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/geithekwg.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gbbscjcqo.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gmbxtjlyf.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gnzeoqmex.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gcredxoxc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gbzmtcyae.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/glelgshwq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gaxzbuwdd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gpogkmvtd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxqktkp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/grfsfmjyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gebhpigyv.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gahswznfz.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gurdagdwl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggoiwvxsd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/glqyrkwxi.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gwojmarxx.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gcgjnshhx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gxdqwuwic.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/grxedkzwx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gdpktahqf.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gioapibkx.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gcwdomooz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gfqyoaoao.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrhzbkut.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqccwslpo.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/grjpkrtkv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/glsftxgdc.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gelslrndq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/grgjqojpo.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/ggrekytmp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gbzflcibj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/griiylsnu.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzkrbjrfm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/giiwitkvm.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqigwszfw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gghzkeehu.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gvynhvyje.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gkzopooal.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/glwmioocq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gbvbvefbb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsjgzlbx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnxtvaheb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbihnfwzp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gslijmybf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gptjjpzpi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gyecmvzgh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/guvqkvkcv.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gmcsgwhzd.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gbjfdtzpb.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjrddrjdn.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/guccwcuqp.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/grtuzhbzz.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjlflvbfp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gjmxxseev.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gkdvvduxc.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gyxxucvui.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gqccxudkm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gjufigrok.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gaqkbthwk.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gowiaualm.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gookofjts.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/glwpfnabc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gjzkercgz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gkershfir.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gigqboosy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/glczqmjdp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gpyvoonwr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gdadkzgfn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gtabissrn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gmpqoelia.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/geubftjaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gklvvilqy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gngtkplim.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmqlhmbd.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/ghcwnxadm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gqiyyhsrw.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gutwluwhi.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gmkbozsjm.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtialfdyc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gkqhdnmif.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gllcpaevz.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gpftncdjo.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gznbwcnqf.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gbpuzzznw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gjpctjoud.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gzfietndk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/grsdvxusp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsggmvcj.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gggggoiag.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gisozklez.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/guoedfwqs.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjeusrbn.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gkuhrnyek.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ghdlstype.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpfbqtkhf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmdpeblzk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/grqhwaulq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gejdcsywf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gmbtsrjlg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gctmftoet.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gzctwcuvm.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gdlhkqkrn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/grwdjurjd.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkeftkhqn.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/guezvofgx.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmrecdrvd.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gfsiljhsw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/glujeutcq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gcyenxsvk.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/grzvvblcn.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gwwljtmpu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gjmdahtzi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gknamngry.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/goqmwitfr.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gajybgepe.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gqmdlqhgf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gfqqardic.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gmgougosv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gzqdlwlkm.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gqgtokjtg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gibenezbu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gflbgdswp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gkeljgifs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gwkuoxhel.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gmrcwvagz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gwckmvuiz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gamltsgul.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfkvjpdg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gkhxjcegm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gldtogxwj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gaagimoxs.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gbizvkpum.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gslstkrtw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gygwmlemt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gxksurmvv.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gunalkakg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gdktuhhmc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghymjccck.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzubxgjpa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvcgkmjta.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gqdmdrzor.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/ggzygggbs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/ggiqgjqsh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gpjniqufu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghrzvhjzi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gkerwkmrw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gguuazutn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/ghdbdbdvn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gkrdxsmtk.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gzmpkqfyi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gsxmrjymj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxguwkkdm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/geukbaurg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gikfbuonk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gclomgrjm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/giriudcbe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gjtutpmaa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gmkeakzoe.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gkznauojl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/grjzebsnp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gkzdoybiz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gizfxwxqp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfubyphpy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjfrtaniy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gatxfefex.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gwyoghqxq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqltxnxqk.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/ggcrtbndv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/ggduacbdx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/ghlyhcbmn.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gvelduosg.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gfyoucflg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gladdwhat.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gggmalxjn.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gxbyuklue.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/glmiqbltc.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gwazkjgot.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gxaqlomyt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gxgixacvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gahulvfqw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gebekylpt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gxllgssvb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gskxnszfk.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gpcopqzry.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/godialudl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gkgwkemwr.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gmpuymeoi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/geszoejkk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/grrjqvmrf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gntomjgam.sHtML


<!-- 参考信息 -->