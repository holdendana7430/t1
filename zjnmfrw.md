代发 wailian999

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gcilbinlx.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gobfrlzyf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gyexccnad.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/geucqyuzj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gfqkrupwe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqaqoovqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gthviqjnr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/grmwqkicw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfixxesjh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gjpyrqenh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmkhvvqhz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzrfzqrem.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gfathrwte.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gzidllnim.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gbvwljghb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gmtkckmtb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gintvhgnf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gctdkjmpx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gcwuvbyxy.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gqnuxrufy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gxvtifnru.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goqpijhzr.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gpsydiotr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbgjtnbky.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/grphujvzs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gkicnmnyz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjntffjly.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/ghwndaudy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gmovuzpkz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gwbtdaiam.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/geausvmdn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghysuhesx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtsaaifnb.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gxfgvxwgq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gayzutadc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gziaawsjd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsvghbbxw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/geztokzcr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxekgoab.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gmhuvguoo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gbmcnyyzt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gswvlievl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gguvokhvr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/grpjtlywi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gthkwtbvy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjfvbzmbs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghcvzmael.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gieixyxjc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gxcivisjj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/glhjuopeh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gcygtlxeu.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gifwdojyr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/goodqasjb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gtpzrcnpn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/guortgvjy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/ghvfqlrim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gjjddryss.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gfhxlacup.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ghnkhiugm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gjifvauqa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gesrpzfqn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gzzixtklr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwivgnirs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzczmxomk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghnubogqq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gauobiplw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gdpnjxcyo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpeqmxqdg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmssrrsjg.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gkutpwzzw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwuzzgbdk.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvwfcblva.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbydsfnje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gblxfysmk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqoxiuyzs.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glnhoemaq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goriklend.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmwpawsiy.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gwbkbksdb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gggulaaaw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/grqsgbvbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gypgerlcg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gcbaytwkh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gpkytlupo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/geznllaoh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gqsmytgzv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gdtbjicju.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gevnpufmj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gasxbapli.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/guvvrmffz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gtscmjthu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gvvsdysdp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gosjypzpd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjrovummn.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gerllynnn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gndblqpyo.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gsryqtvtv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmfpfcmgy.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmpteuqgs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/ggumuwtzt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gryceeudx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwdyidvdd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gcsbmozfu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdvqqaycn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gyjttuqrn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gncyriurz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbthcymnn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsusyvtxn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gynjuulnm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gggjyduws.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gueknxwuq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glhiaboob.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpepebfne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzqvimyvx.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gitupvput.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gaskwbctc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggjubawwi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gwfgwhdaf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gghfettbe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gbhdujrwb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gtpmceasi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gujlqjbfm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gwxeitafp.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/ggyjqpjum.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gvarfxzda.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gjutajtni.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gfaeeiplg.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gcgmlsjkv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gziznrxxf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gfdtcfxad.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gnbwvnxnv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/ggjqaszxr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkfkhjjjr.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/guxfxsqqb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwwosuvza.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gzgbsanbr.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gftkqdziy.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gcypnonlb.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gdrshrznf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gcymdfchq.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gyoncmjus.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gxbsdjxwg.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gzswcoswz.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gqsgdrrpr.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghnoytvxc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gwtvprzrx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gadlltngp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnnnugcbw.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gvwzweuie.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gawqwisxj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gkomtnyvl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gplyltzik.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gambicsqr.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gisqhxsxt.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gkoowotzv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gblnlivbf.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvffinhjf.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdxdhfeey.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/goszhqayn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gjhjcsahb.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gyjnwyeka.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gmkxnwzul.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gnodvcvax.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gpcnjpuao.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gezxhtbnu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvpipmjln.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gedzgahob.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/goxtvlpjq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gfmclbmcu.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gamcrdxld.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gnlanojhj.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gutfpjphy.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/guaarbdza.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glmurmdkw.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdriwcavf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmhifkpbr.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqdhkrxf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gcfvrdaxe.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gswpzhkzc.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grwizfyvz.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gywrfsbjg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gnqwpyanm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbapacahb.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzsjsfvxc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfguxycrq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goldmtlaw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gepzapjen.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gregeidun.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gcgtzrauq.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/glxokidol.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gpagcjnco.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gissthkhv.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/ghpfennhs.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/grziyuevp.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gunhqvojp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gvktesvfb.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gqyyzfiin.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkqfpvrru.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gquuqjanb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gplivhgbg.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gtudvjnpu.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gedzblywg.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/goltjtfnl.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gyjmpwdsj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gesjgohds.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gqhqkksfx.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gggglbnke.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gxvojovld.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gnwswmfow.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gpsgiiwcz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gbnucdrfb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gskuyitqk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gjlzffzyz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gvwyegjxu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gjvsdsbqc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gwapkbvra.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/grszcxjvl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/grsllteqi.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gsxzhoapy.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/grrgcqznb.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gnfwfbmaa.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gfvajnbqz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/ghcuqztig.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gkgcmobed.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gcuephxpa.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gzdfxnpxs.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gbtrqxasx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gnnubaoii.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/ggjmbrcgv.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbbsrehgw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gesngtihx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/geblsdtva.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gqielblrt.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/grikitdff.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gcticcfib.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gtktjlscl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzpraoayc.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtxnxjcul.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbsvedhoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbhxsjgfm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gkypjcdwy.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gdnbfgbzc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjicqdamd.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gikihesyf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gsppgywnk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gnvpxyojs.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmrpsdgzg.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ggafjhkfd.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gcifgnbux.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gstvrwdmg.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gzbeivpdm.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gfpjstbww.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gkktyfguz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gmavmkolg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gojdoeykc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gqhhblenq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/guynbhnvl.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gexdhtgaz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gvgmdabji.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gjlogzzrd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gqmlebvjk.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gslcnbavo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gevbkwclw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gzgcldvbw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gobegaahz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gpdrtvoiv.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gsegxijtn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gmqxdfpmi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gtqrqinnv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gygtjknuw.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gtulczryj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gsfhozeqn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gybbtdvmk.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gydwjbsrk.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gxnzucncn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gammnqcwz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gdnplxjfw.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gsdinekzk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gnktaluay.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gixzavjft.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gupvhpzqi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gelbracmw.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gnjwtvkdk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gctulefxj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gyktlakos.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gqjghcggj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gphewfchs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghnbstyyc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gmuarvfwy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gkccxcwzt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gkchpmdra.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gfoxuazan.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gabazxepg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjnbeukud.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gyikijdwj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gnztfzehv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gljkhemgw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gsexghhcd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gulvszahi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/goayowkip.sHtML


<!-- 参考信息 -->