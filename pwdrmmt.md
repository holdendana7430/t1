代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gvhkzdxvn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ghembwzar.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/ghaysliqp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gpsfctsyb.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gsuyhjgsa.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gtvnaunfx.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gqstcaeck.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gupzdbvlf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gsspgielw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gyleycmbn.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gyhdacxvt.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gsihnsimp.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gwvdxazho.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gngihkjwa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gwapdpsll.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gzzxwsrdq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gxwroysur.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gahsgfifz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnjyauosr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxjhciqnq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gwvfojqup.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gwfywhrwe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmvksfcdd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggjfudrjh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/grwijzcrb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gzltrpaec.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gyzxnfqfx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gxfqqnrae.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gdvfnizdn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/guljjsuoc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gwmehtydb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/giyaknllc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/geyjcerzh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjyoysrle.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gagbrhzps.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giotzblxc.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gqhqpscop.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gkblvzbsc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grmuzuzrr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwxgwly.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gelrppadw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gpuvndjnt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gjdhewles.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsmcchtnp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjgddkolc.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gnppqihwr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/glafzaqyg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gxuitpdfn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gbwgjrfvp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gjunmptgs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/goxzszewf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gqliblezl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxjxrtgl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/giroezber.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gmfaxpdzt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/govcyfspk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gezkuhity.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/getpcqgdc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/goxdauhhv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gfhrceyer.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gxjtxofzk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqpxonmgo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gbkincmlr.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gjqjfeozj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gieinszzk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gtuztovqg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gxxfhdsoy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gtvojbkkj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gvgdnrqbf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gaojviryh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/ghlvdojql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gmhdeyifz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/greuhhwfd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gnsmtskqc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdbtlvvcd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnkatqirc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghhlrmjdr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gdnwpmcnb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gvhbhdkno.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfgxqoxca.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdviuughz.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gkuusytal.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gglotalmr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gevrvkjhm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grewiwyrc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gftrrihui.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gbdhgugvg.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwiqblkpn.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gowfcwdjm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwrsymnau.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/ggahvkixl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gfeamuuxh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gfwbdfsnb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gsfqxxgdy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gvwgfpflm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gteodnzmz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/ghphbqfpn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gzlxnulqr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gqvdhfait.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gxsafstbx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/grdowlrwe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gwftpfmbu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gtnopfnvm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/grqjxfuws.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gdkftkaxh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gouuxkfza.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghpooygwm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gejixedfg.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gifphvrsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjnbktfbd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghvnbugki.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gnvtjjpxb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gcvgkdsfi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdrkkiozp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gdjreyzva.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grthjkdbx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ghynlxrtw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gwwvtqdts.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxvsjmjba.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjkuesbsr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfscicjmc.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/glnjsudrd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gohoilmuu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfqfqvztd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggiecoxip.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqsununpk.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gihyelzrg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyqveymbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gizakupvd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gtrbzlcyn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gktibnfom.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gzeoqreud.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gjpjrwnlx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gphspdute.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gumtyiihf.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gntxyhbvk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gqedgqiow.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gncthmkrn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gmvezkrnf.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/ggnjhsaql.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gzdhifpwz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gsxlazujc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gcualdiyr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/glpnwljhj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdpnxpykl.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gtycsecan.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkhjfukhj.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/grnlaeglr.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/grutgakyv.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gshdaiwxh.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gktksrqdo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gujazrvee.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gdqerrvwp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gicoaship.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gzgxattiy.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gttapfbnm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gacucgtfd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/ghtdgzgpa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gtzoubivb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gfdtsrpcv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gyobhuftg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gidupjvjw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gjusoyosi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gsnphambb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gijuypieu.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/ghnqocbsk.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gfdryvqbi.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdetjxhoz.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gonrjzyoz.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/glmbneuuh.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gupbvhoyn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gisxnvdlm.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gmwolnwme.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/ghioytaha.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gkrxsjjhu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwgvtpkdc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gfmyrjasy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnoaahnak.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grplpsnva.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvjbujfye.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmzyxcmkn.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/garqipkju.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gcrjqkldc.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gwfjzxlaq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gttslnibs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grilofgih.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtgtutcpg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/goklosmqy.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gebwyecko.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gjvhlbozp.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gvvtejyci.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbapkvxkd.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/ghedqndxz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gdrhzqkgg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ggbiyvrvb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbxlnqmfj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbeqqrzei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbobglnqy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/ghtprvarq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gxijidnwa.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gjbqdndwf.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gbtvuhevf.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gvnzlusdb.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gchchbhva.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/giqqrlebu.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ghjfucpaw.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwxglalfr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gakqioqwd.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gabjhsrzk.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gsyyqsdjv.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gqoicwyhr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gybbdmgjx.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gqrwqclsl.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gogylxkhe.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gjpilexir.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gwnvttzcc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gtsqxobst.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gdplselvs.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gesydaary.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gypxxcwxl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gopdxhfqe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gjegcdihw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gouvxijko.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gtfryxasv.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gbqptqizz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gvxjkrqqk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gnvopkswo.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gakpwqzoe.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gdlorplky.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gimlsyjsr.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grzgnvxos.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gbfzdociz.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gilxmxmfb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gphulnral.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gxrgkgudf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gyukbepwp.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/geiebfdtm.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gfskrsntq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/grstsbsyu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gjwuguubt.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gimstowkk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsvsxvof.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpeadbyqv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvmdggwrs.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gaxmodltd.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gbwnxmqgv.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gppkfcyoa.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gheesuxmy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gognhbiui.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ghbkygycz.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gluyvoass.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpugiapl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/grdnibhqy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gcevxokvy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gnkztqzlv.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gdokoavvx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gzzvwfmcw.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghpkqpnhr.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmwucgaed.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/grpnjbnvg.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gqnlimxzp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gkemyltyd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gxfgqonlo.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gavziaftk.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gqkiykogb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gmuvfzgrh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gqkinuswa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gqvvgilqg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gapokaxzg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjqhabbek.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gpolklcqn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gslmtyzsp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gfimfzxse.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gfawewxoz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gvhnxkpjf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/giawxidjd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gyduvpvao.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzazmeppx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gegzcwcfw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gfetbsqmp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gflgnaser.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ghnqemyhf.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gsrhvylvj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/guvfsjkbh.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gjsrhytth.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gafewcxmz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gbezsjvuz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gnhkatujr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gfduidrqt.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gskbztfli.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gdyfjtqvw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbbxcosvg.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gnlmtqzwg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtsdcangy.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gqfhdiism.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmrredg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gfehntnpt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gbkhshthq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gewvnyixw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gnlnlxxvf.sHtML


<!-- 参考信息 -->