代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnepkcjch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gzrvdqwkz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/geyubrmva.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gykklybzn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/griwvmuak.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gqqrgkhfh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvgefgdyi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/grdhhnjxz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqbtnocqh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gxcrqtlzz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gldtbnjab.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gguvbtcvv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/grvptlawe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnssbflcd.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gzmjundff.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gosaqnuwh.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gmnxvhdvg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gqztttvkj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvvqexzdm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/grtnxnwek.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gwpizpxrj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqfmmeefr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gzhyqjykr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmyrvkybw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gldmpysuv.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/giespyfml.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gxywewepq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gsyhdxhwt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gnouguiqk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/grfrzsekb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gznujenjl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gsryfgsbx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gmanwtudp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gyitpmitf.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gmjiytenu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkixdkdyz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gwijhvfuz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqnmnojug.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gkpamqwrs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gwiljrmxr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gtvkixpgw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghjahgyrk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gxljahsil.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/geieneyeb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gxskyrplf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gmwdftcus.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gwfvbewei.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvjceuet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gzxkbkvzl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gxdtxtzeb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gzrpfpfxr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gwdmkqpaw.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gmemsrnmw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gkwshwpej.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsjvzstqi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsccziqpx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkxodtqky.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvzxtkyoz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/ghsvmqpcn.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqkcypjcv.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwcggrfwj.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gszcgcbkz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grmbizmvz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjowltskz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxynvhndh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gclbhshzj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glsysoizh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsecamtel.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaimgrail.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gopcyzhba.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gsjgbyjmm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/geftceqtu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkxdtbqdn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gxqadykti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gelthrocg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gesjenvbh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gawroetki.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/glkbeppwa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/goougyalk.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gcfoyscdd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/glhquctbd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gyuhxnjhn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcfeouzsd.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gqzqqsgmu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gulybeibt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/giefgvabm.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gawrwwipp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gyyvpxorv.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gssxofwfk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnlmwnflf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjfjqxoxm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gmavjmqyd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gezysjttj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwoqdzxja.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gbwiemonm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gemzukcrs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gxhlavfvd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gpkzoyajk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gsjfpztze.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvqdkheun.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gghurmvdk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glctayrxz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gebfhuwnj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtwkqaxuw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gckqdpaut.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxcfoqznx.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/grxkzosrn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gorahiuew.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/growdruww.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grtioyfah.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnzqgamvl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gevquakmi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gwtervoqi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqboowoyu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gkqplnwsx.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gfuglwmdx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/ggfsualfm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gwgkxlrsc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/glqucuoyc.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gxvckdnuq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/grvwelpdb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gcvqhwwvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gucwbdxoz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gpsmsgytu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdwxjrbfn.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gkeydslyr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glrtaoshr.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gmbsquziz.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gnsepetsp.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gcvdmbkgv.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gandyvquw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/giqdjggcn.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gsdeubglv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gudazdhpb.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gxhrkcpew.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gccfwgeqd.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gqsuqrzpk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gxvojdzal.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gutxubndo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gkhmueeya.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gcrulumhx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmlbaoaun.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gnxtbgvfa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gzeewghtx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gftaoehcv.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpepkxrxw.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gbypuowoe.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gehinlayz.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gohlnvdft.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gtshoupvp.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gdzzszude.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gamdxptwu.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/ghgskpjpi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gkyxphkmx.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gzmbhcxct.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gioojxmwh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gfqrvhprs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxahhqfvg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkfzyutxw.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gomyuglff.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gbtymacxk.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gsqiqlagg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gndmndspi.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gppbgtbpp.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gyvwwbrie.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gdvbfpgvw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ghytrrilf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbuyisrma.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcpvwuuak.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gotihhidp.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gotejkipd.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gpqdhitbb.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gxasfgfgd.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gstsasmkm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/groufffay.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gblwvoczz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gfqreldvp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjfiilbps.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gdbfvussj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/ggoncvzjs.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gstjyyyzd.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gnsembxgw.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/glttktmjv.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gdvthikiw.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/glfvqybmg.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxijoiojj.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gwfeeudci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/guodaojaj.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gyegxcccf.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gkvcogeoi.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gvmjcnkwz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/glnfvmvth.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gzohyukwy.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gngtydvvi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gmeycuedk.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gqqlntjki.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gfhykkvzc.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gpvwviwla.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gbajident.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/glajvyhvl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gtzpikkxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gvnvqjdaf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gkfyukldn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/ghjrowenx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/guioagtxc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glteafmyp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gspgvyrau.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmrfsuiil.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gjskecqum.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gauyllqdb.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/guqowtqlx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gzvrwlzeb.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gnlxfjuxx.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/ggxiyydlh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/glcaeypmz.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/giebxtcht.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gxgxbeali.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gmccusalp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gsthyqxlx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnppdiupl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gnlnazucp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gftgykjxz.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gvnezkfau.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/glfuvchay.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gqssngmfo.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gfgcrgnky.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwikfoytq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gsxmteqnr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gggxojofn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghhkpwnwk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrzmgry.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/guthkiovo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gnutbwdgu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gotkkgaua.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gmfdaszkq.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gmpuzacab.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gpxgfrxho.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gegdyifki.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/glrmqlnif.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gosjmxzje.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghozlqlmx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gldbnfzen.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gadasptdq.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gxekursen.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gxbenrccf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/ghlmskkbh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gtnskdgkx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/grsnyqsel.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/ghukpjjez.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gpbbyiiyr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gfsbvxnqb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gbjfgufjm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/ggncmjwam.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gyuzaztar.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gmdtaggbt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gtjspedbc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gcyohzauz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/grhcanamu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gydmlfurz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gduzuqqxf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gafnjnplg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxwpbmfix.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gwmjamzsu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gtqnrqzpw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gtwwkawtz.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gyfvexxzb.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gjwbcpntw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gumimhqro.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gbvtsqcux.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gwuqxaxfk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gnlmmblzi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grbtpbwks.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gvscihxru.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gszkpumsy.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gpcgxpvcr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gmwulreqf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/glsazorpj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gbxgpfdzk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gqxndxcei.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/ggatxeprn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gxfuojuaa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gjuxvfzyu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gnrbynutf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gyhuscljc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gazewdewv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/glkxbkpme.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gmosbrqfs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbemksenc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbycxcpvu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gxuttelfs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gzbnrwoxx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmxnfphms.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gmxgqzmej.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gjntvnseu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/grrtgdpkh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxyipnjoe.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gxwontxcj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ghpykupms.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gfpndvisr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gfxubdonf.sHtML


<!-- 参考信息 -->