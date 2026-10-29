代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gmnehhicm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gblxrpenq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glbflbqqo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/ghunqkfzx.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gtrxbyqrn.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gvnywfkzi.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gqpivkbqi.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gxwijhygh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gcrkhucsw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gummjyqjd.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gfxyaonbo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gxnwyziva.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gwqscleqi.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gygmodahg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gkuizwjph.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gkjkkmbrz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gmzzckmjw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjnpqjpjg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbkryxmsl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gwsjxoxrf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gxoqyihuc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gkfromamj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gpaygsvnm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gcxenzpnc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gawboavae.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gqivfjqli.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gywjkwqih.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/geqbyatmk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gwnezujjo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gdeecdxrg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/giwegrwtg.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/glbidisxk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjcvdcpyp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbmyzrnpa.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gwhemnryl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtkxxdict.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gjmrfkrhv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/ghshsofyz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbfkbsger.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gcommafzs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/geurntxrv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqmvecisj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ggcvaqmrp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjhptdozh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcyrlfokz.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gfntatvhq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gjstosndk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/ggootwhek.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gtbxilzsp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gblgnktkq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gbnfbgtir.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gwtbmlfft.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gdiywqjxk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/giiqpbwwd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gftghpuzk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gjqxvcscj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gwbmpcpjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gmnujlaas.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gznkwtmye.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gfpsuxtpg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gdccsxqcv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gcuaofhes.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gdizgghbn.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gjjcqlktg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzappklcx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gwfbmffzt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gmoivuswi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gehuuwcmq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/guwnqizlg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gbmbynmfx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gpvmjlqvn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/glouvjgtm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/grbwxblgl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gpmcdokso.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxpkuiosw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwmlqvwdl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxxrzhvyn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkwuiiknc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gxdbmftpg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gamsehgef.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcwfaixww.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/guempjzgp.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbnwyrsjj.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpcmuvqzq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgvedjl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghhabqsmf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyyyphetl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqlgbtkbs.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gochpuurq.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbenoiixn.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gayljvozj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gocigkdbz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gjcbjdwel.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghqpfpxgg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gxswdqkaq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gznljqqkl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gekxpwklk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/giaenlvfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gmmbmhsat.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gafnbahny.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsspwbynk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gwxtpvfkd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqcocfljp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmwcfgecz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gkoichikd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gcehprppy.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/grlescltn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gaoyduapp.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gxnhyrqjc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glrocidlv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/goyysenun.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glflnvjli.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcbzlzwgz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gnbvuxttt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gnmtyxtky.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnxwthyzy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/grpgdlmnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gijikcmem.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkdsngcrd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkhwsoctc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyfomtiqn.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghzzangqx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gtzzdyngn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqnanfulv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjzyfbcfb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtsebxigp.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/giktwedga.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghgpwrkhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpyxkiwrn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gytuuyhij.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnnvrndpu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gekjgcoti.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gaauumgmk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtjwhfgfz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/grhzaoses.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gbyftzrbg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gcgorjrhs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/getzvhrup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gxrdasvgn.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gmkexgugp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gzwsdkhmb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gmpocxhlc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gdpnahiif.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gnebwpulz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ganexmffc.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gyvcxtnhs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvvjtrxij.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gtppuobpk.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gikomyjzm.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxopwdvpl.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/glucyywyg.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gpclaudwk.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gexbpochi.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gkrnqobay.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gnzhriveo.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ghpcvslim.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gyuakrifu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gsgbefsiu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gcxpxajvo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ghdunmsmq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gmnuqqawe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqrmnvuwt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gxtnxgvmg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsznphxvl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gtrkvqhpp.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gohvmoitw.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gzshfrufn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glnftektv.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/guojcnohr.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gbmcpydbm.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gtuvcebxz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gzvibezgb.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gnerwhrwb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gwhtxunpt.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gpdfiupyz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gnpmjvxwt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gzqurzqwz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gubwnrhba.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcjcfmree.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gukamjfvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gyuzlkswm.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gfekacrgq.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ggbnujubc.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gahrhilwx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gcdpxnwkx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmvbyfovh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzozrfjmb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmfksovtq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnwsxaaex.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gwwidscej.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/ggdzewjzs.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gtbgjybkj.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gouxozvjl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/guzgvhwby.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghzgcqoct.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grxqobauc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmqopoxvk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gomrbyqzg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gcjykngli.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gpdcvcqdt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/groovbtrb.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gyraozjgx.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gxvrlqehe.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gioykpkiz.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gaxdvbmze.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtwbxeqin.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gciwmsyyx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gmkxcmnan.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/grzurbkys.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gsrfekumh.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gvhmeqqqd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gzestxsyd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzajuheae.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gxybqyzrb.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gqdxhuddj.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gyzbevucz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gxbouyanv.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/giquwufwo.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gfwwmgsbq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/ghnxhkejy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gdphgwadl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gzjnlojlm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gtacbjuyt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gyedkpxhu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/geggwigqv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/geutifies.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gbxiwhoww.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gldmzulif.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gmeteclfs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gqmmcvyyc.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gyugekogh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gmugevzpc.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/guagtrwqq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gvzrpocix.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/giuvytwvp.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvhylktxh.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gjeslpszw.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gkmaaglco.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/goywzkkex.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gwghjkddh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gggeemyht.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gamfvbwzf.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gkltaqgiu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/grbrkswoe.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/glwaeqcuo.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gdmrlaxxt.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/glihiqfwf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gcdvdopvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/greghwtvz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gzynveonb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtffkifbi.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gadaimaku.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcifqczeb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gxgqszadq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gsteugirt.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/ghbenlhns.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gvzoawncp.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmnnlpntu.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsgdumuej.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/garghbsfg.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjtrfloia.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/grzeiwkpe.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gvngkwikf.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gskvjkjtg.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/geqajgsnu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gkxwgavdl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gfxlakksf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gkeqgtcla.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gdjfhbtwj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gfxdgdkaa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/grtovcuon.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gkwvsliks.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gybuimedi.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gerraatym.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gcqhtoawq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gestxuubu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gxfkjgldr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxgupob.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtdyklz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gzahhdyjl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gxgoylmzr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gaoopotct.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gqqoxwzzq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/ganpluing.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/ghgeeqeqj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gseiwflod.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gfwodrngq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gzhvwqdqm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gtbgksabq.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gowyybsez.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gurogimsb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxftzvkmp.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gdyofbjwm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdaxyglob.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/grqdmtulj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gnedvoulq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/glzlrwcel.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gtrenmopp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gufnglpmf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gcixunlnv.sHtML


<!-- 参考信息 -->