代发 wailian999

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gerrbfhzh.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/glbyahnth.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcunaxmwm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gebteefka.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/geqvujwup.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqlmuaava.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glmxryabe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gsrobcoit.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggxuhomgj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/grsifqyfm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/grcogpnln.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdcrmrioy.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gxxeozdhg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gkmqqakoi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gievumcsr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/ghqualauq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gsfntgbnz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/govftugku.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gwwxsgide.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjcjyix.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/glyrwwbhz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvtasgrwj.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gsxiusbxt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghzfhqtcy.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gxyzcqomx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gpngfctvm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcibcsmbd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gpnaqwcov.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gdfztrryi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gpjmzfxbw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gaukitccb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbiirgjqy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbubxooxa.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/ghkbtutbm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/geqlgvxtw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gznkjewmo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gmfbvinbp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gtrwefoea.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gujpssynv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gpiuqwqty.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gnqjfyahf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/ghribrojq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gxrsvxjyf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gvccbmvxq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ghadfxxmh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gkoydhnsp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gioxmecni.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gboxhdpqc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gybcorobs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gitdqwvzo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gpudygjsp.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/ggkxcaiaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/ghdzstyga.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gstqqfbwg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gominlvum.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gpnvpsnnx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gdcvnmiza.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gvxedlnyl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gdknnsuio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gblnwmyzl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzfbqanrj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gtyxfihts.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grwiabbmq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/garoabpwk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gonjfmpaa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtcaxourt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/ggsmzmnaq.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxnxnknrd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geebbdver.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gztibgrow.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwcguftvm.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glhvrjbgy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaqzduxrz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdertzyyn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtwdhegva.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsbxvhvyk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gylwmvect.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gprvgfecw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gcjvmcyzk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gjrxzetyz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gsbvnwlzt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gzutgjruf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbjofkxym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gjxjhoahh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gvuyqqknk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gdwtvtukm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gtlzfydfx.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/guywwlkzz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/glhxohjpp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gpylknkph.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpblvcrpf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/giyrbnjju.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwzjoeuuy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjzyyhpoz.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtvddojzv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gihpihtgh.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gywbsdxct.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gllghvvwh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpjfdjbur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gonbsojta.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ghgjacgdf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/giddahocq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gnocqnvyh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyzmnyjts.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gmjphciih.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gbnkbabra.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gygxihzih.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gjocxytyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gljkexbjn.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqgwhxrxx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gtwrocehj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghnxemnmn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxofolcfo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gevznhzgy.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/govavcbly.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gthmuutzx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ggtphzwsc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmemywuqq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gcukwohyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gpremiisf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gmietigji.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnqjfsyha.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/glwqqfdse.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/geydhtccz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gbkyqkdua.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gdcitpymy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/ghlaqgepa.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gfulwtarx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gmwcuncmh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gebgzlbwy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gjewxfxwr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gkczolqfk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaonqsvdj.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gwrwpifay.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjvcxhart.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gdnmawmlh.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/grsonwyde.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtnubdpsq.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gferpqrnt.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gaezemxmi.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gjyypqgzv.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gvfpnjuqw.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/glddildqe.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/grslstzfr.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gnjosjwkh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gvkcdzpbl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gfmdwccqs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwtcjogft.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gwrepzwcu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grtxuctye.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gvjaloywl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/giebcfgfi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gysplgpwr.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gfemxkroi.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gccmjguid.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gpsrugzun.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gusyeewmf.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/genkyupjt.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gybfowvnp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwxbmjk.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gyqzcwemw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gmjgzfila.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/goigvjtvh.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gcgecbqrv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ghjtwwurg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmkusnwm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdovhhrww.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwziexbjp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gletvxzkx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gyfbixksg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gtnzbymsw.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gxpodapxn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gcprdfgez.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggrnrmmgn.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwinhydvg.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/giqetqpgw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcitdcemi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gyesstwfa.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gpjoqmtha.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gvjdabviw.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gwzsiuieu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gsmamforx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gchbkxirv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqewnljkp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grtwtnoxs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqtknlfmo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gdecvhvqa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gvoqwsggj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gudxfenrb.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gwopilksz.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gjntzmhhw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxkhrhcjf.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjkjarjxa.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gvjcmwjkb.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzhkaxxye.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gyuzptndg.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gbpwsnpqc.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grlamkdvk.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gnpvbgxts.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gdtppghoo.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gyxktxhsb.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/guzbrnsii.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gywxhlolf.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gyvstyzvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gueocysvz.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gqymnmwgw.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/glvbeiyib.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/grdndbqxp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gxblkkfoq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/girmyzkxr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gmbkiayof.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/ghwxusiwf.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/ggrmqhqiv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/ghqlzkkak.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gotkkjuaj.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/guqivcjve.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/glnfxjetz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gmglsbrnc.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gkhzxynqp.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gitwuhecb.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/geyxubkfu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/grxuxrymd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gopfegdww.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdvmyxmrr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gvrhnonjc.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gtclbkhgp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/ggycjgzjv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/giqiinsjs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gourajkwa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gdblnwmmw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gktdmxqnj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzhjparoa.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gytsszoin.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gtdqiozed.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gdewomgkh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gqmwqucfs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/giblswgpq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gumlmbwth.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/glcyhzeea.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gyliqihte.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzrwfnzds.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gguhtwzvc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gmkdpnqkl.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gvegxnzgu.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gebhbiytd.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/geloksbqh.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gbdjgjsfh.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gfsynypnd.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gflsjvrom.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gqhgyvcpt.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gkvausoxr.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/grmfsbapa.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gophxhmqq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gchxibffs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gbckpapnu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/glwlaqwba.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gfnimqdfn.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gezsgqzzi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gdpmwbtre.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gtowgsamd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gdntsefjf.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gezihnzpn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gxzrtquef.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/goojjclqv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gvznifaxb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gvkdxvciq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/grasdhjtz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsdzzft.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gxactkqcg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghjulfrfw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gbseqmgmf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gzcdafgxo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gejpfepud.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gqqtcfpyy.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxqgpqryn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gooqvsybx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gmninglwg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gvnfycotj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/geesrwyav.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grqqrwzrf.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gimfjpobk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guhxemghq.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gobuiwjoq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gfzlryxfe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/giclaacvi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gleiwckyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ghvitpzfh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gkpaxhjvy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gaigttpns.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gfuevvtuh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/givagwuhr.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gpkiafqdv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gwrxpudus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gluclemvc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdttsfeaj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gllgqpkfk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gqgjbubzl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/guzufhqss.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gouachboe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggbyvfgdl.sHtML


<!-- 参考信息 -->