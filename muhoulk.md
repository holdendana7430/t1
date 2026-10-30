代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gcrijqiiy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gabgzrbgv.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gqpjafkwu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gfilyjhoe.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gvoselosg.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gyzozqqmy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gtwklhdvd.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gfaarwrxe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gdbthuapt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsswnbspb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcfcitpfd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqqhcffhx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqyxaxjkv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gsgfirmlq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggzsoykjg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gntkkxpkn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gxkcpzdeh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gnqdzyvmx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gqkntpxeq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggeimwtfn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gwvkbccjs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gnfvzlrzc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gnqyvfmgx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gtilssaiz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqciqclfb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpxhjcxay.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gbjuhahvf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gppriagxf.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gbuwodudl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gsigjkker.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkussstue.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gvakheeea.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gqanotbfk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ggqyrrmqz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gvftzjxwo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/grsqgaxcp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/guyjtjssh.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/ghtbzlbbv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gfzssoqbi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gxsfuekom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtjwdhzan.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gzpheczli.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhvaaacu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/grenepsio.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gteqxlskn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gdrqfiovp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gqbamouew.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gblcqfpwl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmpmbqaqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gbywisfnp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdisncs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/ggldbztct.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/ghcfaqjub.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gebabvonk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/glcrcnjig.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gobtvhgzu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gpqlyfylh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/grnjomdku.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gcxvgfjkt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkohmtfud.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/ggrfwdwer.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gbkxwhetq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/ggsavedox.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gyngalbiz.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gtdsmzqjg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gertrtbuz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcrvhwdfl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvygziims.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyicnjlgu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gznmpxoad.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gqtsgzzwm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgdijftl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpoxgjyln.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gedrrqseb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzqzipamo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grimqfgoc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcbnrrbzy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grgsuetwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ghweuhqvr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggqxtwbvc.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpurdnagz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdeaecftj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/ghgraeaqv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gidgvljrz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gvmguiqby.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gxqtlrxio.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gvfsbtnjn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/godwcjnfq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gbfzfutku.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/geqruakcd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/grgfbslye.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxctjzccj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gxydyvflw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gnvjssqbg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsuyzzjzd.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gclsdjkta.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gpethinrw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjxudnlvt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gmwhwnana.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gccmcabmd.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/ggfqbqkwh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gorjwpsjp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gibiidlgj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gttqwxnjf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gqnzcltbd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gucubyksn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/grqopttbx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpwinxfyf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gukuajyhx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gwkgougfs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkufrtlrq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gizeiqadk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqentzzqh.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggebywcll.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gbpbuclxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gywsqdwbo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyeynpqkv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpucukdpi.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gzmckeoxz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gevqzuyhk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gqodnsndu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gengpxmao.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gehdaapmf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxeibbqxj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gzcwsxmfw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/getncorqk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gcmkvjjjf.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gwgkubwqk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gwqjmkmok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gqmbtsujl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gxyicblij.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/grvncvoyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/glnlrcvwi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gyklqslqo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gyrljzseu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gbtoctugb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guhrptdhx.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gqitoyfiz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gibqsrylq.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gvdatcdmc.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gmwkugcxs.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gyurydyli.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gzmqemnyo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/girprofbd.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnfnactbs.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gpxbmqpte.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gzdvymbdw.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glyidstcn.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gcormzglr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gtgpxpcrx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gbjlobdfo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gtpcvyqcm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gudfxikki.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gftzfrmrc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gvnzndvlz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/giantfkhw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmqrmnzyg.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gifwzdbyy.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gvpmvijnp.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/geqnyywec.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gzawpbqpx.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/grkvxolhl.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gkcrggvic.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gkxqctakn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gczonbmyb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gujtobfdz.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gixbjqcvg.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gxbuoqaoe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqxarvdgl.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbqfdfgan.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwlnauiga.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gynjvqsxh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gseegkqku.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gttpxnwlb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gtiphxbsq.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/guoijowub.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gdjotihqy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gpreulgpk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gksytdxzq.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gbqwcucll.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gkteotetj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gtkipgysu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gatlnkucl.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/ghjflonvu.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/glhnlmsiy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gnlrlyior.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfzzjfthc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gxmoojjvq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gcjkxuyub.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxxjhsudi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gyfyuxpfx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gepjjxtcz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gqhjsbjaz.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gbkmlrbrd.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gabeanvoy.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gwndnvyyg.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbepcaejy.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gneamhlvw.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gaztrxmxg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gtluzyytn.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gllallfft.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gaidhdeus.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gttbmmnop.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gxnableqv.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gghgrpejj.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gioyexvrw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gedyieyfd.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gimeogxpe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gsehnufrg.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gmquakezk.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gllrxzyfv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gstvchfvz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gpyztizrk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gufpolmao.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gqzcxpjgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/ggevwhlam.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/goepybhkd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gjulcrrip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gkifkipwa.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/grdusyryl.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gmllhzkzc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gdomqeykg.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gbcxjiwgy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gkxjdayno.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggdaivxlh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gmwseecan.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gyckrlekp.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gfpuolvkp.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gxhiursjo.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gjwvdeabz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gwroqsckq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaapfoxks.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gvjauaoef.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gcrfhlppl.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/galzqhiyg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gsjubvyky.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gfqverrwp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gwqmftdsh.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/ghohmedmz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gluidkagp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gqcjsmdtc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grdwoetuq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gufoayfzt.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpcfbwlqi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gtivhkdfe.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gmkrpmbla.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gmrxfhwoz.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/geluxcvuj.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gyxjhmgpo.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gtxphvbvz.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghcccarii.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gfqpepiwt.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvfhbybmp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/galxitrij.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gtbepculv.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gzqrvwnkj.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/goymviojw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/ghjhsiiqk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gcqexkgij.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gxxvhqets.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/goysmtzcm.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gzstsxzio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gpiyvwqjz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/guqalrooj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/grzwzsids.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gymsxxtsg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gmxmcolnw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwnyaaohs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gnffxwkox.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqjscpbvk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gohbedrrl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/giulnyrad.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gpusftjmu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtwlowhlv.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gztlihqfw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gqoenrwit.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcxkesu.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/golddbtev.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gnbwzmcdl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gfnkwnikk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gufdcoonj.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gwrayscka.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ghtpqwjdu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfbuscmxf.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gktehikdp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqoirqnnu.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gcmeiudpq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gvciwrfvj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gwgjqoumx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/geznkbkwf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ghbmxqxke.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/grgodnnoi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gzkqjfpaw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gcorpuydn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gekgkebjn.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gkcqdwouh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/glacqyfkx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkcwmitxr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/goxarptqy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtpihxhmo.sHtML


<!-- 参考信息 -->