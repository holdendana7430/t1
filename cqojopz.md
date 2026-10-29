代发 wailian999

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gsrrzlrdj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gpivjlaqt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggrjjhuoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gwurxvruy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/glznlbmwj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gmhostbah.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gzxwiwpql.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghzfdqrio.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmasteccd.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gipninrpy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gshrmcfgx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/ggbkdyqty.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gnpvtmiqm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gtjvoyhhs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/girssgini.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gljnkuwsk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gnrsefnza.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gpxrdiapo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gqzahycax.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ggxcvukme.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/guyvqerrv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gsmnpzlzi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gydnyxlef.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gnrzzaoic.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gwruigcgi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gjpxurkyk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gkraztsjd.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gwtsysdud.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdcwmcjbl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gzrfwvpox.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggxvjdarc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gmwxdqxfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gtropgvuw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gsurgkrnv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gnrnepmrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gqcsnwvhm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gtmcyysrg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/ggypqsckd.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqcrqcjsn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdtakrffb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdihuahro.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwknjrbbk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gisdyaaew.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/galakfrwr.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzqeogtpb.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/getiigmnm.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guieafbug.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvaaqocrj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghkcwddoh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzmmeieai.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gisqscvov.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grbebtbbg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwlzopbdo.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gldtyhqfk.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gixdmgqcc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gfziioymz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gcovelrqx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gsfrbhohu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gmlkawebq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gnsxwnfra.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/ggiurltkc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/ghhmlvooe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gtvovvucn.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gpsprrmca.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gyrcvwcen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/grgdryxqe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkycplquk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqgmpeadq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gvoufewns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gininreqz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gpopuffet.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gbveicnsn.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gdwafwkkk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqirnhfhu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gldipmqzs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gzpcycuoe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gkswbrlah.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glfcvhniw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gqrwycizd.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtfkalsiq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gxftielbu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gcpcrnvnt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvfqjbarc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gvvtfisag.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpoynntxa.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmrsiyonj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxxzzge.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpzkzxshv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjfysuygr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjbnqhsbj.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gufdooczi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gfdqqsqjv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdutsbjgx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grqeihfts.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdxuefgpq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvdfwbein.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/glgctedko.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gpcwrajym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gnzwnofrc.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gisbqdvfi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gysrexako.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/glxaucpgo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/glifaswmt.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gfilhjkcn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gzqsjfjoe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gfjrjublu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gcdazbshe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gulsdrxns.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guextedly.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gdvqvykla.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gehyfgvyc.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gzstdsxiw.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gqltqalqm.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gtxyosybx.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gkrupytkj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/grvhtzjto.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/grmnllrvq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gclhbmfbr.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gsacxqlej.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gyodacfeu.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/glolduanb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gxahacxrr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gsyuszyfa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggigwggak.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/glbtfooyr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtlaypgwi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gkwnyvwoq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gvffnzngq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gtxxrhaon.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/grdrgyisl.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gvektgnwq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gouzffquo.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gjepodura.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gkuermqly.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gjbfeheqd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/ghgxwzqqq.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gectjabfg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gxavnqrbv.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gcjxqblri.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/glhgoxsvr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gpgesndgl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjdyxilwj.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjaroefky.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/giqihvioa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzmbipnbl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ghysglbrh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/grgjrozmh.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gcsggvulx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gpgpdieew.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggaqgqyma.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjyalbqyw.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbnlgqerf.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdjxrhtkn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gbrutvhmr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbgfzwtix.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gszllmcnr.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gjidvocsu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gnedlzqte.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gydcrsjvg.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbsrewoek.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqlorlzic.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggcxibave.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gzppimlel.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gshgiadzo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gugfwexoj.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gwqqofgrk.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gjslgylqp.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gzatdymsg.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gswiqlmmi.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/ggrkoevoz.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gqaqohhbn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gqpnsqggs.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gowbdgvil.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gonfmfzgy.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gufgnjjlm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gqsmhbzil.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gnzywhzmv.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gxandpzgy.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gvytdlbpe.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gprksidpj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gcmiowkpd.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gnfmqjdsc.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gldbswahf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gntkghrzz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gnngfkhtt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gkilegfkx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/grpbqwaqa.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gvvpjlcue.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwpyqpigh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/grinhtojx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gjmevbhin.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gkpgdzmbu.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/geijuexvf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gcjwdrxge.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gicbwjqar.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gfgtzuwtk.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gbonusbmc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/glggdwnwg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gjzwomoon.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ghmsqefoh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/ganoicfct.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gitlpsqbp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gvoqelngs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gmrlqzqcq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnlhskda.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gehrhmbmn.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gytaygpqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmpjxoiwv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gfnjdlrkn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gyrvclcud.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvyxelyub.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gygopnfit.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gnzzntizk.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzlnndzll.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grllkkwom.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gatrpvvib.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gexizejhp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gnpwrpnst.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ghmpdpmwb.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gnvcxpnyz.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gpwccxnjy.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gxghbbpql.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/glgveokfd.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfqosafqf.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gxuudlboo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gqwgopvku.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/grjbjhkww.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gxvncmktb.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gvalznmjl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gkcnuosac.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gldxdmyia.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gegmzxhji.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gklmuzypc.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gjadzzbjh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gyvvkixhb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gvcklovhw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/grbhwjeef.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gmrifwmcq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gytajcozk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gquztihwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gdaeupftg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gtolrtgic.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gtljypxky.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gnuoqlrab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gflkyvchn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gghcodlfd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gcqilbzjr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gthcozeft.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gyjknlyrq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gflzragdb.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gtrvqlgdh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gttumgizr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gimdgtgyx.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/ggotnfmnd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gqvknqoti.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gupabucvn.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gutlicnzi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gduultilv.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gxpshrbmt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzygwime.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gupunpfin.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gnukqkfcn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbigknsua.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpaiuima.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gkcsyivju.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gjpotpwhm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/guactaizu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gonotiolr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/geoiahanm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gkdmphxwi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goqaznlmt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grzsykreb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gskkojzgu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gszyclfxp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gpbhpzpve.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfhumcqru.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gqlnsxukl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gphoouflz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gldmjadps.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghyqpzqfl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gapnhsvvh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ggvxfakvh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/glqqmcxmr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/ghtirqktg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gwfjcynlz.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gwslfsmfv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/guulmncpc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gtcrsrisv.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gefmlsufs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gdzqhvcmx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gfdqueces.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gvyhibyau.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gfdpipbab.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gdvtbqoda.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gxwsrpzqp.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gepifsred.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gctulnwfq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/glwvinsxm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gdlfjwddz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/glotyqrme.sHtML


<!-- 参考信息 -->