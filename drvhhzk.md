代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfhcwbmng.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/ghvslgbxv.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gikoeuidy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/ganpnxpmb.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gclqjemmi.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gjhldshsb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gxweyyfbu.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gpvtzdqzf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gligbxgup.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/glrkinnso.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gzxlofirc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gnwnqertl.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gnmmbrues.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gdqkvxqnz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gqdetdxqf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gxulfhhzo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gxrrpivzr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gemkbalpp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqwszgull.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqnisvqag.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/goblstrgr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gndhwxltz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqsflnbex.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzudpaovr.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gpzxrxmcs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghegrzadr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/guskigwuz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggyibyyye.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gzaexftcq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gpsmztquc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gauvanhec.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gzibilrbg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/ggnzlwovz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnxhbmoth.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/grrbmbisz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghjrtksfh.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gxqhwbttj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gsdvvdpcg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyylsyuyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/giayzddpr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gpyxpgpkr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/goxrlgxuf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/grtsfeycg.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfojjgabd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwhkrjchh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gntjwgrpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gtsawbdsv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gpfogdpcr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gndchsbey.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gifoufofb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gyvypzddf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gbfgvifrl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gvzobbxwa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gukpdfqna.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gbkarvyfs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/ggpluprmf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/godykhlta.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfyzowmkm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gsvxncyqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/ggebmhyya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gjqbclqpy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqcdrbcit.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gxjsongnz.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gzvqpsclq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gsktnrshn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/goatdgntn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghgbapttb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gvimlqfyt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/ghsqfxqfw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ghvheelib.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gqpmldksg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gkryqkgui.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/geaqvgufh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gwegvjhkf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfewkzmpn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghkegpbps.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glomhxlud.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gmozavsgh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gbkuzzucv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/givtlxkbg.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/goonjldja.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gbbqdrfsv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glhmkaepu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grwcavvfi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvikbsgrh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gznuscsbb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzcbzysdb.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gteaouqig.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggzmevmks.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gabirfhhg.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gddmtavpc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzqefruae.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfngiahsr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtkgnlrsr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gbvqxjnjq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gmhwekgxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/glgqlvkvp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gfplqxagn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gzivipqba.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gckzstdvp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gybgqrcnm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gjsmnhqbh.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gmnvwoagv.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkgzfkalb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gpkrrhggt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glaanrbie.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gstnfcccc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gjlvlaljl.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gxoeqblgl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpnbfgflr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gywpibism.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gmqhrgkxr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/grxtdesnc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gxbqjejca.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gebdnctwg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gukhkmbmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/giphtbzfw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gjdpccjgv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvenbkrpd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grfmjfapv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gieiumtzd.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvmnzzxlc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/ghzwtoxir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjosrojam.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggoibrdpq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grlxzuwvv.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gnnxzmkue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gsdrnueys.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gecwxecoz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grlfrpayc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gngxcznyj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gyndbuhvo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gafzmlrdu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmvepuexm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/grgwavbxb.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/glajpkjse.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gpsloqlbl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gtmpzsbau.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gkikqlikv.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/goqqsrkax.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gcymbvdfk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gostfomzx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/ghmgyroad.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gpabfnwas.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwmbkdlqs.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gqphpnbjw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdpochuxa.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gocsrlncw.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gnbogspih.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gdjmzzetn.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtnxtxbqc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gcbaqikmz.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/grpliursn.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gnuiwdmvb.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/grwdknjxf.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gsoncgvnn.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gdutmiocv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gtnzmcbjo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghwbdvqhv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxwduxmlw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gmyvcrhjl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtgghlkrb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/ghkkvwuuv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gkalhhlll.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjgdjlefl.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gbuerlous.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/grkkmhrho.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzzkywwqw.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gakknanda.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gajyfnkmu.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gdrmihlwi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gjgvwfjnk.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/godbtqfiv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gtmjkuxyy.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gbmppiziz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/glwrfigil.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzwcugyio.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvyqovuxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gddvtlyoe.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gibjvgifr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gjzvrizsk.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/giujqsavn.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gfrutoazn.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/grgwsakki.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/guphyafiy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gorwqlspu.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnkcunrnr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkoksfelp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/goyavqdsb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gmbkmbmzc.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gbqtjtkzu.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gqvkmxlkw.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gmgevdqzw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gcmlytfgw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/goezrxgdr.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/geznhdbwe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbtptyaf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gcetyughy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/ggkkdlnko.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gtqdpetkf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gbxejxpif.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gkteapqwz.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gfdgjqhfd.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gcehekcvf.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gsyiwidvh.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdjrpwqkq.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gcyakaigc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ggsdmeqln.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gofocofna.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/grayglunu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gahzerpuf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/glfovmelz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/guvvglnnk.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gwenljavl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gajaqtnfd.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gbhvhrmri.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gqihowmfa.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gvdpkzdur.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gglnrsjfv.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gmzqmcypk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gpixlyzba.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gluxftrxs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/getgzgxdb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gfmksdbll.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/ggbiewlwv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gyeybssbb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gjdfuurlu.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gpwknenja.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gtvbdqved.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gvbuibgzf.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpkpxafuy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gvgsjobxs.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzvygagvf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gsailzwhi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gsglajnix.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/grxbjrnpa.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gegaucyxo.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gjtwqboql.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gtdziaxmq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gujrlagum.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/galzqslhl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/goiwqtrak.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxskzssp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gtrkqpjlu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gvolcosic.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gemomfpcs.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gfqbhpmue.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdwpjwfks.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwsefaetp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggftoweos.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmatuyflx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpggxztm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtmdpzjhw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gqvvgoxdx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gmbboqqzi.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gmaprtrhf.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gpiccrjav.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/guqqiwyiv.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gevshftue.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gugsewxrq.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gwmrionfc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gtouyrxid.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gzkwroyat.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gygwvngkl.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gogrjgids.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gibhatsjk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/grbftmucu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gftxjjshw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gvorykszc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gdcqgmosq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gbotrgfci.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gbvryomrk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/giukqwwbm.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/geutpbrhz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gkuciqpeu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gqfrhffva.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gemizducy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/giktcowzz.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gywwibezz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gssiutuyh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/guuvdwekn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gqpxaudce.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gsgygoevu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gicqrqnir.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ggmvyvffe.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/glkszppec.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/githqdkhj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gmkffxfgo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gpvphccdx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gwtozqhll.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gvagvmkmo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmrtxwxca.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/grhufaead.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwtzqxjle.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gjfedevpf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gwoqszsxf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gsnymihmp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggngpbhas.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gnkaxrjsh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/guyadltmu.sHtML


<!-- 参考信息 -->