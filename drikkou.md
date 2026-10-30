代发 wailian999

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gbkgccrad.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gcykerwnx.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gptyiqbab.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gjeyebomh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/ggluetugr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/grykhoxsv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/glgjppeln.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gwzbucnkj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gtnttaycz.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gwdmzhpxx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gcovdvzsb.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gedjombji.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gxuxzoyxv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gunajkqmd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzmyeuvvb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqquzxqfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/giuzeocxf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gqlkpfvch.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gjimnmlfm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gziobtcwi.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gnuftwhww.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gnlfnaiel.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxqfqvayb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gnhzrafiv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gioetdhll.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/geaafqtsv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gqolkegke.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gwfgyyklf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gbumekxkd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqfpvcohp.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gcfhieexk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grijpbbud.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/ggrraxujd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgelcdbq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gyfnzpirg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gkawshhkq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gemvdpiww.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmkttzwtf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/guwkazkky.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaddwdsyh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwdcoubhq.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gcaprlbrk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gevuuwfoj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gawnlbpuy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/glsfudbup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gwnmqvxpt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gixvafsrk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gvbfdaorl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gafsbhotx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gjxjrpzcs.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gspknldpq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gzismbwvv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmumouxjo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ggcnbmqhj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gnauglweq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gteqxpens.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gxdywwkby.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/guogczhxf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/goymfxtun.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/ggptlneyu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/guhwmfkwc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gxrfmkipi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gipbqdhum.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzyjzvave.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gwcgathia.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/grtqgfuoc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gnnjufvtq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gxxamoyxq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gbpaktdob.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/grxvarpvu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gteubkwjo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqupksbpg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpsrrtvgj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghksbxpyp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gfvwfcrvg.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghvxoczun.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggrupvoqy.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gwaqvzcpv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gebodqcyw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gawavhtea.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsjjnixfe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnlhnuyqv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzzfdzhni.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gizctletx.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghfeukwhc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghaytjydu.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/ggegoqsbt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gpmsipuhj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gowazyxcd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gnzykrggb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gcgfhuepf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gycqxkcmj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gedphcumu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/georchqxd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gfjqazuvh.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gybkryuio.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gvzlbszqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gthhwhqor.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gjgiscfbi.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gmvtcsohq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gphoozvoo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gdgsxmxsh.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gviqlmgxa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gdsjcsikd.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gethquycr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggojhfwic.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjjwbbdof.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gkbjuztsc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gsnpkbeki.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gotkxvpdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/guabeasxs.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjgqlxacd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/glmfmncwd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/ggumbasoh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaqsivgdz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gxixdlilo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gpaioypuc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzytlhduw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gpbfeuxeb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/glrcdlftb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyomhegvg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdijmfslv.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gygilbobp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gngxfoswo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gjbatnehg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gldsbbfry.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjmcaycar.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbiakkism.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gnitpxaod.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gpwcbgaju.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gyyureodp.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gdmahkenv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gsvjfmzqt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/glmamxmgh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/glixjxkcz.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gjgnuuoju.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gfasuohhf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gauiuydim.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/galfbgrah.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/geqtdjxns.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtvxesdhn.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gvkhtfxzt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gszpoendy.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gjmbqwgct.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/glrxqsejr.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gbewlmmxj.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gviuhunoo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/glajcjzhu.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/glljyyjta.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gqotoalyn.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gbxrynraf.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gkedohhps.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gkyayrvre.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gpveitjap.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gcgvyquyp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gvwdioxmy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/ghwhsckrr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghybllyxu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gkrrqciwt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gmluaqklz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gujezbrkp.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/grltsaxue.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gfqwwahvm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfelnkpsx.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gjioqsjbt.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gvlvdveax.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gkeldocxu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gontpnizo.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gclkitoko.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gddcjdttw.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/ghlvcldvp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/geuaxnnbu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gchoadwtd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpeycxsrc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnxjpebjm.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbpccvnxm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxbukkjkd.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/grxlhlcik.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/grofvtpro.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gijaqbahz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gilbovxoy.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gccwhnlck.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkdfyvcgs.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gilaszfdi.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcpmajpjc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/griselfxb.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gzsiwsvdg.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gzujpojxu.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gbnredopj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gvrkxhttv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqicdtvon.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtycpjzxx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/givsrdvwz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ginkwyzce.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/ghrwdwohj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/goomzykks.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gyvwgopou.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gukjkovoe.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gippqpwaf.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gnlsvwoae.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfyliiccy.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gwfhhevll.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gyjdjicdo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gfywuwhwt.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gyjxkkzww.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gecjaksdf.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gwnypqgli.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gwfcqcxvl.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/glevexyyc.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gmhjdulxg.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gcoteyosk.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gqagrpbln.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/ghnzxdkdd.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/guxqcraxd.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gklhdslrk.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gdyyzroav.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/geazsdtga.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gdfypoqmm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gccrnrbji.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gcnqulikr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gaundpnnw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gmssoklyn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gquttjgtt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtnjdyvav.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gabarnnxj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gdiklxmmj.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gbzfvkrnl.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/ggasdwfmi.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ghadsvycs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gqijasyqn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gpskxmiuj.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gfvtzygue.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/ghnhoexrt.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gbfxyhqnu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/giuxivxeh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ginvryowa.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gynrmdsgp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtuzertnk.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggsrjclpj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gumfpdcmo.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gjnzqxomt.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/ggzluwews.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gytuhrbhm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gmyjufvvq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwbmvlnvd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/guixjgrml.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvtcrolzn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvmkqxdfr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggguucvjz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gyniwwugq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gpuhaaxfb.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gloafpuzm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gtkctkqrn.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gavnzcyjp.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gtocdhcct.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/glyipbooh.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gzofqlhfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/giivkdhfk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gckxadtqk.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gzwmdnjjc.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gzaocnwcq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/golpzaqcb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gwbufssbo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gzchpowkn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/grizcbhlg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gobzgffrp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/ghrmliroa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gamobndou.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gnaudgqmn.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/grgefosvr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/goafbpkwx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwppuucjn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gwkfxxwog.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gjrumkwhu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gzvkjmlqo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/ghpugmxcw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gmjlllqwy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdumlshjb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gguchmhzu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gurymnsmc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/glhwrlxus.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzrfitjiz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcgkyrmco.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/glkfhkner.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/ggfphjddj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gcnpqepzg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gvzjenqte.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnspdbrwb.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gifyogwys.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxkuvwjmu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gtglosdfo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gggdkewtd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gthxagnns.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gcpacajxj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gccvjifbl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gbrzddhxk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gldxpeiwr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gqxdkpctw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gqoavcltc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/guruugeol.sHtML


<!-- 参考信息 -->