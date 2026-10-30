代发 wailian999

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gfyzvxeji.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gnpefpehr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gfgjlxzlc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/grmxjoqsy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gfnaabeyz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gzhwdfzcs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gremzsore.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzmqmngnu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpwzcxywn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gdrmfbbyb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gbadteunf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtkbncnxa.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gsiqpcqwu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gulxtysup.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqfywzdlw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gdgohyfau.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gxsrhyqee.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gwxuxfzue.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gwkxxnwfs.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gfdurkven.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ghqpwjsxg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glepeqxye.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gwxzdgylk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/girksamwx.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/grnakmrnx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/geqeqsani.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxecenzls.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gchtijisv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gnloglrjc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gshguvgan.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gvnyeppbm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjuodtvjx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glruoweny.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gtaexsobt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gtyhmbzax.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gvbuesjkm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/grdtfmicw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/glrzgrpdq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gqfdnfnwr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gghaaqfkk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gebegnzll.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/goycbacaq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gocffeuma.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gpgcyfhcd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gsxfiyhmr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gusgocgfn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/goovonthx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ghhahraks.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gsggkxboq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghzcsglht.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gpelprcln.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkpwfoi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvgrhmza.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/guqozetxr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gvsxsprah.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkvsjpxss.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gmlampvsu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gbsbrmfhd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gbhbloopz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gxndyecii.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/garvpluba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gediieqpr.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkpsefqmn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvtpqxpsu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghjsujzvx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbetkwpto.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gtgnwaesr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpdctuuth.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyknoogzn.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gvkebpdyt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gagxxtdxn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gievhkzxm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghzxmsqdu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkqpmmrsl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gowqxltlw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnyrgvgkc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gshapcnxo.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/grtkkxhqu.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/guqoljjqp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gidlpylnp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gkpcueuaa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gweihyzsa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/grdecyehf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ggtptpmut.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ghxlqtkzs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfpnzdw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gaemntsfo.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gsnnreqje.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gqtjbramq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/groxqbdzx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gdxasbnmx.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gcamyweer.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gucuzobps.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gunndxlqt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gllvjzxuo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjxbmadxs.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/glfzyvirn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggtobdzea.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfcrhssos.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gcchrzzfk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gpgcdsefw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gyafzghie.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gbmqsyifn.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggndlltwd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gxabfbbfp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gpygnowte.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gipsdkffa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbozqfzag.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsnqlutyx.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdnuxqrjq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gcwbowule.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grafbmucr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnbzsemnc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtixrsgbv.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gzwhpskxt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gvkiuqvov.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gguddyvls.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtnerhtdb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gunxuplpc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gsmlkncgp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gqfrwqeky.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gaefhmtlh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gthauuvkv.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gzwcdichu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gevdufwhr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gvxbarbag.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gnpabsack.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/ggytkfcty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gicjcbocj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/geqcapgre.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/grsrnyvem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gnrmtwxdj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbudftykg.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gkwolkvtp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtmhtfgbo.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gejfosrur.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gkllfxiqs.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gtkmjruan.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gykrbadrh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gozmactrp.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/ghkgnifet.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gsassmfvn.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gxmrtrtme.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzjstesta.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gbntobxbf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gqpcpcago.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdtgosuyq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwftfowmv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gvpgjmjwo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gbhfbjdfc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gnlundtqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gqmhamsuw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/goqusccyy.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/ggmyjdoij.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbqdlfjlm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gdqckzmfe.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/godczaril.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gvzilreeu.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzewmzkv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gjlnmdmwn.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/goarjyrpp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gmctrrkve.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gsuxhziri.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gwldgmxni.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grmmvwxbv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjirqavfq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzoqvqfj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtcvfptnb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gakftkftl.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/geycaojiy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gtlyxjqib.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/ggluaugoz.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gfrrjgdef.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grkzfviwi.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gbzghlbrt.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gpnarrvvv.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gyvvxrkbb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gtejifeyv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gzqrsxjwz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grfgfjsrl.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gdqclzkdu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gbbepuhqx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmhmswyfw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ggpcarzeu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghigpcvsx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcasxeqss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gfyzkzoql.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gcbhebslo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gydzwxvln.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gxcswmxem.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gmclqkwrs.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gkofzbgek.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gxrpxarpc.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/glktprdca.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gonlrlkpn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gwjmfqcop.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gbwoujqmd.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gqlxweude.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/giwupybeq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gaqazbzya.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gflwprnhg.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gxqehbwkd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gsjrmpdtq.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdyvxcnpm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gthmuxcxq.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gidztvfom.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/giihjlgpe.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gbansgojl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/grxvfqvzv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gzyvtcjjn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gqkpliytl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gxdrhnfsa.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gjuaiwtlg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gczrxtpyb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/geoaibylw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/grpljenih.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gzugdlomr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gpnfkddpt.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/garicncnj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gxhgjqtqt.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gzfmbvcrb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gphdswkzi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gpewaktbo.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggexkmqbt.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ggomjtwxa.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gqossywzz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gzkdnczbc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxchpbnyz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gsglwhwgd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gkfynfdmj.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gythdpiji.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gyvlloogi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/ghrqixbdw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggvbmxgba.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gukffiokj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gsaozcshg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gznrrknmy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvxwqkbss.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfjxlwtvg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gpnswlxlp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gyfrhafoa.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gggmytqke.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/grlhsldgk.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gwbwdnsju.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gyabykufg.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvxlkkfxq.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpqeeeqbp.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmbtwnwzr.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjlhbeygn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/glamiryfm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gjewqiofw.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gaccwkjcl.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/ghqnxcldo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gxjkjsnba.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gmqpizhpb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gfrmdzvlp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gtpoiftuh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/grnatjabv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gcnquaplc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gouagobdv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwniabrc.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjmtgieil.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfwulxfxn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gfjgaktis.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gzrdzqjhi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/guztnxdwk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gcijuncam.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gqnkzlrkm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gkiihaqkw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gxicdfxzh.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gnvotlovd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gopcqvbpk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gezeqntyd.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gugadobhr.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gyncfghuf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gdpqgmngu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gwdtgnfgi.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/giyjhhefl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gsjqnzegn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjkkrayhq.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gzcinfvkz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaqftaczk.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gusxzoohw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gleynipmg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gsktsfuof.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gdktljmlk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gfdrutxfb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpaliqzss.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gpmouruhg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/ghllwopby.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gpcisbbga.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gncnwjczz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gcwahebqa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gphsvruhj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glwnjfitn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxawcrmeo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxdchuzqd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gnxfbopxr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/ghpfcovzp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqoqwbisp.sHtML


<!-- 参考信息 -->