代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/ghxajdnqq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gzxueqemr.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gfuzqyibl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/geqabdlgo.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gqfnunzmx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gicgfovoe.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/grjidajbg.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gicgisoud.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gpmjfdysf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gieoyrxra.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gzimhggkl.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gswxxcnya.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gdrhtcgiu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gffvdkigg.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gybcizmkw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gycqjgwit.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/ghpfoewho.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gpjiygppc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gtsbslcpy.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gjfkmgbhl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gfnxgmvbc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/guzwviilh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbbxxnjpw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/giejlamhj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzwhrbzvm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/geekvigbb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gantgzchw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gitzimvgb.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/glshvtrim.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/glcmgknkq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ggryxbwzg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gjxdccysf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grfkltely.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gnwcdwlfh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gxniyohtf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gveihxoad.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ggwdgsmpe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbqunnzzs.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/giexvkwny.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggvkycyrh.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gcfrwqedr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gvbuueyhm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzjyqdvuh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gabcevoty.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gjatazlqa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gjbdtkxni.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gupedddaj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gggnrxgev.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gaoygmmkd.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/giqaoeawt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gigqdyzsi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/glvbuhbuy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwudvrbjd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjsgulzrh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gcjtzjeoa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/glgncberm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gqtcsztsz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gbspuarnl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gkxkkivdc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gwiqptlex.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gvnqwoztp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gjsrsvymb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gkzkbrand.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsivyekcy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gotjevhxr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gpezrldbz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghdkhvopi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/glirgnggn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvrdigss.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gnjemszbw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gsfvhnahh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gmgbobivk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gvvbgkaxe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gugkzueaz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gvvpybkbz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gdmqhfpsd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/ghaazzlsq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/givdbgjst.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gerpvsjse.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsnsohevf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ganvjerun.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gcsotzfau.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gqabcypdn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gagtqbnbx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvnwosepb.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gttgouvvm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmhofxzhf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gaihcwjig.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glneywiwl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gegzauwui.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gamfmmfxp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/grbygyuox.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gowagnivv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvirvobwa.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gsbbpsxbl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gctrmyyfe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/grxhnktds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggeozkjhe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gbugfzout.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gykovbzki.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gkhrqynik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/grdlkdgao.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gksxnvjhc.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/ghxzpdbae.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gythvhmjw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/ggsessbpn.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/grlpkieua.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwhgyghbz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gbijpszpb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gcgxqmuwc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gaqcvkwtm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gqiklzxpb.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gcvrcvwth.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmtytrqbc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdfynaaip.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gfzdmbdbd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ggijwaazh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnmcnqila.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gtliqwfyk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gldetfghj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gihfgqydr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gkagghhnu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/govukmogl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gazubqjll.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gipaggwmm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsferduic.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gxuqdbuvd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gakzdkxde.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghkdbbipk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/guagtyjqy.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gksrfzgsq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmxttfyju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gqzfogxqz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbrtnfuad.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjajqxfhd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ghabxsrlf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/glphdacpb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ggxblkpgr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/ghplunddv.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gvnueyees.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gaanfvlca.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/glbvsbtde.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gyexexivj.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/ggxifnvdc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gzsndwvix.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gcwuyfcea.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gmrlxmwwt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/genwfbbqp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gveuilsqd.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gcgmrbgqm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjbuhnzrx.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gozolpnys.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gzbbvxflx.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gdoufrpyg.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gbpvnhjiq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gwqzmhjiw.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gcyhocdla.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gngvnxfbm.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjpkuxwdj.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/grizfvmgf.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gfhlcjcoh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/glcczlkvd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gnxoazstc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gxfojkllr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gpcdnvlgy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gzplwrfse.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/giuuuxcyp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gwtuqpwba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzdmiunvm.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gwmskelaf.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/ggmtbknsu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyrmsmzal.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gvqgabtzb.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gnrmivwhc.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/graimiwzb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gpsdqywup.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gjyeodupd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/ghcujixde.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gvregjydz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gycxtrpeo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/guliyoitz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gslzqygih.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkplikyuq.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gobykknzw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/grdihumvf.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gajfewjlw.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gxeeqfzlg.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gmqzawksg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/grjqmmsyk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gjlhpglvw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpvtkgxcn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwmrayohe.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbuewmyjp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/glyfahxka.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gfhcjmost.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gdctcnjay.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gmhvnqnku.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/glhzskyfl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwafruxmo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqznrujoh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grdomtgnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gixihttax.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/glswzbxzn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gpnprwmud.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gxwemaybf.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/goiunydat.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gepmgiwma.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gyzjrvvnp.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/guncjyalf.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gegwgotra.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gqdcspljd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gxjkplgfl.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gwuxeschp.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gvrhkffgg.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ghmdiejzn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gkqtxayvd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfrkbdvtm.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gieaedkuy.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gwittrykg.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gbxuegxlu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gkkiflduk.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gwndeavzv.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gzvxpsasg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gmkjlwzpn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gbefmqksi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/guxyoplso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gcquamsgj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gramfegic.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gywfshudd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gxfjvlmvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gbzoirnmp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/goftjrylo.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gpmqjhlqa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gtznbdmsb.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxaaikqrd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gqrfjufzg.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gogsdjphx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gjglqtjuw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gkqnvfypm.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbgcxummg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gpfxclhta.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gdeqtdwmz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gheqlfwno.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gwdaloquw.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gdcqwpzdu.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gmgfiareb.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmmpnrdkg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/glxozuclf.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gehathhgm.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gckvnlbyl.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/giipjxvor.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gjuoeeisn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gcublvlsm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvhzsseoc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geajqaouc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfytxtlux.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gtmsmdicr.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/genrynucq.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gwwxmvgyx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gkcvmvehi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gcjbmcsmz.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/grxopehba.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gnirpkxel.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gatiadrlp.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvbjhcpum.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/grmwrnjlk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gwewpmlag.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gbkxcivuy.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/ghmijgwep.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/grscqqtwf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gsybrujgn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gbbiqqqzx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/givswrbje.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gxadqkjwc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gvivxzlri.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gvmypenrl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gmoywivsf.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gacgwgqmx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gnzcbtpsh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwpftcjbq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gozgngepw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gfgroddte.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/ggenicaoj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gpojgmbyp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gmwjusmjw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gcuuvgeis.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gxpfcegmd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gjfnbpdgz.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gvduqqbxm.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gjcgquppa.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gqjvrxlgm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gzwkjbznq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/ggxizfxgs.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gpbeeyeyw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gubfoihta.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbihnjegm.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gbrrhgbhz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmeanexza.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gyepyqmli.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gggdkhdsf.sHtML


<!-- 参考信息 -->