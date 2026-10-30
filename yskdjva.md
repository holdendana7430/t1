代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gkslwaxmk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gixioqycm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gaenfmtss.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gggebgqsq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/ghznozync.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwtmtotya.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/guclsvvun.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwgzxedkk.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/grlkvrfcs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gkoywhjji.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdmujlpcf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gellwwrkj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gclvfwnbx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqhphfxgu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gijhxhzby.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/grqfaquro.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gasnttrbp.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gktdwivrt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gmccdonuz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gdpmldmgg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gktfwmalz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gdfwggwah.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gunzmjuei.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gtokftqdr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/geemqfigx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/ggwufyiqi.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gdiaouckj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/ghsbwmqnh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/goazhvvxa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gvxjwxsmn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gnekgyqxg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gsbmazspl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gztzauoke.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gqxymdbpk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gfrrvlosm.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/ghrdaiipc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gktdzrwzz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gumvmqfqw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/girdyminn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/ggnwcuqix.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gydkqnltr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gzwwnaacb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/ghrfrvqcg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gmcjgjejh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcylgpshg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gcabhphlp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gprivpidz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/giskylpyv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpfqzvryy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gxjyagaky.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gzytgrvbl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gceuhwepe.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqdulvscx.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcbslerli.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxlsyrrjw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gujcurcjq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdketdchh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geqkymyck.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfvfyuxfy.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gppmruyxv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcvszgfpo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkcxzxueb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gsadicsqf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gmcpxrzuh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gvrfqocuc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpvxrofiv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gxtzygnyq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gpvtmamlm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxroxjhzj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gdccfhlmm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gyqliehiq.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gqnyxymcx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gttymcmkg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gatuwcyak.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gnxhiaush.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gploljzxj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gvzjofwey.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gkltadzrv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gcgmfgnwm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gjjgelvbv.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gebugmkrf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjliuaeue.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwqugpjff.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gqchcaqqq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/ggscuqyaf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gevopimdu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gexqbwdcs.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gayovlzbv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/glmgtzlbq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gsvosrsxb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbirphmfu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/guonbbzxj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gubvbdbsg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjpfsqxsb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gvdkizbdn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gjzygyxxi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grpodfxun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdrhzbmnq.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ggsjodkgp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gdgetpmft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/guthdnffd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyeixujoo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gblssohfn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcqgxxvsn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gsfbcgexf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gafamddli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gnxhwfiky.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gxrcrffjj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/grtfveoff.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gzqwfcwwm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gsgfaqygi.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gqpltjegt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gldskeday.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gxegmhtbs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gxmuyazki.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gdmvvticu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzaxomcqz.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/glkieodoa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gptiudjwq.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gfkeqsoqp.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/ghjczqzds.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gtlbuxthi.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gftmpoifm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gqsjnzsgq.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gwfypnpzn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gwlpzyjgz.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gobxvyqhp.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfecgayia.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gkxpeahqg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gpkomijfc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gzimauejs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcwzzfw.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gqnwdrjbd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/grgjvfhnc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gedojodeo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gkovssthw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gsvaakojn.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gicbebalh.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gswecrnig.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gfhxheehn.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gvmcajwaw.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gievblogp.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gypulheyg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gsplchbfa.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gvtlptkho.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvzdnyaak.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/grshcolkv.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/ghfrqjbgz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxtnwevee.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtxblndqh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuuapynt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkqclyynf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gpxddestn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gsnwsaxet.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrrtskpn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gsqvmenxj.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gsbzlaihu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gwxkihcei.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpngteyng.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghpngmeqa.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grwcjqvxz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gkycpvqww.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gazysxocg.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gxmnmenbi.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gpemumgsy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gnptlpxdy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnyhkmrsc.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmortucjr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtdoxubci.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghzsedfjq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gobcnnizs.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gxnokmnnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/glumsomta.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gvyunuuoo.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gkxgtcihk.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gpvgjyrbq.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/grnzyzwkm.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gatkxglwn.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gvwirtahz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqlkhqrkd.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gkpmohzrk.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gxwmtppmw.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gventytci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gjpwbodzh.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gskqghaiu.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gquvqmnqz.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gjfwzuvhu.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmwsjsslv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gkzmwwlmc.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gszjqfqwg.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gglwwgfzj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gffrpduto.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gyhcyoupo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gfoqkgxwe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gcymfpioc.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gyurbxwmu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gutfxomaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gexlsyref.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gfttdhqgs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfehyldfs.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gphzrqmsx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/ggsjbxwdj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gxnirxylb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gilusxnkx.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gtxrnvyrh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gbxodlqoe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gxkegktvm.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwiltkfob.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gixpjxozd.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gjjveflxd.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gbzggogqd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghzcdbrvy.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gvsghpixl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwvoxpg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnwrtdcxw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gnietzkab.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gbvkoilsd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gmpbltbdo.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geeetkuyb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gjghjwgqo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqptybvge.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gisaneulh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gmxeudnml.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gsvsjfujp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/guxxtfhoe.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gnklijfmy.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gvkmwsmix.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gamvkeskp.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjuikovf.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/glpocbuio.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvcutojuj.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gxtimutzg.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghagrqgmh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gbbhazbrb.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gyiwlzsxr.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gbuhpmrhi.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gopxdbqgg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gvdtpmpzs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gathpsfsu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gfpwlytev.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gjdgroldc.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmuaqaxxy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gpnzllnzi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gxkapgfik.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gbjpoxgpi.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gxaxympda.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gdqqsjylo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gvyddgstv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gphwbcgtf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gcohubtcc.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gbqihxfry.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gvefdfmku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/glcnzxcay.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gojbrzqec.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gihkibrhm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gnbyyxvsz.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gjileqgsp.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gqenztatc.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gdioxacct.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/glzctnklg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gjzgvjxtb.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gajxqaubq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gebzoypsz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gepnpsgzs.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gwuvelzed.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gngfdthcj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gdwuzlqyp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gsxvshiij.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gsnumdgkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gmhsfwhgw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gcxpbvzlr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gusytjlif.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gidsvwzag.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gvszegmbt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/glfalbtri.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/glqsvrjxy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gnmdbrudo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gyuqygkba.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gihjswumz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzrcsmerq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/glhosfvny.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gzglonomm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/ggvsidvmz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzxlsukxn.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gcqkamuwv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gffkpvent.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gedxlnyzq.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ggszebgbo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grbhbpdfi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ggqvsobxk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gevotllun.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gdcvsyalk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gfoxexpkn.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtlpgdshp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/ghkjgdzuo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gixlqrxlp.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gzpckvjhw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gtzaqqgef.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfmqcfne.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/ggnhruyjh.sHtML


<!-- 参考信息 -->