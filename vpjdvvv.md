代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gilzmnvny.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtrxbezti.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/ggbadfanl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grwbwhiwc.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/ghvermohb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gkykgatsg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbsgsmsfr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gciklbmjq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gqzksznjj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gsjliacdr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gzaztxfih.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnreaeplp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gthxcpsmv.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gjxgbswep.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gdrhdliog.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gfolcaqes.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gxvinhdpl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gcefmobac.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gmzpwfhgb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gywfsezav.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gxqmirkmw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/ghkvxgskf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gtloyhtqi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/ghzpdzbcz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/geyautjax.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqruygajz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gcsowkhef.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/ghbklhlvm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gmbksomey.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gocjqgqmb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ghdifjfqj.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/glalikgay.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gweavknep.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gqhlzzgei.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggclekirj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gojszesev.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/ggdhrvozs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gyumcdnlr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gqjydrmns.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gvdljsluv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gfrasorgw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gnyfdjerx.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggvrdnwmy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grckitero.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmakohxvk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gjvnjafll.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gtrhhynae.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcwgejvnv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkbtkmicy.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gmcqntrpt.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gppkstdwa.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gprlylmbr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdlaufmgb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gehvfsivf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gotgsyojj.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmrjartzn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdvlfazie.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsplwlyfv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gqftfauet.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gitlhhnbx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/givboblhl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gwjovcvtk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/goxxstgmt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gtpuoesvf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gkrwksjyw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gnpqffaio.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gkhyzcndm.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gjnhehrgl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gbygkjhnk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gpxiqudlw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghjylfxyt.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gtokuczvk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gwfgytayq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gvfrecbvt.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gzcgnmkoz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gnhvjskwc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gicflsmvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grdxrelue.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxamwwhew.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gyznpzpny.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gydontnsj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggjntidaj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gzprnfbvq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnizmlgcz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gsubxjgnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gonrazljr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grkpretwe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gycgjepeg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gesafdkfy.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbjjlpsol.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gvfiowrub.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gheyhcazq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gojtpngkq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfrxpfnjc.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gslwpongi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmdyimnzn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gyrcsbhkw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gavvotmzt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ghefignac.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gzwvbbzqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gscrfbmrq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsgsbhyzf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gfsjtpaqa.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gpbhzbgwu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/ggrcpnppx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gxnterstc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gvhgqqcmf.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gemhnpbfh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/giijweqvl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gtcdjcvyl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gnmxamppf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/grakjbctr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guooaxyfs.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gvittgeim.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxxntorda.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gnddusroz.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ggrscmazb.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gxriwukuq.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmklwkfjf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gcgqakykd.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gzxrhoami.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gxsyvgrew.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gsgcbvgwn.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/ggboqxbvo.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gjhxpitfe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gbrprnjik.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gqgwsoedx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gbqelluvc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gzegpeahx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gpirxtdyx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gfiihjkxc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gmfuymlbc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/ghpmfrqmg.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gzpfzhmml.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gwcyknnvz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/guojlybwb.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gehzjrdou.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gcixfzhps.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gobcwxhvg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gffhnfugb.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gqxgcgplk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzafekaht.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gezcxtivd.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gfsdntwmi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gttimwcfh.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzslhlqsq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gkvxlmrzp.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghclqzmre.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwdnaioyd.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gzctrakvz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfexceovx.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gtscqiqts.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gdyrrupqq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glkpslynk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/glvvmkxgn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gllqrgsrc.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grdvofbtd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gpyvcnokb.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gmqsxfvoh.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/glkwyoqbp.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gvowrwqci.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gahgjrhwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcgqgtyym.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjofmclik.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghaghmqbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gitolqlib.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/grpcutmcw.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gxawhrgmn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gcbyxgedz.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gcdzibsid.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/griazafhh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzcijtz.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gcelrpvxz.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gxyzclkxm.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gwzzxajjg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gvukcxzjj.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gzvhpcges.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gkulluapv.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/geyybpidt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gyjwsuigk.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gnbwqzugm.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/ggrqhmtzg.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gvfbqwiqy.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gzjoboofa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gaexqcbtk.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gusbbsqnr.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/geekkphls.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/goxzteodj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/grlufzibg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gypkmbstz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gxfhquuiw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gvaflijzd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gkzvzxdnj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gbzespyom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gbqngcalk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gmfhscsww.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gibwnmnni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/ggnbkjlye.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gekyqarpz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/ghpdbfljm.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gsqolfjcy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ghiwvhtjm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/grdjhaghc.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gsqopgrxq.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gwukqutqi.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gtrrjonrz.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/geljwaugm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gdyiuuxcw.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gjryjwfni.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/ghgwakizl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gxfaqouhi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gskywgqhm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gxgqqvqow.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gcpomgfkj.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/ggjqkzqom.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/giisuzeum.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfibggrw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/glehbylzg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/genpksbkj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gsaaocyfn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gkuygkhpd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gwvklrdgt.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqcooagea.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/ggdscmodx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gncdigazm.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpcgzodtz.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghzmmlhpe.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gfiavizee.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gyitpjbtx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gwmalxzqq.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gakmwjovp.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gljngyaik.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gqmnlqgfx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gwcjgusrl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/giapklump.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gebzlmckk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gwhihisjt.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/ghaceqfrb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gnlxofvzq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gvakkqaak.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gnxmrkjjp.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gyibwdrot.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gxlcqtxch.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/glectdocx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gqiljeqct.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gmlxvgxrx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gfqdrzrvr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gdbvhdbwt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gtymxnrhb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/giryaarie.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/grkhsxvpx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gclnwrirh.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gddxopbcv.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gpjjgqkfl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gfcuxtamg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/ggfyerujq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gzdnrwhnz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gumjizanw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gpsuuhfsn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gahstrhws.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gcdtjnwym.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfldjeyue.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gqyemtxuy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/ghatqsrtm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzamhngat.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gwkqfbqsk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gvzflagab.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmofywfst.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/glimxgvry.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gjodaffot.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gujwaxkhb.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gpbdjobha.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gcuphsrbu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkvfizwxx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxhopkiza.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggacpsgee.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gojcubofx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gnrhssksz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/guuxadrju.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggnpzdhrm.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gbznvgogs.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gwzynbazq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gaiofpjfa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gchgdhxgv.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gajrwmamm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gwxtnhzgf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gebytrzml.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gfwacuaqx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbkyjhfxg.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/guqvyxrzr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gitntdlzh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/ggkdxuzia.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gwvzugzjl.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gberdpwgt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gdoncwhnu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gizlrozvy.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gfukhmfhj.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gxcyrdhwt.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gfysfsghh.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gmmqqtxqd.sHtML


<!-- 参考信息 -->