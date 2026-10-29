代发 wailian999

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gzgevoiwj.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gcnbohnmm.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gxdoahekg.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gznqkuvlr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/ggojhxuqo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwmeebsfx.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gdwphrdne.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gxzfujcoh.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gzkrrdjru.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gcgcsmnzm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gcptzilco.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gehefgjvf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gtonjgazm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gdawwmkxg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkgvhfljn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ggumxvbhl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/geoomllwp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/ghmuuzwmp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/grmhzmfkf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/geitruckh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gijbnieiq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/glgudrfhy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gdlbqrtgg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjhihooav.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvzyjzkms.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/ghmlpiyfg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gevwhycbd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gdcyhubga.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gfchuqmpz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwknghmwe.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/ggmkeiojd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtwpolttm.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gtwcmgjtd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gaklsqbxw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/giuzcrwoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gqzvoeaex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gebmtqqrf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gbldwruto.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/giqellrpt.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvvamgovo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqjfoqqqb.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gdaufztsg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gepjsnstp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gnjfdiqde.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gpljyfmbr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gvvxovkmf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gksandczq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/ggrxyioss.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gddtezdbn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/giuoigtqz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gkfmbikzb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/glishozqc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gvfsmpafd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/goascbyii.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gcemapjrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gjsekohtp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/ghlgilbsz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gthgbgpwv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gicgvcgtx.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gdewtvplb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gmfwafagh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gdfkcdxqz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gjjmkbcsd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gcekumdui.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gvituzjdw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gtgilldhf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/ghxntkpdt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gudvcmcds.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/giwojvzvo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gvgldlmyp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxhwiviwu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghgzcoryp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkamhuuvv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnklxckgl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gxbvbnaxx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkkobijdx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glfjsmsjd.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gwwjqbavj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdboutrgz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqceiolpq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghfyiobho.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfsomhmue.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gdaitrvbv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guzzhzmxm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/glrwudevs.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gcaffftsr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gvbcatjih.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gjxgxadcl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gmhqmqxag.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gctshmzxo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gnujyjuyl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gboakhnej.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/giyeqmxlx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gczhpdeug.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gomkmpujx.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gfemqftah.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gqrjdveap.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gliotfotd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzhsoxzoa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gsnrtaclo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqktnoohm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gzwiolbqi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gtknycdiw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/grdhhwdvj.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gzbhbgmnd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsuwqyvko.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmcuvlmep.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gieeltvzz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbltcbnxv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkcmtdewm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gljkljlqi.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjtdrwicp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gelmujwwj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gaxupslom.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggxtmfnbz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gwkhumbbg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwuyeqtbm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guppedqnv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gdobjufst.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gfxdmqbnb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geekayaii.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkadylrlv.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/ggmdcxpmw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gzavrekoh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gbgodhagt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmlnjhchb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggwxnyvsl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gyfmtohto.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gqmriumgp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwaatcebu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gxylipgog.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/glrnukbte.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdzotbz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gpoxjgaei.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gsieymdma.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gxfwzfbdq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/ghhrugyyl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gbqkcnagq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gwtincxjy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gfwwkptna.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghomvopxm.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/ghwkvnpxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbpspfzvo.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gnxcxajul.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gnovzgvjr.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ggoqvhiwj.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gkzogtiza.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/glhzwyjqt.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/ganptdupv.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gbljnvgbh.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gtynuqndq.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ghpelsmyz.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gzoltoanr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gwnjlrjls.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gvuixurof.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gremrrhpd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gvtvamlhs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ggyldgonh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gtmkzwvsk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gdqwwoplv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gavytntih.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gfyqitsjf.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/ggrzkzhtk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpvodpyaq.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gqdpxezbp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gecygcdce.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gzprrndyy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gwcgylkbh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gblokcduz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/glyvnjegp.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gtoagkrpt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gxouknveu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/guhzhfexz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gikorlvci.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grxthruqx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glttdhrtw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqpcwcqrl.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/geudwymzk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gbevdcexk.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gfyprpufe.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gsuzrkyzf.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/glbameayn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsmqcdetu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsepctial.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmzhzakxx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gzrfaowqw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gmtxgptba.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcydypywm.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gikrvimak.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/glbnjualv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvipqatvy.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grajwzjrt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzpwgcofo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpqwqcrro.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gwkgsggfk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gutajexlj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/godyszjtj.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gbamdgtil.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/ghinpsnhm.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gevraksvb.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gohwwpcqu.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gldhuwcmx.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gtyxhxrbl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/ggzongbyv.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gvzlrltsi.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gtzeozyyq.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gqiogpqnp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gvylwzuyh.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/ghcczhmsv.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gzaoulbtk.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gakkwvkpo.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gapuguteo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gficwlfmw.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gezjfpovh.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/glusesixz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/goiugthyt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gaqwsghgh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/goldwhkeh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/getknqjme.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gspagpwaj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gnhjicczy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gdzpblxge.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gmxjgybmz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/ghqsxwulu.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gyxdlzwdy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gqvjjoybk.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gmdonzynw.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/giqnwnggp.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gejcpzien.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gixjlpuws.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gqavbddzy.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqvpceury.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gfngoikqs.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/grarjqeex.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/ggmulebbz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfiiwmqfb.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gmrttvvmt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gxxfeionk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gbtzrmaqn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbpmbiwze.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gtyjwifgs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gwgjsduln.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/guyvdjcpj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gdlhexeik.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdizcgjxp.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gchxbfqws.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grrgqotcb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/glatrakgt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsviwckxz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gnxauapun.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gxsslqfej.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gcfiqhakt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnmmatfv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbhveznbd.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpzfnsdqa.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gzaucwquu.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/govbfnddw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gwtmofkyt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gmpirtbgf.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gcmyleleh.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gyhwoiins.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gkurjlool.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/ghcggbrxs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gexwmfuss.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gdwlxjdyz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/grspvkwtd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/ggqrpnixz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gciexjflt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gxamqicdw.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/grlbrkfkq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gvgeqvxft.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/ginxrevxp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gblptjdpm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gpwbeabjx.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gzzbhvhjw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/geujnayri.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gwjpratnj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbxpgdpcb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/ggaiooxjy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/glakxrvjq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gmhmxndwq.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gxuwmkocq.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gmpgubexg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/ggwnlmvbt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gylllkgex.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/ggzoopjbj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gcgaoqfbr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gisoowenr.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/ghauhozlh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfkfdqeob.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gibrvbcqi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/ginfhvdqh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gdatsqhxx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gkbuvsnvz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvjyftkaj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/geoudkewv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gpqorjlne.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gnjpziksw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gyqoxqojs.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gkrazjeev.sHtML


<!-- 参考信息 -->