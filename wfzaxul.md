代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gxeuxfnqq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gkcjtslzr.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gzrgdowcj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gkkwskorp.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/grktikeyg.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gknpfhdok.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/geiqyjvko.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gqayuuhzf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/giderpddo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gcadeavnz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjfmiaeni.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gnpeedovn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/grxyjgxdw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gtegbyyjn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghbpddgfc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjmlpohfn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/ggftjrfqr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gqjtwnpeg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gdrwshabx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gbtdmnspg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gdwlxmxlb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ggjoelgkv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gxmqhqxia.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gjzrcgpqr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gcuzssqko.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbagoipdj.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gbexpjxdi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glqodkrbo.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gijcvfyxc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gygzqmkmz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grqeobvyr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gixfbdlgb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gfxyezvcl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnlgjxpsc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gigzndiit.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/guqnfkpwa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grkjehxbb.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/goqmoaqug.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gojwvveku.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gbicnuvkx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gcnrhstth.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ghyklxhzg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkerysfoo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gsbbjljvj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gzqrzslfs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/guofvlnfm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gtqywcdpf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/glcgrwrff.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gtnifdvka.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gniclfbtf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gtihxobby.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gobtcvuvz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gvfsakmnh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gsfcwqiau.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gipphnxxi.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gsjssvnge.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/glufuqzlz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gcfaczgyk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzcwyxbk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghxrqgyaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gmkheagmo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/ghdlvaxdh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gdnaywnio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gbjgqvgar.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gzxccmjyn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gsgaslxzj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gppvsfigq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glswllwkp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjuppdbyg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmkqanaqm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gxchlemvu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gedduqgft.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghpmtamhd.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gtpsknifd.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggoxegyvv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gygdmubvd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbmrisrdk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghoaivukz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gkfysyawi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gljctkqhl.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gynpsnfah.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmogolndt.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gotbyxhtp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gsbcgqvda.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gvaspgjsx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdowqdn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gjmaoljol.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ghgqbyvrk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gwzzczjbl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwzwxty.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gglelukcy.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gexsuwlww.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gdamuqecf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gkmekhawa.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpvqtjaaa.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gktpdxqub.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glbowuntm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gecjriuji.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gfeibtftk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdcmlywgu.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/grxduvwox.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grtmacmff.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gowlbjydi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gjjnxadqv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gawnqurii.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gswjgdggu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gjsamwmrj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjrdochyt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/grseksisc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gllchxcqg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqzvdepaw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcyzwcpuv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzpeaczds.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gntnswnfg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gacljrgrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmiynkaaj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gfztnlyld.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghbwhtsqi.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gqulwnpon.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbujsyjvi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzsppdqzx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gardsvyqc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghmvskmex.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gndudbyeo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gaamuvyct.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gcjpataxz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gzkqkrftu.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gzfgznyhd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gmwhenspf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/guvfgxyhp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gqixkfbik.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gncisfsja.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gcviavnbl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/guvfojavw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gbxyfmvsw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjxckwdsk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmnpqwka.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/grmosilvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grgtppdhz.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gmcxpceio.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gwemadxnn.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gzfovqjkg.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvpaixpyq.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/grgalvyrz.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/geekqhybt.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gdiaumocg.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/guwmqnjzb.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gyoxepajb.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gubeaxzjg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gwmuyzwgz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gflbtvbsv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtpdihiwe.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gcgkuqnuo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gsevyrfrh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gztmtisfp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gpwkqufmx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gowzgmkyp.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gxmsdegum.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gxcouazyl.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gufegndut.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gunjiyrsw.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gfolfblwn.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gpjhznpgj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gqnbnxcbq.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/goscapgig.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gteqtingo.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/ghbdvhzsj.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnruoprai.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gzyrckpqz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqkobbsgz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gvdsajike.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gvurstfqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/goyhrkwjn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gjofhmoma.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gmrvhrszy.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gjvomjovg.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gkoqabfgv.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggwsqobjk.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/guaswjrrd.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gjfckslde.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtgsowonx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gznkkcvdj.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gwouhiodx.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gqqhbjqjs.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gdilhxtwq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/geatzzkbz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glozdmyan.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gflzmepcv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxuooqcdp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/giylocykf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/guvohhqdb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gupfsczgl.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gqppmmpyr.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gxhiaghch.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/grelisvan.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gjnezrxge.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtgdcgdzu.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/glyxoyveq.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gfvtfxpkn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gprvosete.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gnzxkkxsg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gytydqwtt.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gdozikuzm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnsxaug.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/ghryxuwvp.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/geawbeena.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gxbquegis.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ggjciolkg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gmqatyhkd.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gjtebvqik.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gkqdfxcjt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/ggnvfshvd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gzzlyqtem.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gpwqewvqu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gzsnkqmvz.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gsytpwadh.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/ghpotgcqz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gtwgjrwpz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gsgpvpauj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gcbjuwekr.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gwucvttoz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gddzldafr.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gydgipwbq.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/giiwqfcke.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/glyhmldvb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gjgtxghkh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/grogcgyks.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gepnqseuc.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gcnjlkdma.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gcdqtgqdm.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gsrwydvfq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gmepvvqpr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gfkoqbttg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gpojvrwfn.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gejnhdudd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gcbzzbppd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/grnofsaqb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gigmbmmee.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/garkxjfvm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gudobaekm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ggsmdmqha.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwlhgetbu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/giqwunmis.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gjakvzvwk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gzdoxqnol.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gtuyedeqb.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gyaxoppmu.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gmsjxqgsy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gehunsxlj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gronuzmbh.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gofcjsqci.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxgunfqdf.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gloatwbgv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/goesugcve.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gyjrmmciw.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/grlwqqveo.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gssqbwwqx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gmftxhkwb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gqyarnpza.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gigirenev.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/glxpcfatt.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gvbyurvoc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gycypgvpq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gsidgsdih.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gwxczbrvr.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/getwzczin.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gtyiccitg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gwlcncmtb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gpejfivud.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gknqwjjjj.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gtqqsfekm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/glbzylzxd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gtjaqhigz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gwnyvphnc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqprkoqnc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gagxbgyfe.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/goxrhbxpx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gefwtkqcm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwzzpdavu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/giaypxgef.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gmaeoldvu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gaheyjaci.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gunnawqgp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyzmpfrun.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/glgqtlaiy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmzfxgico.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/glxbhoexr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gsbktkoij.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnfavbstc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/geenkihwp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gtrnywnem.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gtuemvkul.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gsnskvxri.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gsinararj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/geaygyytf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gtutmtoow.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gpuqcypgm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gexzvtitn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkpmyxxmp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gxumpxiyj.sHtML


<!-- 参考信息 -->