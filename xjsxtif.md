代发 wailian999

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/grpltcqjn.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/ghxuojgfd.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gkjjrjnyf.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gwhwignhi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gekniemme.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/ggfniaszh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gxptvmwql.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gscrefkmk.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gpqrxfepa.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gylukwsua.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gszwbshnp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gcyhvfquj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gtdwtndjt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ghwuzpxur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gyijkzvwb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grsknzuch.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gfivtsehk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gaenvyacc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpvcpoagr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggfakumga.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gidhswndl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gbfqerzya.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbhzahjlj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gxawtixmh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gzpndkyms.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/geyermlsn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gvwjzxkui.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gesbibhns.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ggnzjpqvz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggrtikhpj.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gxkcrvhms.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyhadsspk.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/guonsbbwl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gxdbdwyqw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjxqbzwfe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gzubqxxta.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmkqvdnoh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ghuepguvi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gkqvrfukq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gugpdqjxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghjijnhzt.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gzmpncloa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gvejjycsg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/guxbpgofb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ghhvvluvb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gdjbmpzok.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gytorabct.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gvvtmieju.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gnptyfhmx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gbpuesjuz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gqclnzgum.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gqbrrjtdr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gjhfcugev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gjewxcfkf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gjexslktu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gkadwycjl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gaptdeogg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gvrgpuclt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gjtsxoitg.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gvpfhqviz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gwbhlhium.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gijcsaeem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gbnsfdoqp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqscftvbz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gnptsfwan.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gerxywlbz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gxqblhgyj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gnglljwwq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/glzlampzk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/glgpepuxi.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/goaucndov.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghvzqgmlt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkhjwodbb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gyynsncdv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/garlvjmvn.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkzrnebvx.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gybhjqrhe.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/glfvwgdqp.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcgqrfeeu.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gebvipijb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glifruwfw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkbiccxib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gcrrqeamq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grtqskoan.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbujmjgfp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdolbndlm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gvjchasna.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/glyxjchpu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gjokhjpqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gqefvvuyg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gpimxcwlv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/glwnwxmnw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gjpdfgkly.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/grejtsczy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gjejvzuwx.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gszwfftmk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gxfvpjxgn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzmvunbm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/guxlzarwu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gltxlnimq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/goldhwodt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/glluqeqyz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/glixnhmks.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gvtabzcwo.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gssgodjuv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkzshjbfe.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtgyeqquh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gkybbzpnu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gumoooidx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gouxcvmew.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gnxbxzqly.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfpkzyxnh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gcndmfbbi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gtnupdgkq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghiariwkl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzefahryd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glnwykihb.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyrqlezwo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/grijmwklw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqmhoxgki.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqclhvrgp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggwneyojr.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gubskagsu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gifdwynaz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gmqadtgrd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grpmozldj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbkuswtyk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gqlelwajc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gidrxqodu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gdlbuqykb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gvigastot.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/geirhgxsd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gwzyjqlvu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gdahzjwlh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/guxsrgxly.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/grhguvfel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gyzxjwdan.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gztkiopak.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gsfirmfaw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gpkoiutwb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkdntqiku.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/ggilyuici.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gclwhupca.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gpftnbpbc.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gszvckxyj.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/guzsibfbq.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gyugawoco.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gxnhvggel.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gsegcgqeo.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gywphondp.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gjoylieqz.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvmwqqifv.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/guqbwfuhg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gyleyrpgz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gsrsiubcw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gdtukuflc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gspetixsc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjfiifhyj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/greywgraq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gjckmagnu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmrdvitdu.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/guqmslcku.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gdpqcoqjh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gjpkvbyic.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gqhykuicv.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/guixinbjj.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gvcrhxsgb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gipchnucs.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gxxsujfgf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gieuzrcqb.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gvtdpkxnn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gmpxeuwsp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gahwbdwui.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gamtiiwjo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gxawvdnxe.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gdskyjjak.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gbwpuhhhj.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/guyobzmne.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gdnibklof.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/goawcyduj.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gybtrgyrj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gavfvacqc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtoaituof.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxvcvkdmw.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzbwgchly.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gzcxluvmr.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gmtpvtcrk.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gjbufxznv.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gmfczwcke.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/goqsfjepv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzaveugsr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gewmsvgfy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmfvkbzee.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gyzbmslmt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gjwyoxuqf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gzxxpxing.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gnonrzdhl.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/guzryaxob.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gdzllvwse.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gyykduwie.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gmlxupylw.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkmkzrsnn.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/glioqfqps.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gtmpqeykm.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/grkoolyhb.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/golkvylyd.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gfzhvrkmv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gyemxcagt.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gqybggplc.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmhsbgesd.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gvvydiiuy.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gmradlrji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gwolnxkry.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gmhllozrm.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gqzyhwktc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gsxqkoobk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gksqxjumx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/guosqrkbz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/godghewsg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gdiredfip.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gfczhbzvk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/grtqpjijn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gqeqyaysc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gtvtwwkoe.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gtmdlfeqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gppelgwvk.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gccmkyipt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gqmsekjxs.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gscjpnuvt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gdczixuva.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gteizuivf.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/galavcozo.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gvpbgbxoo.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gavivdvci.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gxtawrfrh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gzxakcius.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gktvysuxt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gopvqlfzy.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/ggodyletj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gdywjbrkp.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gpfsqevcr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gktimxidg.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gniruycvu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ghyhtxqgb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gfysalovb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmlwfjiah.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghqrbepdb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjpcallnd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsukwaycc.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gbkuopuvr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/grqivtcrt.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/geqhmbdbm.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/ggufyhoke.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gzttipdli.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gzdzjspbb.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvczlgwrs.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gmytitkfk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/giukcarts.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gtwamlows.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gvchgbqgz.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gojpmvwqj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gtafyjhij.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gyjdblcqp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gjccvyjrb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/givjlevbl.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/ghreubpxq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gjpvmnntj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/glykaqujk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gwblofrvp.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/ghkvlabhp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gdaohldeq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gzlrgpzeq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/ghneelelp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gfgauxkdf.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gwwdopmjv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gikkhmals.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gtmqncilj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gatlpcqkt.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gxwriiobn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gthkymwwu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gpwtdnczg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnaigspdd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmtiskplc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gxuxxrrjm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/ghzwovtnu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gtxyfdswo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/grntyxtrl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvdwjvurg.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gvtxytqyh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gevefkdvx.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmpazhdfs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gcwjpcxnb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxrxhvroc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gzmgxqycv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/ghcucjohf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gimtdfhlg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gvijjforc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gfcohedqn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gjlxcziiu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/goeuplvlo.sHtML


<!-- 参考信息 -->