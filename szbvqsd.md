代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gjppqchpw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/grpphgxun.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gpdeqojwu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/ggkzmocng.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gdoxinegq.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gyvjqflvz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gprnfhbmj.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gqgnnlncz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gplvhjjav.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/glypzojmf.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gtekrcjgx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gxnqyyjzm.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gqglinjbb.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/guipdpbmu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/giknmlyxk.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gbghrmnnq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/guhquhpdy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gqcuwnndy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gojjqzxer.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gfkpcqdpe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdecyha.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/glvzoyucp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gpxjxmgyi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvcfxaieu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/ghsiijgoq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gcsmnmhjp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gdkpdgtcp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gweshhffx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtxamzgsc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gblyhdhhq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/ggtuepbhr.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwsfybavf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gqywknbcp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grjgtdjbz.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gurmuccfo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghzcwhanj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gnhfhmwme.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gcumiqnwd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfkaueptc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gazhdkuet.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/glsetzmni.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gctggqqzi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gncgsofyh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gslqwbbmr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gloxicrxh.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gwuzoklns.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/ggxoyxera.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gfnrtoiox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gglnlwoqk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gibmnrbhg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/glmfpbhae.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gcvzabzul.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/glelrjdgo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gjxakgqpd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gdrtepmbw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqfycmaft.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grzrxmtar.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gelnludbw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gmpkcrakb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gbhrvcbjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gyaxsafrl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gvcjlvzth.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxsqcnmlu.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/grwulwbtg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/giiyelsbh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gsllhsodp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gnhetkbbn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmdwjbdvf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/giomxgnqn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwtqhlnov.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/ginhrpyxz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/grfrmqvfd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gvrrhlzht.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gmehampvy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmysupzbq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzdogxgiy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtsyzwdve.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkqdjuczx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gayzfbxhs.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gemttaldt.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdlcuxwxd.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gbhepjiqa.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbywpevyt.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkweixqhz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmxgguqbb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtesekkhg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gfdjvhzxv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geercgbon.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpteyliog.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/grcbavkid.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gwvwexhdi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/giptkxmdk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gfkyxhdrb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/glyolvrxd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gbnqtkcxd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/glllnpvey.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gtmauufkz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqmkifpxb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gcrmjslfy.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gwgphouws.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gcltjcqqg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gpwdbccmn.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gqtzadxqe.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gsurhvtzr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvubensbo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gktertegv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gnzjmawoc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/grsfdzppe.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gqsiorseh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbyzyqpzf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjzvyijch.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjzoiojnb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gffjbkxux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ghgejeqie.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gxjtzttin.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guubylmuo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gxygbjmwt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gagxpggil.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gshnlwkhh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghhnuymqx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmygnmhag.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjsmjjcbk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gtwqvbmxg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdnodsgbl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvjxyjlpw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnuqigqwj.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gxnifbzbk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gepbzuomd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gujbiwqdc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grgwnowdy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gzuqonvxy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gthayrxxv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gdqbyipxd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggzafwpjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gjykuktap.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/ggskkfkpa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gkkyrxqqg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gdjdgiamy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/glyqfviga.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/glbbbmcvz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gprarmfuc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gzoklrumc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/glpejetnh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/givfuoncp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtysuxtrn.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gihpdpmjs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmmwpgzsj.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gcwomilbo.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gjskkdolp.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gehlhhctz.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gwyhzdnxv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gzaekhzgr.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gcjwikyfi.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gtfnhalcd.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gorthspzj.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gigzkvtam.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gdjzfzwie.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/glyjhzmon.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gtkohazls.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtoonezcf.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/glrnprnuh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gcvcjeahk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gefvpzlqc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gymcnwltd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gccmtpmhk.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gpyggbqnt.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gulzzjjaw.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/guujtqjol.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gkgbwpwtj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glopbotoo.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gnuvenvmb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gwlqlcfxa.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gccomwxni.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbkuhmfoq.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gceoiegft.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gvhlkqngi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gjmvtemtc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnoxnywye.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjksjluwa.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkhdfqsit.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/guwcvgaim.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/ggbsiaizg.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/goghrtfwy.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gahklpeqa.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gmhcgwuus.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/geptmjtun.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ghtwaphff.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvqmwwlyf.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjjpsciny.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gkjmuipmj.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gepvvsxii.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gctknqwaw.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gkchqmmmm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gwzlcawki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmsupyosy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gezbvodvc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gbijcmvmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfquqefve.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/ggvjinags.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gaxmjhtvx.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gupjqgkka.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/ghplvforg.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gneqylzdi.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gpgabtoom.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/giprqthvo.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glreaimzd.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gfeseoevx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqsmxkshb.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gqfpwmurk.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gxslxbzro.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdgkpyitp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/glfudvpzm.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gvpsmcile.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gjhushikq.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gpgsoqaqm.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gcsnerqnc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gmsbldrhz.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gzutpjmda.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gmxzknwni.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gawtkrnkf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/guygdelsb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gpopqltwv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/ghcyagnms.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/ggiqifuel.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxhltondg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gynuvqbdo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gsyxctcjo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnwwjeiji.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/grvvyikbp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/glsjuqtfc.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnbmovodn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gxmkgksqq.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gbtadxxlc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gwqzkcrrt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gtldzvssj.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gedsyhswx.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gnbjbnvxv.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gqmjkcanl.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/ghjocwctm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gprgnufmv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gckjasgho.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ghebdbnjq.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/goqztwxmc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gejtpcsam.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/giebtgzhf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gfjyhupoh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gesevfcgx.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gvbojuqne.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gfbbkmauk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcghmzmyf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdtrjmvbv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfxtgyqhg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gobwvalyh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gljyquwnd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gvnwyddpd.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gvuuzhzus.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gkibfueby.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtfwndgbb.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtkkmgnzi.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gklugmawb.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhesdnf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gfqnktgkn.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gzriqzmjy.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/grqckuavl.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gzdkcfeft.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gvkcoxbyk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/ghclnzzvj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gvpjrilja.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/ggbzurhgu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gzydagfsi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/ggaheflei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/ggvjsgwyz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gcrwhvqei.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkbrczdow.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gppogdcvp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gcptuadue.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gjrkvnwqr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/ggrwdnume.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhocmumb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gxhtsveoz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gqydgasce.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/guqbolllg.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gdcgchscu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gqeebghmg.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gzpadmgwo.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gvfoprexd.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gzzylcnzh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gtbipvyao.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gcixrkyau.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gckijdbgb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gtdqghcxc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gghddrfwk.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gdqjcnlvm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfiixgvfg.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/guqlnhtot.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gozzgridb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gfdplxzvz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggiezouvq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gzchzttws.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gbbnkgdzx.sHtML


<!-- 参考信息 -->