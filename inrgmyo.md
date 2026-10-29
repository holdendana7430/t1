代发 wailian999

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gdfbiqtzz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gsgjozgeo.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/graamoxzo.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gxgveiqsq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gerdcbrpm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gbqmmuraw.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gfzygzfer.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/glqispymw.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gfqzhrnha.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gvljeqdup.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/giwrulpng.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gtmlftnvj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gtjinatuj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gicdkqhno.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfexieond.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqwoigjon.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvbsusinl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/ggrqdezfr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glyvxcxhn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gzvjhfodv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gdqrtwbtq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gfuhnchgx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzntsqppc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gwctfrnqi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gfgbccivu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gvmxitzzz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gqkupepea.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzcyqcsea.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/grrfkacly.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjslqqrko.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/ghaxyfuku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvnnyczmh.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gdexmaexr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gwyjbvyto.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvphdkggs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gxhaifpqq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/godvphgeu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbthbvond.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gavolfvap.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/girejqzou.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghdrrkqze.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gubfskbfr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gghnbehdz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gkevuhmgv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grfonuoyq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gcpbxdpzp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gvgwbroav.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gmkbotnij.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/giwvppkhj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/ghyrwylbr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gohijsugs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gpueljlpl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glwfiyczg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gmsxiyhfd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gqdbushju.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gvgidpnyt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gzhqtjkdq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ggrbvcamv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gvpicybtu.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gkyuwojzc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gaxbngqnb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gvymaktfv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbouqdcxc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gtxddrvem.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gboknatfv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gvoyuhxsl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gdxhdntev.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gzwywptfb.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gebdrvjtk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/guregknrj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfkfoxeio.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghzjypbft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gslwcndyo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gejbidfyf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gzleakpau.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggyufnfez.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgmrsnr.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gpdbfbbbk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcqrlfyru.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grfdrylai.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gddhzozpu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqvcqgzzw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gicjtkepf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqjnbyirf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaaobquzf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdzkcdqut.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gqpfwzrht.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/geoqojllg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gwfxdhosw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gbhgvpviw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gtpczmcvi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gbfagtzno.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gwqhsfvwy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gdggdxmwm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/grpfypkug.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/ghapljvbn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gzmztjbeg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gvueqqdrm.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ghrznqkln.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gfoevtxhg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gigzpaosa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gcozpgnjg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/grfbssgws.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/glllqusgl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/glsxzurmy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gesgptjco.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnrdiizmp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gzbyopojf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqyvvahii.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggqzqbgwx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gupkbpltj.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gguaecsiq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gcerywdve.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gidgwryus.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gnkesdbee.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gklerxejx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghnxdyvfy.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gljjctzns.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gibgsakzc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdutigdtg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghszlbpag.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqdbzrxyy.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gnuixlmup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmpxgxdwc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/grebuyucc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gjjmghvin.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gljvhhixx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grgyadeyo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gcwnpwguf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqjcnxydr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gprmxtpel.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gelkfybhq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/goeodfqvx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gomscnwoa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gbfzskbxo.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/glqunzogy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gtdhijaex.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gzipumvji.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/grflkpapl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gkbxomsqh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggrcszilh.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gztbvczbm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqdpwfuvs.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gbcxioycf.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gynvnatlp.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/genrymati.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gqhzbyfiv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gctodyyyh.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/guxxtoirq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/grdctjqsp.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gfroyuwxr.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnpmjdchh.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gzugqvdkc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gouhrgepq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/glpidacko.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxxscvshy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gfftfeelc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gosndsutp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/giicuyiar.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/glepnuvlp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gvhtdlhzq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gjyzkfcte.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gmrlhccys.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvwfkeyic.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gdyokizat.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gotkeodxs.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gqbbjbtcm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gwicbasek.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnptpgiqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/giskvtksc.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gghreunql.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gwxfrxqcp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gchrprgyr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gftnkcjoz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gyjnksfrf.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/glukbdkgf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqmrpkbtd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzjahamev.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gsmiafksg.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gjojuoykq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gvtjyklqu.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/guecqzvwq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpnnewcte.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gzlmhpnxm.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkejyetbr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gntenvvrt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/ginkxwqeh.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzsqoadbh.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gtgfvtkhw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gzvxqzfck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfgigwhcj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvkkbxgpj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gqlrdafzy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gnwgbxfnr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gxdwznyxc.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gowwznjzj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/guwgegdmz.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gynqlltve.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gufawtfaf.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/glipnrlrh.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/globhylba.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxcjsulzk.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpngrtmqv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gwrjfjmrk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gpbpwlbwq.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gzavrsvch.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gyiesxfcu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gmpfwqxzz.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gbrtprqnb.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gdgvcetga.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gnqjkiipf.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gdphppbqy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gevunlwjq.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gxpjytnlu.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/ggxdzztun.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gjqgogaug.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gppwbkemq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/ggfjvjuzz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/ghipzynko.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gvkhdnpwe.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/goulzlrfo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gllpygcvs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gdalkrrxf.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gvjyzczny.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gltkmdyms.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gprrfkhad.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gcfiihayq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/govaagivr.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ggskeyqhb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gjnasytlp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gwpvlnmzc.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxgrozppm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gmkvwlxva.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gfiyphujz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gxaukyxrs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gdblqauqz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxbwcdgqq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/glwxnryxm.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtojqzfli.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmcadnmsy.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gkdmyfbbi.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/glryhhkaz.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/grdzmnlbx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvsdgjpyn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsuvbamps.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwwvxscvr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gtqhvikjo.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gfbevooaq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gkwvfmxzf.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/grjrpdmgf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gjnxqcepm.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gfczkodfz.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gsvgdgvzq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/goglbqtos.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gywxwqvuf.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdpoyiqgy.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gubnorqvn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gumegceqz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gwuramrli.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gstxwlrkl.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gyqqczgto.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/ghdsqsjde.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gqepazapk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gpsjsgttj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gufeecfyj.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gwjbodzvm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gomsvzblf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gutzgdouo.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gbaoimydc.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gpcrzwnyz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gzlcwafjt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gomzdgfbe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gyqiymhou.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjmicmtua.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gliycfgak.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/grswjnmuo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/grymemtok.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gwemjosgz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gwovcokra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/ggpylmefb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gqflkvblm.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ggcbzrtga.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/grflqadon.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/grhrgsdqr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gbyxcyqtc.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gwxtlfbgh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/goksrinjz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gharjqidx.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gbxcdnddu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwptdyycv.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/grubjiacv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gbqnaqxkv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gkrfizlvw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gauoittkp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvzmfjxvs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gukgoccuh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gjashrogm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gqmmmstmp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gokzvzbek.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/glnescgnu.sHtML


<!-- 参考信息 -->