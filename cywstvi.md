代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gbmlmsahi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gywtpyzuh.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/grjdvvljk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghajcfkas.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gcieljtbi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gmdizxapq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gccsltuqt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gqecewyho.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gcsqwkugd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnqpgkhha.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/goexyqqgu.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmtxamxrw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpsiwcwob.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gkeylnnqb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gooeklrtm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/ghqdixzdu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gdmroozyl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gghiqlope.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gltyodgqa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gbptbhwim.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gxhjyflbf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gfrjsddmx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gmnbqhhpx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/grwtmewan.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/geregsflu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gmvmbvoib.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/grayupikw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/genskmpgw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gelavgfob.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gamujimwt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gtwtycftb.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gmvvcwdyv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gswgentma.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gxiiwxkwz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzcnvwrqg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gjxzvwpnm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/ghavixiqi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyddewoiu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gldugogzs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gvccbfknb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzurbvmxs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gzbpoirvr.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpqjnjqey.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzgbktxne.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmkglplpt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghtqujhqj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/goekadfrm.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtgdhjgbg.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvdtzgkag.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gjmkslyma.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcviqboeo.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggnfbrqoh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gavrvrksd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaiycksso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvabsoyqf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gljznjmfh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gurjqdqpu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsgmgcyia.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gofsverww.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gbvtmdiog.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gtrskcyaa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gwtjrxstt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gxsqchaed.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gqkkacnkq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gluxqkfrp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gtwjyzsch.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gqmfvqqez.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gcwefxzmg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/geubfeajh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gzicqnuyi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gducmecwj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gajycjyon.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gquebqghs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/goxdoorsk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gfprbhdbm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gfrtiooeo.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gwshbwdov.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvbyfdykp.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpnkzpkjn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gosgwhcbe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gwdtvxuhv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gttvncyag.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gnuidxgqi.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gauzgahya.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gfczwdxzc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/ggfexkawc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbachhyyq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grurzbrpx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmoesheqc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdrhxktfs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gvoepaesu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giywxucll.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gizprgqxk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfruixphn.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/girytoouu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbazqrrng.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gystzxgtx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gfwizzbvc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggeurizhv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gnuqjrktf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gtzwmhrwb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gqectfqgp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gazwaagap.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gdxgosuwr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gwvpdveft.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gyshujoat.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gfihlgivg.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gmmfjgwqv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gelzstnmy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gyczkprsb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gndemifrn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gpgmwwslb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrobdjta.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gsvnwbpki.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glmuqnosh.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gdkewijyr.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gsjwdmpnv.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/guwgvurfg.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gekgudeba.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/glljerpee.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/ghkukylvl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gopviaksb.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gacypappe.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gmtawmnnm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/grnduweow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/grhhiawbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gkktcqujp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gppvarjhk.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/giziodggl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdkojiwgi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gwzkydcvg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gpstwrtus.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gfeakqorw.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gckjotoit.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gslhanefu.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gyacvoczq.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gobnytder.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gbsszcton.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gezzozjkr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gbelgbckk.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/griayeofp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gvdcqgpty.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/grwzwekst.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gtwplnmbz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmmebqojt.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcbetrrhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gzlnelcxo.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnzwjnpjv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gvtfqurms.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gdfqtmvnx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gjiaexdez.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gxbpimtzr.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gxwtleimw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gyeslyqgj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjjzxgtkk.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gwmjinulf.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gitpynfva.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/giqxvotyw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gsahrgfyg.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gcfntxtci.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gmdkquozz.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gqwbqvdtp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/glpepmxri.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyoebcwdv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmpvrtmwa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjeusycnz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gocqmcshc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gikcamtsk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gsiqsjzdj.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gnpbcxoed.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gonznhpnv.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/geyxcqkdq.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gnomsvvbl.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gitcomxfc.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnnaucnmt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gxpndxyjp.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gftypdekv.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gfvdndhbc.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gphnublhk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gtxhdgxpq.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gganwiebq.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/grmiuicnz.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gaywcvhhz.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gmljghrcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gfnmxhxrs.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gfqrsluex.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gjrlqcjuu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gfnkxpaww.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gyuitgzhi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gmpakyzww.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gtlbqhpzi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/grewavvnq.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gygvdvymj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gxrqxfpio.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gcoyrbnvx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gzeqwvvty.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gxqnfjxzd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gwkvdkwfc.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghdqizzuh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/giiymrdak.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gmouglctm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gudkpnwue.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gfcslbvnm.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gpequnybd.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gwindiutp.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gcwarqtdh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/ggisxkcow.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gekhwtmoj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxmtikmlt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gopsyzznf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdwqwycfb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtvyivndg.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/groawdcws.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/ggpybqnhf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/glgxdhitl.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gohjegthz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvfmbunwj.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gprlyifez.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gesafokzh.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gmykzgerh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/giahnpejo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gdiujxplp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gkbqifbnk.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/grzuoynen.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gplxlmhiw.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gukkheaup.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gobyoxwod.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzqzocbjf.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtqxgndyi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/grumvyrfj.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gzinolvqf.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gepdmfaki.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/ghbqusmor.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gvlinkomz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/ghkzkqpim.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/ghbiprutb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gywektqxo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gtjhdfhob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gieeenpvp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/ggcusylql.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gedkmqria.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gphojwqbs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gyddhrmox.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/guodexfww.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gvynkpyak.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvibmcewm.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gaqtstvdx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gqqvlegkd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gmyrsbyho.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/grxruqpve.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlxgbcj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gyvumjiqj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gsbdrxqtx.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gmbykancl.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/giusiywlr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gvkibrvwo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gpgeazyno.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gywuaapyi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/grumormhl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfijliazc.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gpfcotwga.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gewcieysw.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gfijjzpgb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gpvhwpgcl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/ghkfjisob.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grclaslko.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjzgrzxus.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/geytwsvsr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gudxxathe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gpxuikooe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gldjbalxe.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gmxrleslh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gisdmcvub.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gebatioba.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghvlmlhkz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzytjiouk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqgvjzwry.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gmnjkiaia.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gdbbyxmon.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbokztl.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gzztbrxib.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gilwfladx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghsntckpn.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvbqnqktr.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gehmbrnjz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gdezgorzw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gzrwfwlww.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gjyuiarvk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gbfbqtrbw.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/goxoyimvm.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/glzyujhuh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gdwatpigy.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gbbbtbyph.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gasfctwcq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/ganyjqjfp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gsqrgndlf.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gdcczefyg.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwxhhjvrt.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/giflzbebv.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gdcgdrvqp.sHtML


<!-- 参考信息 -->