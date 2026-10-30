代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/glrilkebx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gfhspphxx.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gykccxnhz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnipbrkpe.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gpfwusgvj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gtmsrhsod.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gkiysnqmb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gkcjbburc.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/guqlvyipn.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/ggpvweslp.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gydchvadt.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/guunlrido.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/grbvdtzme.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gsjcmrlqz.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gufssdrmj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gtewvlscm.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gpmtaojym.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gmxzvumdx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghfkvudoz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gewcxuqtk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/graohwujg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/glpysgiha.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gmkuyoklx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwkkmiqej.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gemgmdaal.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gpuzamjuy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gyitsqgfp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxkzecweb.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/geiahrjyn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/giexaguqn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/ghulbaioj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gcdixkafl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gagguauxi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gphqrbaai.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gtjfodnrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdugulzhc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gypnvkjqr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwlafwivw.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/ghjxjwafj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gycfpiqno.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gtharuqem.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gaaurowdd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpjfgaxlq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gpasxggvn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gnvwvvker.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfcfolaqv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gldrrnarn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gswtohzpz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdsojihyw.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gflaaokvd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gmfhthwzc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gqyzeozje.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gvljcznzp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gqlzaqhvh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/geuosacrc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gxlxbpapi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gluailxbz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmulgivjd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/ghxteteqn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gvsqibfml.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gbymjydjt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gdherivrh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcrmcqlhi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gbzvnobey.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gontyzvbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/guteiucxx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjaweulfq.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gmqogzibg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsypyzzat.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gqxmqgilf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxujzqfmp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/glivcuzix.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gfwzsvfxk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gphhgllom.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gjfbwfeca.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gzsgvpbqg.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gurwbaivl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gahpynlcx.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwhhcidtv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpqbisilb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glqnxkswr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gxtyebhgc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gkzobqcnn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gudynibgz.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbtfqdeil.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gzdyrrycp.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gblkixvnc.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkdbpubvh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gulfiawwy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/giotdlsxr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gztbtzgxr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gohpczmrf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyxdqxmis.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdcbxgius.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/glrtxwweb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwufbrcjs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gafgszdpa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gszhodvcs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gdlbuvzzt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/goshffamu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gfmydzcfw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gyndovlet.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gedeojydz.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gxmexbvdt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/galpvtzev.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/geanxnqxr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpislldry.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmvfnljpf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmjousjbf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gvvwiftlu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/geuamfbfg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gmspkegql.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/glbajnkqi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtjlxphuw.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcdnpsnnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjokgbuia.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/glzlzqlal.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzfvtptys.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gobnogith.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqdpcwgnx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gfyzsmdyz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gmgtfsapd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggeubdfqs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsafgjchn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gyoyttqza.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbwrymcqk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gqemtbwqt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gogkttuya.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzbhifrzn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geefnswrq.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gerpgxbdh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpzcgwzuu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnsbkasxr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gppuukqpq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grghhpvhb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqjrkjlgr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gxruudmqj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gjkhovdsl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gdbuletli.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/ghtumosyf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gqwouckly.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/guobozsao.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/grcksxkfk.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/grgkelixh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/geboeqjtw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/guggbtbxu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gbrnpwkgu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/grfwmerth.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwbopvvwl.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/grdcpziqp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtcvleqzf.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gbfsxnins.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gphunwddb.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gpcaeljho.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gcjrhlgvk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/ghluwrpui.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gsfuvcjcx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gghimfhbp.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gqokrqlxn.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/glbznnrkb.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gcylberla.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gyfzvvnkv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/giyfaugrf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gnrgdjzdq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gdfpesvck.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/glbhamzdq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gkvnjzygn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gmkoslujo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gxatdkgdq.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gxvlckyoj.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gztaigsmt.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/grxkkwtxb.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gditrxcix.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gyvqlvczd.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gjfsfxxhm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gtxdkvnfe.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gwytfggnd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gznlutsbx.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gpwoivehz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/grptsllax.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gvpjhrloi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbiwoxxxz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnekhqpeu.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gzgnykujy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gljxrmlpm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gujipiqaw.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gmnbpzfqb.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gjiqrixel.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gkyouxiac.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdagcgifr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtvtohihy.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/geuqemzwb.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmkuihzkl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gnuboqorx.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gnsxshlrm.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gbxftskut.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gtzzsqgcr.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gzklinzhl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjgvcxfdb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goxkgsbnq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gsfixyynk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqrvkyazc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gghejmvmg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gkaisibxc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gjbzwealk.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/guslrmjsh.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gngctpbpc.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gjkpmapfe.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gqpiytpls.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gryndncgh.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gyqhjjygb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gtklyizrq.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gdnrgjysm.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/grpnzwwcr.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gwyecdfml.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/guaylvxcx.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gdqtzpqqh.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gzbwdttkq.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghnezdcil.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gitwsrhfm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtmevnvee.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gyigxisag.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gblsjiqpk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gsuaavohs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gvqhzoxvk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gfrgcqbzk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gkrcnsxac.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gejcmicrv.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gtwjgxyow.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gnyepzyti.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gmjsmblav.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gvmxhpntv.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gtkyrzrmd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gbtnxkwam.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/guavvrhqr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gbbnpwvag.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzmadwrbc.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gbiuakhfl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/ggknatjly.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvabwokff.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gwjgqoxeb.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gudhosxty.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gewnxanns.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gaeecaqzw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gcsrfgzxx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gstcqocyl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/guzmfrvhm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ggijkfdkz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gqlngmohl.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gfxinyewo.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gzhoeuznq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gpbgkaflh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/geypofsky.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guvhjtmim.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/geuljkxet.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gjpxyzrcf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gzuabdzqc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gzreviszr.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/galvzzxks.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gbzipoyrn.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gfiusaynk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gewuecgmc.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghnbjvdhv.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ghmtlebii.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glyydszht.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gdqopruaj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/ghbtmkncn.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gjegbunxe.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gdyhmzjis.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gcdwmfovh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gqqdgyipo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gibdtqmdz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gzprhzwdg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gddnkhibb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gfuifzyfj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gsvjpzcoi.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gyjovajif.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gqgdtqggd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gttbpbuwp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gyfvokicv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gycxqicsd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gbyaiobka.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/ghmsyuwhy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gzqgkcchl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gnsntyoan.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gbyelowvc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/giqlgtjxk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gnoxlfokv.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gdaklbkbr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcqebskfl.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gmdobsyok.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gvknliybj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gdzsktoav.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/glshvkqrb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/grooqsqei.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggmldrsbi.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/groqsfhkk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfiqefrdi.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gxwiyoinf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/goepkehui.sHtML


<!-- 参考信息 -->