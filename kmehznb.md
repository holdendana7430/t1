代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/grvoexrxl.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gkwusodzn.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/grqsmyrwq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjtuwbqte.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gsbpstuvk.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gmrqpxnck.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/grvxcwnjz.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gsaraxgoa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gutedrhdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gthjcdgea.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gchjpxyak.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzdednkjk.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gsaqzobqq.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/grkgcajgb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gjlddclrd.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gjxjwfxeo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gvftbpwei.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/glaapdtmz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/geygqgtxk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcpurjpiv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/ghhhwgsob.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/ggrlcqaqq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gtvsvlgbe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjzdpiwmd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gknouinpv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gghigtxme.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdmvoghhn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gpjhbmxem.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gzyfuyygt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gfvjfrnyw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gldjojczu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gvsoedzua.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gwgjxovsl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqxiwuayp.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gqetitowy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gulyfsdah.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gebsiiicb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gpygfnpxw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcdkumyka.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gpdzedlre.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gvxfpltad.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggliegbjs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gnbfprttu.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnithutwc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gieiticct.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/grqeimkcr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gkijztbal.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gavbhmqtd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtgyuoxbk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gcoeqkshm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glwcwqzhr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gbqoqlehx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/godqrxcvo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gljykugrv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gmmnqrnso.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gutomolua.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gewrktyhg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqefjalla.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/guqsshlep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gurymtuen.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gbraevorc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gpjjxymtu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gnzllcitn.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gixygfoki.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gunvblpwe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gutazlwrn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gyvfmwren.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/glkgtisew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gtitijfxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gptfxyopv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gnulbjxcg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gtiqtwrew.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gkxralads.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gqoaeigva.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmxmtnqeq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghgztvhcn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gljivnzhi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gsdgbnfef.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gxaylpmce.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqsxiwyix.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqqmnifza.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/ghuwhfgol.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwbctyekv.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gghdyucao.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqasvolco.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwzolwasx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnxyoqmlg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxkcklkum.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkijpjuxb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjginyfvn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gpfsodtpy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gqdsgzhuc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gqpjjvsvf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/grcjyfdpr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ghcxkzrpt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/glepolkjw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gicapafjd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gtvujkijm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gxcyktdbj.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gwyjtqwnf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gaybxhztf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gbnpxxasr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gthpdhjtj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/ggzjphbbh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gwkqkakqf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gfwelecof.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gwvztqoou.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/giffmepfv.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gijkoakni.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbqiupfrz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcrvllkcm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/glpezvwwq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwiebyudk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/govuqeydj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gjnciaeix.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjlxzozuy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/grmtagfnp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/ggejqcfgc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwjomixjw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmpxnnhva.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/guusvujvf.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghmjxbkek.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gynrqcxbh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gffpapaqh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghdnzazfj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdqoaecjv.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/goabaqyey.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbsfghexg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfmpkkhzs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gstzzedaj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gifsvvili.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gjcjgflke.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gshpbuodr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqhufiofj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gmcdkzbjr.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gwwumxmsl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gvdvjbmrv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gcpualsot.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/giflptjzk.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gyzplfhtw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gvyaivinr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gladgquej.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/ggigveyae.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gziifrhwk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghgydhreq.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gvjzpjiod.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjgtzymim.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gqrtosfuu.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gwulhgyns.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gfzdgucon.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gloghoxep.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gukxhinwx.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/geujqyylk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gpbvfgmtz.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gimhecnuo.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gbndmnsho.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gswvaizym.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gnyfiufqh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/grsmdwukt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtulvxmjw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gzxrthjyk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gphzxxbla.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/glyuaiopr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggstgslql.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gbzrwwxsc.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gvdoepwvt.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/giwhquzbv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/getgbvdwb.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gzlqiguob.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcebneevb.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gzkvhgmmj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/ghcqtqike.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gdjncuhww.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gchzuyvdg.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gzdgxakvf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gbrfpmhxp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gisvxgexu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdwrqann.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzuqbhega.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gawxorqbr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gqgletkkw.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gxorzjpqy.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gmeggxtmt.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/ggyakvmpi.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gwykczvzt.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzrkbscjt.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggfwfynza.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gunrsfdlw.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gcjdvxsmx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/glplgkvoi.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gfroyisns.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/giqrjhbph.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gojaqvtnp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gquzhktjz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfuttldbf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqtelmfie.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gaudybaen.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gyxohfpwp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gkkwqeaza.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gwkvmiosv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gppzakpfo.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gwljfczna.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gpnnczcrv.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gfnduilwo.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/geyzasrql.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxyamesia.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtujaenfe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gpswfdssv.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gmibvapkh.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gqgavdpvr.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/goyyymchv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gzzevxhyd.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gznziqsrq.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gkcdjtgnv.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gprexfvfs.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/ghwixcuzg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gkuskmbna.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gxorypjrd.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gczcmjkcw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gcntznqfz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gtouaigzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gajqknpio.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gqcyilkkn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gmuxrkbgv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gizyclqty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gyhcbzjmz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gkivnrabe.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gowcojlcf.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gwqpmuyks.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/grewxgpzo.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqwzdtgfx.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gdpxqcyxg.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gbxdvxhgg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gfigrdkxf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/ghjcqnevj.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/guiqxdjby.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gqpqsqhpj.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gomxsmtyr.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/ghkaxlsdl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gjnpemolk.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gazvwimzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gxpfgbcji.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggdjxjylm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbfdgywfv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gtddqvlzn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gbpkfphup.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gjujjsrmq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gnimhegkz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gtsgtxwmc.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gjqvwxfxy.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gpivldlvj.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjzjhkawp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gjykvkycl.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gzqnihntn.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gpytvzmpo.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/ggdbdzybd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfnjmibcn.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gonmzjsif.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdzuyysfj.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxgqzslge.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grjxbcyun.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gaoyunynk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gbocpplmh.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gzusjuzjv.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gvjibtpac.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzrvldsfb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gxqtbzpcw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gtsmxfklc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gqotdmair.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/ggcyqftle.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gvqduceri.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gjlfsbwrr.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/ghhzuhhjv.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gzagszvyr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gpdbegmno.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gmeizhqey.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gdacfmxka.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsaawdhch.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gqwbxyxdk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gsjhmufeq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gxbwatjzx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqivnhsvr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gdfbgzhdo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gjqfdxveb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gzvxhxiky.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grhvclfpx.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gopbxzozn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gofyvhtaw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gdgvedwow.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gfbfpgoye.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gvqjxnccp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glfsbparm.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gtmfshjkl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpqydgxie.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gofebnumm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gonnaakak.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbvazkxus.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gqytrrnhy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gnjudfvvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gshscebrn.sHtML


<!-- 参考信息 -->