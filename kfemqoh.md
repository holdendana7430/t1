代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gkzabjufd.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gqlexqcsa.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gqgnabzxv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghfhpntcw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gezsavwna.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gmntvzory.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gtwddgfzn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpliheipl.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gippyevdm.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/ghsohambf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/godiehlea.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gfpnncpwo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gszspzjnv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gwopxmdvj.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/ghowiynxy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grfinitgc.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/grresrewg.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/ghednbfgq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gsaoadylp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gbkrwhmtm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gbiqbuats.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gadilsrjc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gsjxckdoe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdwifskil.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/guxopcjbc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/galyjrytj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghpkfsmry.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gichrdcjx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/geolabxzv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gwnunibyi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ggiyaeaih.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gcgykzhlr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gtuegkhcj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gkkpeojuy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gumizacsc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/galdwhgjx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gtnxupojm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaxtmavjg.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gjcldwxlv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gouuwnkip.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gbwfeighd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gabcsdjci.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmkbbtysf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gthkjdvsh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/grbpzvame.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/guynevwti.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/grkgraggo.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gystffimi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/goidcgqrt.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/glufklsfx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gbiiebron.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ggwdrhphe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/grcaznqoo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwnbiwstp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gidqfailc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/ghxwkpafo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/ghazmgaao.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/ghcmrwslr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gotjypvqu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gaqvdakwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gjvuctbcx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/goovlnkpq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ggkdyyihf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gwisdmsyh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gsuughdfp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gpbqrdepy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmfsszsxq.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gviczzrdd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gbxawrfgz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gnpkciaem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gnyhbnhfz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/ggpisvanv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gppgktqzr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/geoumlkge.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gaxnechek.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gqddhcqoi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gxjckcyyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/geihhsloa.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbjmajfyl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpwbjunnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gastlhgri.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gszllyagm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gciyzfyts.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvquqwcje.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glfdwogjn.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gikpzvheg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxvqxmgya.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gruhqatle.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcmtykcwk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdjnxkjzg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gnlubetsd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwcaowxtf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gupnxcqbx.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/geagbznyf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gcqrpbyzw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gkwmeaykb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gldvoogzo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gwuqyncep.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gnchfbwmg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gozafcnwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbucopnh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/graukiryj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gcevwsfck.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gdzqwkesh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gwdccxzvp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/grchnursq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gdraoflny.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/geghllkku.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gvuklowoa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/geujqcjyg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gxmktmmbm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/grejpnpfc.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gfolfunco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gndwhkgwc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gffuuaieu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gpvyuitpw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/goeankvnf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gzswlhaum.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gcamqxudg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbmmcdgfi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gjxocuquk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/guukcvmnr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggzctwqkj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gihccebyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtenyueyh.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcwmzdgwt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gmysyqepj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaqujvclg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwhdlnnfk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvshxxyyr.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/ghbngkxih.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gevwayovk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gaufftwnb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gpynqlmij.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/glxuqyzwf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/geoonytuh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gtivvmnfo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwvtwvdzv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gkdkzorlq.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/glyzehayi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gfcldypob.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gorazrnbg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/glejzymna.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gcyuyagbk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gaxyysugc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gfutcfkff.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/golsbxlfb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gtzwtvzit.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwiahowrr.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/geqaldxgp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsohtnees.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gevcfsbql.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gipygorji.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/geceqbyoi.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gzopsruee.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gsyuzyrvl.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gfzkhnaln.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gzcvmlyfk.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gpjvwupwh.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdafygqkv.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gogxkuygz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gblujerfe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/giikeyeob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gapntetzw.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gjqtbquql.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbxoexrbh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gzggrscim.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/ghcwbzyvw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwausgqbp.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gdptsfcod.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/guhlgcpjf.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gibezdydh.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/giuhjiujb.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gtdfgvwuu.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gkqhynbhl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gmakausar.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gfscmwiso.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gxftiaeaj.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gjdicfmno.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gthecespi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gceklqkay.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/goitdjhzs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdilqbnhk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gymztlmvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gskeopypg.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gezkmshns.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/geoihkryj.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gsyvroown.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gzkexsqts.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gzkdrdnmx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gegfwruxf.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gtgahcwrt.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gclnooxkd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gawetymor.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ggakxsgap.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gyfdbskod.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/ggaycewap.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gulsjyzbl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqutewwgr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gggovjxil.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gauhxydtt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gqcagxbed.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/guodwbqgg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gxojmwifq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/guwhjchnp.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/ghomigvgs.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gupstumwl.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gzwrvvsqc.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcphriufc.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gpimcxovr.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gxrntteyn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/guvfsvozd.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/goahcoexm.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gvnqfsuoo.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gdwtyrdqf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gfngnfhre.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gvzqfxwsz.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gnjnpkhoi.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/giypmjwii.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gsqxlzoxa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gpfvqtpcb.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gpmebwzax.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/glwykogpz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gqszkaxex.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gfejwymjq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/glbqrkhry.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/glknmyuqw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/grrejixra.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuqwlfgx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gnbywvvwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gteadzhqz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/ggoymnmzy.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gogwlcltt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/goandtdwt.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnqpuzuig.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gilmguutw.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gngwrfruk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/goompmvmj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gvesadaeu.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gkbjncinj.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gktrdiwgy.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gyrmbuzfd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gwicodlfn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmeaadhpe.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gibphuvzq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gaebdmxtr.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gfxsksmsj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gctjbbtmx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gfgdkdtvn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/guybqnspt.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/genanhbhe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gzjezodkc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvxoqkwdn.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbxgcfvzq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/grfajatsa.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/guovqeeld.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ggkdqbjwd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gqswckcfa.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gwmquzauc.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gehcjrzwj.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/grdnuwnnx.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/geyihttjq.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gdyovjrra.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gmivysrms.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqctzdzak.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gkidaqsff.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/geaxqgjvd.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/ghwlyueyj.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gyluybvpw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gvdvkfphq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gayrypotp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gaywysats.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gzluztsan.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfiksnwaj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gqivrebur.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/glqucpymo.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gplfmfysg.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gnigveddm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gwsvitduf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gmsiaigqv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gdmchmalv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gzqsmkiqk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/grcdotcfv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gmwubizsw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gdleaabns.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvmjzpfro.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gqadyrlwu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/glpjitnpm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gxdtmilje.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gdgxksuyu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxduzgeux.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gbwuipthd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gsjrwjfum.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gdffclgdn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gznlcamyt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcmvabeau.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gxhtppfbf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvvetaimc.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gytrypeuy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gluozbgmv.sHtML


<!-- 参考信息 -->