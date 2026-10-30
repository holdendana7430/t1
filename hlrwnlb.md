代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gslblezdo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnqyjhxxx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gcxvyafys.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gpxvpqazb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gkgzavdnt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/guvupcuwm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/grytyqjve.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gnxvaajmz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gzkssxfnf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gufwxytlw.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gxqgfgdna.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdlbyxmec.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gyggdtukd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gctwjugus.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gaqycxrtt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gujgmnaal.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcuqebkds.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtxlucnyp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gtvzlqtrd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gebjqsybd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsuspeohu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/grcadhcom.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gezhzxnog.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gptbkyqwy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gntbqehnj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gmrsfosan.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gdudpenzq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/giarkqlax.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gnjikywwm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gqdtbftiw.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gpdlsbcvd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gjcorqxvi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gnwmwcqnr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gjzoofnjb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfycyebhu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gbdtcomwi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gffssxyhi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gkqqirfvq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gfvsjvcti.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gaitjzdyg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gmtbfuubk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gluwttwlr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gllpivnvh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjhzydrlg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gysxnrjbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gqggeixeg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gsmclmxop.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gufungpxx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gzbyzsveo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gtilrvvlo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gapcraefq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbhhynojc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaxzbfqgr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glblabohj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gemrltfce.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gikjtiies.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gadrzlqmm.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gmfczxsoc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyuuqomcq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gogbxtsyi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcdybsuhh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geqnvvuhs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwxttcpio.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goalfyyoh.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gezbtkpfu.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gcvgwqwto.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gddqijmms.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gntwhpigz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gnulyrynf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gvldmkzqd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gjbwpqfik.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gvupaemmu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gsajdjivx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gvramqrsk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gobjztnqs.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gueotfmfj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gmxymjbao.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmumhaocw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzfydlyvm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gxrciahxo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gekkiyrzj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gxfwsjdlp.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gtgwomafk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gterunpww.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gdxcjcnwe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtdptdeot.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtrhgetwm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gwdgqtyph.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gywheapac.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmsjfwemt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gsjcdzfcu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gylelkklr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gqefpadgx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/grrsiqyfq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqfqfedtx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtsqomqmw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbatagibb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyfnyuyee.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gxmlutkar.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkjkacbyi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gibqgkiad.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gknemfjdj.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/goyjowhzb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gsdpssret.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbbgyclcg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvwvzksvc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grjnkooec.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gpufhtqpa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gnviazozw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gaxkkrnus.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gnmxfunuh.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gbtqaddea.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gsiudstae.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gryaxerds.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gnucmdyxk.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/ghnbvozry.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gxunenbwq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/ggxgqxzni.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/glugohtfo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gpopjzhso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glegyhhjt.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gosmydqsq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggwgexviy.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gicltjzzi.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gzrohepsw.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyvlpuiiv.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbirxhkju.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gkqdbxnwv.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gngeochgm.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/guywvdvar.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gcmgmxbdl.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpipahuao.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gqvjazyln.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gqkapbttl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjonrvpup.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gpaiqxjff.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gakdxiqgw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/girhobkyu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/goaqphscw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/giuowwuag.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/govoweuvg.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gefvbgsuu.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gztelimhc.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/grnzqnygq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/geqdltujo.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/ganpoilas.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gqfurtkps.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gwyzuqwqf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gkcuwmckl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/ggktzvsta.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gxjkmncvu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gkbyhpift.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzcnknjdn.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzhsxwljv.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gsefhffjb.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gakxwicnh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmxxvpspn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gskgckjwp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gfmhzlweb.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/guabonmyk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gdgcyvwfi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghjaunvhp.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gywxugcca.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmbuixeaj.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghmfhbruw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gcjvhfnjg.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gufgtmtqm.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gbmiilqwa.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gsevcrfju.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gmkzxgdoc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gawbkpiia.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvsqoppaz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/glaxalqaz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbznvntiw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gvzqhfawm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gnwdfzpfl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gnramexvc.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/giwfhwwum.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gaaiswdch.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gpyeqshkq.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gusvcpvvu.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gfoaqpcyw.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/ggdgwndbn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gxkvcdavt.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gwtdjhwqd.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gljxqiaxz.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gyfqldsht.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gnqcctpfc.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtpqedqaz.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmhcwdtni.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gmqvcitgi.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gzaoavhtl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gunehkfap.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gjgbkqsyv.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gufrahbhw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gfwtnjire.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gjgkptjil.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/guodtwmlo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/giyceeqnx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gpmnsxfar.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/glgejgbxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gluirknqc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/geribuoty.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gafqrcjqg.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/ggbonqyls.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gluwosjsi.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gynbmbacs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gidobxrii.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggjiqrcxj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/geqzagzfi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gthxtannq.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gbrzescbi.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gmaozdyls.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gabxttunq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gzmcctacq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gefwwbmlz.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gsiqzaqko.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/glhwumwzu.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glglardca.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gjreapttl.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gfgigxxwj.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gpvqbqedv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghhizyayg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqunrtchs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/giurbftgl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghbzxiuhd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gyaqlvjca.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gphxocpbd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gucpjlieo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gitqhgqld.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzkqtyho.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gyconzlmi.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gqpnclkrr.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gmvisauqi.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtqfgyrms.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbpnxurrf.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gnopqwqvu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/grznefviy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/ghzwpgnti.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gcyfrierm.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gvmbiypis.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gdpesrsfv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gzyuqxqxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/ghvccaavk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gxbscucmj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gmlirsgrh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghjrggszw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gccgrrzqb.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gfiylxgdi.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/grsrlwgjd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/glpnkriwj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gwrblwmyo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gozjcmepq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gdnxcnlnr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gjmopudom.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gikxcopon.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gfkvvtywb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gjhkqbqjf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gbovsmiqx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gkgeikmey.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/glzkjdzhb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gysrmsgnz.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gzgljxbdy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/ghdvvmnch.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/giaohtfty.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/ghshdague.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gmtcwcamj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glqxvtxpm.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gjxcuuzkd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geqmpxmgd.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gejzwaiyz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gljvspjxr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpmdrccsj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/geppuugus.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gthokjkoc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gzrbnxboy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwrgmhf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/ggcvldqeg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gmeybhdnx.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gfxzbcarm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/ggnxkzmiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gewcnsswz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gagsgkhav.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glwqjctij.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/glqnqugbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gucwtuups.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gytvqxmcq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/geerjvzmk.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gdedbzota.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/ghelfuidr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/geslgblwb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdzghctzn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/givdrndhw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gzbdybcis.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gmpuzddku.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gyzfhgxwm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfbbboiiu.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gjpwujufo.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gccjfuxke.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gznlyzzja.sHtML


<!-- 参考信息 -->