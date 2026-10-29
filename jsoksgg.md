代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gbeupcxgv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/ggmjtvlzo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/geofxytlp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqkqhmzin.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gsctcsedo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gatkhvmrq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gvvrwlnfd.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gpqgoitdz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gzpppsvzp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfrghthja.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/grjrqtpin.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gchifwvlo.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/ggzneshsc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gvyxclmyb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gylpgdelm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/glzernaaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gdazovukj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gihohluam.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gazayzeon.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghphmmydh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gytmfapku.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjfquzakz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gyziwmoap.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gquukhqly.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/glbewreek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ghlendcin.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/glflmiuql.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gqqsylajj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gdixieocm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gzhcbykpm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gzvhagdql.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gbqciacio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gegqguczv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gstajgcbf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gljhlyhia.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gounrkgkz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gnywdfcie.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gyvzfirsd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gqjjdieib.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gcbjabdxn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnaarpqzx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gkaaswxpa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjuiyynep.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gzzglnkpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/grzuewhsd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gcogewgqq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/glcyirpgf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gippmqdto.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gzzdpbrkz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gzswemejn.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwkwpxxvm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnbrmbbos.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxodubiqd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/guvevkqmt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gliyitpfw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpmakxmrw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gttzikqcc.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/godtlezbd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gymbjderu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcdicunsk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gidxfpndw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzaavaqtt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvntzvoxi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdzfgjzbv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grngualoc.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsmihfsly.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gcswtqdbj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/guqsufkqm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gnoomnzin.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gsbbaugfr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpckhcp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gohqaqcgs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gcdqrlgfi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/ggckkedhu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/glsaoxktl.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gmpegudvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gteiqxkdg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/guvzzarog.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gvovwmiah.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gofhfgyca.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ghsmyrbmk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gsqefgdcw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gwkwuhejh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gjtwgmcig.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gsiiozcoh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyuuwbipp.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwdtnrzmi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gpmlmuumc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gepmeugtu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwelbkrjj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gmwwuteqk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfnyaqnae.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gcyxbbnkp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gmdysvqew.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnbpyrhmr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcpmwkosf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsjvqttcj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjijkcmgx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gajkwrwmj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gecguznft.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvsdlfawa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfqdsmhae.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gzlyhbnnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfubswtvu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gkihnvccp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gseyvemfi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzoogsmzq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvjxiealq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gldvidxql.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/girtzeryi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/ggtdrmqpt.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gpmlhirax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/glfpdvurd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/guhclcgrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gqwobvrob.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ggizttuog.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gxzzyinne.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/glpwmepkb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbgcqhdph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gukegkezb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyzwslgyw.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gntxfnejy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzdxlofrv.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/ggaryafaq.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/glmafqphz.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/grvymneaa.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gptqsftew.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gwlyfzrdq.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsdamjrch.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gkylyiruf.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gocxhumxz.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gqpvdxomv.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gyfrphwjc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gzlfoggtc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/ggiwotwpn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzsoqczzm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gzorbvwpt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqdljjsbo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gdklxeeug.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gpbbrsoil.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/guskvnvdd.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gyfqzqzih.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gpoeovzmm.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gqwjnpemr.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ggbdglfif.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gqkawxauz.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gjlrsybkk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/geihpffpj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gnkdkdrvx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gipxltoet.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gyqhbgtnm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gguroulmw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbrnfdmff.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzqvrdxth.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnddkyqru.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gvtgnmddl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/goqcpvdlt.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gapmtwwii.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/goxurwcps.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/ghtfalhiy.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/glfvsdnth.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glxkgobgl.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/glsefpnpg.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/goruiqkdv.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gytnyqbjc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gbeayynmq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gnhtlwnso.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gzhploukc.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gaqhgepuz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gfynxjukt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggoodasqs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyvetirwl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gssjkgqfl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcsehgyj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gmwqkpnaq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/grucnktnq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gbwihcbbz.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gwydyhvhd.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gmmxyaqtf.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gnqyqugql.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gtebfefgf.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gowfkaqxu.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlfdrlw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gcyvojric.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gftgbcswx.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gcktwbjtu.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gyiirltyz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/grqsdmnsg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gevfdexmz.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gicvdlerb.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gfgxjripy.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/guxlnswkc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gaavzmnem.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/geuhlwdfd.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/grsrdeykp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gdijmyqam.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gipjwgjng.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gfhouelgk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gajlcncih.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gruuhwqja.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkmztzauq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gqwqelaro.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gcbiejsaq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gediyrklb.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gtartagsy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gcbmsecke.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gotuwgzhk.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gftjuaute.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gkvbaoyxr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gidcpossx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gzeqkoshd.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdapzexzq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gdqwbessx.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gygkxiwok.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gojinpeac.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqlwnqhvu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gmjvukwmy.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gancdanbr.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvlrpyhvz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzweydndd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gasstelaw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/glikadkkl.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gxlimikxt.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gxdweyxnj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gifrytrlz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtngomfmw.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gwdstqzss.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gqnhzczza.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gwqmoptsc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gomglhlth.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gtfhhiqkh.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gshhbwrxf.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gmzhdisuv.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gszmulgrx.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwpxuupwl.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmdalwcok.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gigdcnxig.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/ggvxmrrci.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gjufvisbw.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/grrkhatdu.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/ggpzkxdcq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/geyeffdbw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gmakvfytk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gzalidixk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/groqvlojf.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/ghkdzrwzg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gqyjfgxie.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gwjakpmdu.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/ghcniltht.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gzdwzzmme.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gnjayojsz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gygcayirg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gyicqwbqg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpogshddn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gomlvmqhe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gsnnehemf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gdcqwulub.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gohmguqmb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gjgifljzy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/ghsxylxqk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/ggrixczvm.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gscsbyedn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gznovpopz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gmxplukux.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gkoyioret.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gggpnkcfg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gjgdytwjp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geujvhhrv.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gijxjqrzk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbjqrtwzf.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmtcoqqfn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gmxncvppu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gzxpozssv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gygslhvmq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/glsxefzga.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gpujbcckj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/giadzfbhe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gampkmetb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gfihokrxs.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gugrqxskb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gnfozzikt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyccytido.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdsnyeuvy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpnnrbwsl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gnxscccle.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gcdrpvgzs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gafzhntfs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gehgzauus.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gyilfxuff.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gxlswhhmm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gurynhbdx.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gxjfyvhaf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxtwifk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdnkowmrv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gogqfrlfe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gxwqhlqzq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkgienvfr.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gbaujwtim.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gneferpsm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gximkvsuu.sHtML


<!-- 参考信息 -->