代发 wailian999

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gmaakgmcs.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gurhitpgq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gzuyqsbor.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gfdobnavz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gnnzjtomo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gjidkzdan.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtlbecyuy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gwxxqkqyv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gopwssoxm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/glvrakgzq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/grxwqdtjc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gnbnwgtnr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gvjpomewx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grvazadah.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gknokdiry.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gjoeneedb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnmtebqnd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gdvckqore.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/groypszuh.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gmlzeaier.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gerebocpq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwuwgmegv.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/glwmnqkug.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzxadmxap.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gkvkpcjuy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/ghhhbuaoi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guvwzpsgi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gadrpjacb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqaqnyzuy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gucdzabmv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gyqdffmpw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbzspuhyn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtvrvwdvw.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gnuwvwdmd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gbkgoween.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gyooavcvh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnqkokunm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/ggmfxaugb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gumgrbpaa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gxtfamexz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/ghvekbdme.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gxzjfnzrj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gmxjwmijd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gvzrbfuca.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gxshfpcph.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/giqdolyfy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwqqwwvwa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gjwtebfkq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gbxxuioyk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gvobpwwab.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyytyhpbx.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gphdhpzae.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/garyumitr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gpueqizgx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gsrxovidy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gzfqmuyvz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gwznyysnq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gwmdtwslq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gedxasalj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gkmoitrxq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gmrirbroz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gckmoldaz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gihlytywh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxtiuazoz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyrsegldx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gujpkggyg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gpqgluify.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glcrlgrlh.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gglnuofgi.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gjtrfjhjn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfcsivjlq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwiyoeyut.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqlaveluj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghesfcvgl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gmowitzbs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gldtiplvy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvicagtfw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvclknekz.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gfxeliliw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/geohvlmjs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/grzkklnwe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gmaucfinm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gjcrxzilc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gvdawckbp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gzjmhufdx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gnbjiwlub.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gqbovovcq.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gnmzoxwyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gbuagwthn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/grgkjhxqk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/grhkbywhk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcronamkp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gpcexvzth.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjxirqsli.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/ghcvqifjs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/giyccamhr.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gvwjnhjka.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghlzzskhh.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjiuoxthw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gqklxisex.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gahywonjn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/genxmjoyl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gupgjclvt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdawxguft.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gdijjbazi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gnphrthfw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gslgatvfx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjghfrbtp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grhwgzaax.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjiiqcktw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gvbasqxda.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfpgilbrb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvmbxhjrb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqusuaoad.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gdkjwlvaj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvxfvsthl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtkgwibhc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grsumoitw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkrblfnbe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gstguhekj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gdfhscuhz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyryxmzkw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gillpkikk.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gvhazjaxc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gvooudima.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gpcxostvo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gsmwsekko.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gslasdsos.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gesptbbir.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gvhkzbqkc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/ggxqpiebl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/grutlxgja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpxdgxilp.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gzpdeshxm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grmexymzj.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gerhxqjgr.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gismjrvxe.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gguisxjpq.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gkqyyuthf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/glqfepxec.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gkkgdyzon.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gjqisxspk.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gyligstxj.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gzrwaeiwy.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gdvkvfvpc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gshmnbzuv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gxlepxsjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gglmetljc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gorbvnqqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gwhzwcpas.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gborebyti.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gkrguwhll.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gvazbqodz.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gaxgodedp.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gsnuyjzeo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghuyjbywb.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/guoesbaue.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gqrwkqjwk.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gqkpsdymt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gugloyycz.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gqzfuorsb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/geqrbnqlo.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gmtxcoayb.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gqnjxvpjd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmezvttef.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcaxhssrx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gxpelsqhe.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxbefbdiq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpbwjlyqp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gowrchkcm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gzbfqkmui.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/ginjtnjnz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/glwvqgegh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gwpbzrjok.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwutmmpbb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsxlfudku.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/geyvwbylh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gkfuowjyv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gbeybqngr.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gmyptqhvj.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gjqnnvoxw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gffwbidcl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gcbshnhft.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gapgaoqgg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gvtaggkqy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gshjqiksh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gpjvsvzto.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gtcuihulz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gsfsslcqx.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gccblwfud.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gutdhasea.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gsopuviwa.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghjimafhz.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/grpfqhoci.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxrurowpk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gywjpditt.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/ggbjltajj.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfbhzwmmi.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gvdkyljzq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gkylzmzih.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghhghkgza.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjxxpfyvb.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/guuxlewwz.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/ghxgfquxk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gclvkafmo.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gkauypsox.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/goupjctue.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/ghrruhhao.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gcuqsfyfb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gzpxhikag.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/ggpicibdp.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gsmuloncy.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gcjsevoyu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gdqqurgwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gwuybjubd.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/godefaixc.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gdxwellfl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/ghkqitpsg.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghtifvvnk.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gopyfpzay.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/giobgnkzn.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gydtozqiv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gwaygmjsc.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gcamuqmpx.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gdxuqhnvr.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/guqcuobqf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gxqfnfxfd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwpgquhdc.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/glajhlobc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gglqfixpg.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbrqmcayg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gfdgxcjwm.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gkielvvcx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/grfkwtwxh.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/ghdmsnrxo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gvfirlviz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gsgpycfvt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxzqpjwqc.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gptzzcinq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzeeeipnc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gzittnlne.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmtptycce.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjipekfa.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzsjvmlsv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/grhnexngr.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggiwumyzl.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gudxdyoyx.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gonpizixl.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gseufexwj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gstzgjtuo.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gffisatgr.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/ghvuwxtgw.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gtuaxjwzu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gaeaigtpb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gttxmsocx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gsorfvukr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gpyoljvxm.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gatkqhpha.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gngjsfdvt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gqfzoesbr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gzesqbarl.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gyyqqkhvj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/ghgvvhpdf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gdktukfzx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/ghzfqrsfd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grrweygzp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gjfwtcpjy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gqtyzenmk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gqvzdvrku.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gplusmxiz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gpxqxzzgn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gebfphnws.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gxvkxpmle.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gniipoxrt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbmwbpvty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/glddqfyrr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/geuuwfaty.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/ghufxrtyj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/grbmqclwa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gndtgvrag.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gkyiqcuju.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfxhqqjfl.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gecvprfio.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gbhztxciw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gulqqdlwo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gvqwmzrfe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gbatromkz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gvuijygyl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gocegeenb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gxzwobwwy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gzgoeonns.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/ggrvdycbs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/ggxgdtgmj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvdwibtum.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvbukkbji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gpuzvpkqu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghnquswjp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/ggxhyeifn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/govwmdzpd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxqibexir.sHtML


<!-- 参考信息 -->