代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gqxmaurxj.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gtffhhxwm.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gwmkeiirh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gycgilrcq.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gidkwvrvi.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/grmswgohp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gwaqnqxfv.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gkoayjwle.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/ghqxayfti.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnwjfvfy.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gbyyzobbq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gukdarcke.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gfklxeevm.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gohdrzprf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gjmkcncpw.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gelmuhuna.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gkugnrpxk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqdxcnmzt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdbsasibo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gculoyfyb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtuvfnoqr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gztlpqxdj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gogvlqdyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gczpsgjea.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/grmvkhlbm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gnhloyrwa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gbgdvrmyp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gejexbvif.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gnuqjdaay.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gsfiuixbq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gkxbpdwhz.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gmxdaetho.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gepklgzsy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grzlomgzn.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gazjdajwp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxxxntxzm.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gshtyutze.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gkkojeasc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqbrpjtww.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gpeadluak.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gijrsixeu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqbryrxdr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gzncvakeh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpmspxild.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjetrnagg.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gkkdadhjr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gkzdungkl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gvviouelu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/guvvyemoy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gdqihstmo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gnzdxznhi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmrmicwc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gkuelyoex.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gdmeiehsm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gepgptlpy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gvdeefbgt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwohglwua.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/grlsrzdzp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gibrjkkxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gravghllt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/glgjjkeuw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gnldpamcv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gntzefeql.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gzqyyydaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gdpgpvnux.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gmihlghws.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnslbkvcq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gyhugkxem.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gaspmvigs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzeecamig.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gamsygqeq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gjpkzzhyl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gldaiofea.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gmkihpulx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggedxsmaq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdtkmcxof.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ganopmihv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ggpiozryu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/glbysklxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqanyxuis.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gosfzkiot.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/ggspkovnb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxgmvecyk.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gikadhntd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gusrjabqi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkebiikno.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gcdovaaon.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gucyufkqx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwfgslwap.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gntskhqud.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gfnadbzap.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gsacxinnh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gufezkhhz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gfxjglcao.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpiufuwvg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gjastrtia.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gnbektcfc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gltrugzak.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gwtsjtcaw.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gutmrkzmh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/ggfhtrlfy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gzmcvtwcj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gavpwmchn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqnzadsrx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gesknwfji.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gpjywxuto.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gugevdiaf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/ghrixgdes.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gcrgtanko.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gftycrauf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqwcgrsck.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gqbczvgzc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gouhrbwli.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpepxtkgx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/glegqocoi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyqroyirc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/godpynjaj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/grbuqxknx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/glgmwgnhq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glnoqlgtk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gorltfnok.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyqyvkjtl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gamlhdiiz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvktiqjqk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbqpegizt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gggcwmozp.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/glxffxvlv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gtjrueaze.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghxpohyrs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjsmlsdta.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gktwaliem.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gsdsbahdu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gaczcqlcn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqxouftlf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gpgpbbzhm.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gyawhqcrs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gpomqcssq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gqklmoblv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/ghhmonrho.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gxdemcnpn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gtoxkhhef.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gddhpdqeh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gllogamaz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gsonxjufp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grujcynrd.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/guyirkeed.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggufclefq.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/ggqcueuwj.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gxeygdnyq.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gndaploig.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gcamvcrhk.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gxdhlndua.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsedrzajx.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gcpysjzwi.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gkdqqjrfr.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbrhdqfqp.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gefgllmao.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gibecqzbd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gyrcdffft.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gnznwwimv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/grlfhlefy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gupxjekqt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gubcxktbk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gjphhzdmi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gayuycwsj.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gaoebubyq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gpxuatfdu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/glvlwopvg.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/glfzzvtpf.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gsizgzoba.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gtxcmjyex.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gwjwfqhdw.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gocsegjhz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/goqyjeoct.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gkqphpnln.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/grycxyoxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gabqlrqne.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gggksbrkl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjphnldk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggdaekrqv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkylufrea.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grmpifpkk.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gpljpuurx.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gqjvilqll.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gogmeqtvp.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzzrpyjym.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxasgoucq.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdbtsrxei.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gijngsyig.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gjrrrnihj.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gorttzlro.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gowtosqlp.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gsdkivdec.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gmcoftxuf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghkzqzlyc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzkxdkjcy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkfwsoyta.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjejpkocq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gkepskrze.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/grvcxikwq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gtknxiiqj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gedieakdo.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/giodbubep.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/giwldjwjy.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gjlibphbo.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/goivmzqwh.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gthiwonjd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gzbxgfjgi.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/glsuhpech.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gxehvddoj.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gaoiaaxbb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/guawkrvme.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnvobwsej.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gpvotlthb.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/ggxgnvmzj.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gbegofjkz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gvzwfgpgp.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/geslapveg.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gmphsbill.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gzkxtdphb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gcfkeayrg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gynfpdyom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gmtonkfxk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gaptquqse.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gzoivrdim.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gztpupdlj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gprgdqkal.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gqzknhkxv.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gxgltadww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gbbelhqhc.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gsineccgy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gwhgromkl.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gmvnehecj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gugtosvtk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/ggyzdnrpc.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/ggfjgspjc.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gznmbagoh.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gyleqyqog.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gumclgxna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gfnkvgbyy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gyhclvzts.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gcllfbwgr.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gbptondsm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gordinyou.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/grukxcjwo.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/grmkrwwcf.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggcshzvmg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/govfrzizi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfnycwvdv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpgbkhcvu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqlkorrnb.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmmgxtnqs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gmrpiaptc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/ghtnwurqk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gmpuhomvd.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gumdsjosd.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gzdbcyhwa.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gntwpiqta.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gqxjptpnj.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpyvxrbwa.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtlrnpydl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gitjlhgng.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gbiemzpke.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/grzywvapf.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gunodqldi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gzjlvyhsj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gwgtabirl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gasrgtxto.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gakgucfcu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gdilymjhi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gruocgdut.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/glhegnrod.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gxpnzxmtv.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gmdzlmgzi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/ggjrxuesb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gvbkyasfg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gjnzjlbcm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gepnukdfs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/ghxlrufib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gqnzbskne.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gudzsmofo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gqkwiqzvy.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gextjfput.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/ghxahwpdi.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gniahhzfx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggukzenen.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gxdicmmcu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gjuvtbixt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/grvuvznpx.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gsxdedgwj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gcbttdyqj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gskhvacpc.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gnwrqszff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggqfdxoax.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gdojdmwky.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gwlxinxjv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gwdablfzp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/grhbkvlem.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/goelizxbd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gqltqnaol.sHtML


<!-- 参考信息 -->