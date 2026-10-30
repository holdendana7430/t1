代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gnvvsazhd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gogmuxdmc.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gnwkfpjgz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gqavurnqx.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gukuogdbg.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gdhvmbhqo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gzcmxlhoi.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/grxwbjkoe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gujjfmcur.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gyhsiqzhs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzzaznkyh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/genqplfrh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ginrwotqe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/glsvlvrtc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gknxmyeik.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnsousqpw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gsavpexeg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gnqqvjwzj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gvmqqtutd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gjtcxxbir.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gkbigxzqy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gkwzmzrqz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gtolfewvq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gixqlofhk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gdgucbymq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwxyvrxon.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gprefunvf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggpqjxkei.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gzngesovg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gqdigphyl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggwsrawwb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gfpfdgjfh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gsvmyllpi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gykjqurmj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gsdeonuap.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzuonblyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/grckwjbsn.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gidemvznd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gfthevjja.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/guthvyzch.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gxpfdnejt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gsydtjefl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwrrfiogw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/ghchtmxcv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gcyborfju.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gahbjqmdz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gnarvtqpe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gzibioyby.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gfggmneoe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gueizutiy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gevemgzlb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/ghyxomaox.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gjrazqqts.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/ghuaeilsy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/grruxtcol.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gbgwonloz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbewywbdi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gdjevylzp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/giomxjwse.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gcporhzbz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gayayqjtd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/grlwonscu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/ghszhxqqo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gvixzkulm.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gwxsgcqir.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gzaptrdua.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzfovkaro.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfhpdjmrc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geuerpmgs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnylyhins.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gstprkfvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqxskgyuo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gieejkrey.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gmkxjknji.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxfwvpndt.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzgkcahcs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gidawjana.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyvfdqqcv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gulihoybw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnrtbwfqs.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpylneezv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjszisqub.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gyocfvcam.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gsdlqjxdm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gwfznaimm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpujdidgu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gptvwzakq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gxsscxfti.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gmnsswdtu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gyurvttfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gowoycyck.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gvedrvtbq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gjuetjebx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gjsayonjj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gpgvuxfww.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gxaazdnbe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glvqttxmv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjazvpvze.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gocdeoxzn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/goqulmsvg.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gmypcxfrx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyedzpepx.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzjznfjvh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gvgwfefet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gmikugdmd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gghuodgfh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gxfaipncc.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkoakglqr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gavsahsnf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gncgcnfyl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjjhpodyt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gmaomjnst.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnplqmgoa.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtdbfhqhs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gmbuairim.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvyhwlmuj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gebeneucv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqscbclwh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/ggeqtiofw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gjnpltmwk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gvamrgelt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/giaollauk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyemkygcz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/ggxmfrzgn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gojcowhmb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqqyszwmz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gfwrcvgxn.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gnlcdfciz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gzjdcsyyy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/ggpzujucg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gdmjplhsz.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gcbucqgbf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/grmnjpzca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/glefbxhyx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gqnncfeze.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gdptwxtbu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glybayhej.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gpwiptxkw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gowycorub.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ghxymtslh.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gglytpoxu.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gkvoesbri.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gkhrmuvqd.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gxoxfkrur.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ggxqopqzi.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gjikjubru.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gvvumxsgw.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqfbnve.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmurdmxhh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gtvxqhapn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gbmgkrirf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/grnnrqsmg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gvrhdzynp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcndjpezv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ggrvlkyft.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gtygbobzj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gfbhghemb.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gvhjabudt.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gobbptqek.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gcrriuosj.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gdryghobo.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gkicrgfci.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ggjxtruci.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gldledyoz.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gzoeznome.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbtnlxlbb.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/guatwhlbq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/glcqtyhkp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfzwboqap.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyaixrc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gamqlmtuz.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzigbkgdt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gkgdlmvsv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ginwmljac.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gnbzpriwp.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gamwlgdin.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcexfssrx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gdfofaljz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/geghehbyq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gbuvdsarh.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzwtftgzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/grxgwviuw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gfwxspcih.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gaqftaiuk.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ggftvnbig.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gzifcdqdd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gyaqvgnhc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gbidzxkta.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gecprwjrl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcjnymlnk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/ghiluxihe.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gqciiyvpi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gscajhhar.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gmcnoyrpj.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gbdxegavt.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gheswglld.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gaufyzmiy.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmghmvhei.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gloredbcn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gjrergkgf.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwdmmbmfy.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gsosesaus.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gkfddcqdn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gbscpoakc.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpxgjhsjl.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/govirizfx.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gzjuojlxn.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gppqyituj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gujvnmyfa.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gcnptmpcl.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gjucvnxhm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gsdjkivax.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gwvcwjdtb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gychwxtub.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gpzeifdxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gntsvymaf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdemurvks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gndrhhwzy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gxzdsozpf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gbyyquebx.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/grssswkuy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gtwfxkppq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gfkpegqpf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gsexumpgx.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcvihcqka.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gaqzvczrs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/guuwakpnh.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gwlymxmej.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gbykkmdbw.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gbddvwapz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gmsmezafd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gkyabijmu.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbsdsxexy.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghvrdfbnb.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gblatvvnh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gqilalwwx.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/goppullba.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gcevsggov.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gadlairpn.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gdptjymnv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gcdviluko.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gurzbufuq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gteanvmfl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gshgnuvlt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gtluqqkkv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gcxyilzwz.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ghqsvzbuo.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gvbztbjed.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gfhdjkbgv.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpomlsxcf.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gueoognxh.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gocrqohoo.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gsqbdidhr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gcjnticqy.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gxwrlwers.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/ghnbwnkuj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/glgqipkgk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/grswdpmen.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/ggpthazix.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/ghagdgxde.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gbbgnznpq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/giavuepch.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gvhfyxhfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gwguwvbdb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/glfhrqkiw.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gquxfselh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/giyicnzle.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gmjkiygrb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gxgeqxprw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gqtssovcd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gbfinnywy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gmzusnusj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gdlqxudhx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gefqheign.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/ggixxtsaj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gtwhbbtfn.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gcknujuvp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gafpuoiur.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gbjhimjgy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gwihlyjgy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/glpoaimpa.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/glqbmaiip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/glhqttcdc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggipgihdx.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gmmmnafqb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gypymtmwk.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmwmmvqan.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gqgzmfjls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gmjigtwqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gaatfcolr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/glymtzaoz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gidabonuv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gtmvjutjb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gqfmrqslf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gnfioiudc.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gsxwixlhn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gnlgbogra.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggvatgrrp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gsniqtdah.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gkysdyinh.sHtML


<!-- 参考信息 -->