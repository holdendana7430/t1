代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gvjkpggnf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gofqhksxu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gegpoalwi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkrijxirt.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gejeeovzo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gfujplwjn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gcyynvcuc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfetwfnnj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gmbcgralr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gsgspxvtq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gqusjlblb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gkpdedisp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gdabeysux.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdglcexvs.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gxoxjfozc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdakslcpg.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gkvmpxrrj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gxffchzek.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/guxmucxxn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gmeitsvwu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvvnalywq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/giudyrhhd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/glmfnictp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glczuzxll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqbmwfgfw.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gtvhnngxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/goprxpxsb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gkhhkosdu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gpmednkge.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gtzvzjfyy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gutigplyu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gpnmuwmds.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/grzlwyhjr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gnyipebyb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gfpobewcg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gcxrkzash.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gfwjszwsu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/geslcbrfo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gmtajhdvd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghdslgubz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/glnaeoawj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/ggclvajbv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gtvspbcau.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gwxpmdlii.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/goqxckzsq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gzyumkpim.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gxznygyac.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gyzamozgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gwqjbzebq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gvkaycjbh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gieralhqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/ggshaywtz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gmuzcsgka.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbzodigq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guvbdqdmd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtdisffku.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbyrdqdfz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtclbksio.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/goxuzkkah.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjoyfuknl.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/goyflgwyw.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gygooksqt.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/genycowcg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gaxjwwwyk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqxvwdhvg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdzmzuhob.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gshpysakd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggfkgatlf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwywlaglb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvhnljhwm.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gkgycrsvf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gtvtwttmd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gpsrlwmvr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gqmnqlnlh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gzrdnrzab.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gjdrivtaq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/goosqorfg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gkrjipsay.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gdozfiyrr.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gjhelmlbz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqbtyfrh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gkzkmbuif.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gkjhakfcl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmzascihd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/glfvkhxrc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gczcrhvif.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gzjsfjxyl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/ghkqcuclo.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gubctkpfy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/glaacsrmu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzgaldguv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gkzpfwwnd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gylgnyybd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gidscigxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gtjplsdgj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsqrgljah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gwspqhmld.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gviyzohun.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geasvshyo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gwlhyoypp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwmzrreeo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnenvgkbf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gcspypeba.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gefqxmoov.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghprzfsqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtvagucjy.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gsdvsqcbv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goyhcfpwl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gtuiaogzd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/geagctkes.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gfiikcqki.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/grtwxzyhe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/ghywugucc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gadxgecay.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gnbcgpopx.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gahncnrsg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gdizudcev.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gozceovfl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gvjlsqhbq.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gaqaahyku.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gpdbbdhrm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gvglevcwt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gpbeeomlq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gyrxluhjl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggjhoktjp.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gicnzwleu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwlnrswlm.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gxjppitli.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/grquitpjf.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/grgkdpfet.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqmmoqqxu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/ggdiofgcq.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gccidgdll.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/geanmtpne.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gtiqzbgbz.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gflzsdqro.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gjokcomlp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gsnmiycug.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gkzlxypiy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfiowslmb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwsfglbiu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gotxrtqie.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gggtjjvgv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gojzjzeoo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcqxhrofr.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gyczaiqte.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gwbvqhplo.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gzquiidbg.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/goomfwopa.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gempvejfv.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gneokhwsd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gmhlbgdbz.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gzielvrhl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gylptfnse.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gkqmaoxlq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gnzptriif.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfeqzwwub.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glqeeaszk.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gxvjfvops.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaaurytku.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gtpicwraq.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gtetptpxj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/giiyeeqqj.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gieuxnjah.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gauzwrnnr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfxonbwpb.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gazmghade.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ghvmoepjz.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpxwzdomo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gpspvtpzq.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/grhsgdrvb.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/grhctilck.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gxtwxhwgy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gfjxzyfjs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gelaumxrl.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/geqcyyybu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfvpvbwln.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggoaalsay.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gbkwpokzo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gqklemzow.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gskbzkmda.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gsyuwyvsh.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gaqndvdyj.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gxhzyuddw.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnxltxuha.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gnmmdqgvh.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gdoeijuvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/guniaiuvf.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gwqcmnxrv.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gqdanjugy.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gokhmwbio.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/grbgnmokk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdecaezk.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/glaooaqco.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gifwpalan.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gcruygwmg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/goorsbuqp.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gshweexfr.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gydcenaqc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gmtsybnav.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gqoabcton.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/grwbqbtyd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gqdbdumod.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gfbcywens.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gekhrxvcx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gyzjipetx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gjzdwulud.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/guapslxbf.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gonzzugjl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glsyoufpv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghekeothb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gmvffzznk.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/guugonlqn.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gtqekberh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gdfmwwohr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gunawjwgo.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gjqubucnp.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gaaviobst.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gliaunvos.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtphrtchl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpvrcsujx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gkcxrrhjf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gxkhagodu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gaunvonii.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gmcjjntmo.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/guzgbmvpf.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gzumroakj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gjztqcdlb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsiwbqsyx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjyuzzjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbtxdrpbg.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gbgmhnpye.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjkgtizre.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gzsavpmpt.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gaoipiswv.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gqrahswry.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gecoehmcp.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzikcgxna.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnsrremsd.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gddgwfxmq.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gbcbvkqzf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gwbqsxxwa.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gfstqjtte.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/ghiogpmvh.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ggtjvopxm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gudxuotdc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gfifcpwhy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gvhnuzlxu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gduyarqkr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gtkmbmttg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gyyaagcwl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gkmybxlwe.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gfusodsdx.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gfisbaxqw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gupwjdxgz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtamdposo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gooqqvcpg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtirbnxxw.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gazbegmrb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gkipilqix.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gvxnrjsgc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gehyssjkp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gagumamvv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/ghughgolg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gynpuqfbg.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gptprrxhd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmnynvjjo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gpppryyol.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/glaxrphok.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gaszsqzha.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gwlldksxp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gepsmtxsz.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gfpfbthwv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gldtgvefk.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gtrddypwz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gnihohvve.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gbmjzrwet.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvdrgnvhl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjidmfxb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gbnomepsg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gljlffxvy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ggsdeaiov.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gzkizejgn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gcfymwdcc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gqfpzextv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gucrzmjdn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gzmtmakfl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gnayjrjza.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqclsumhg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gscnkuqvj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gzexpjlex.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbqtmvurt.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gdbwuoxoh.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/ghyxfasll.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gwlepmmck.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gzvnkyhjn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwsqngzqp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gokwrirrq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/ghilrrtux.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gvxvbcykp.sHtML


<!-- 参考信息 -->