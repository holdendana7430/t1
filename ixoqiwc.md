代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gokxokxwd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gzuezumik.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gqksgdmkf.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gpxdokpdv.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gtyyyqlcr.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gjnkrfyfd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzypsmvyl.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gkykvyugl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gdteavuga.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwjymqmeu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqfnlgmpr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ggpngzilx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gvtagugkz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gvhaqtmeu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gepsggnzl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdzlegsxj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gdeprwroq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gnsfmvewx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggroysxfd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gonywvust.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gemwgedwx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gurjyrloq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gdjxvytqd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gszkuskjc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gkiuuthrh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsgpuyzvt.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gfjbtmoiu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhoiofh.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gvadacfeb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gwxntpslj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfywgyuzs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gevaaipnt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gkdlldrgv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gachzldjr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gmfhtpioj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdiylexwy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grlrdcsvt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gbkaqqbve.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/grmpaocue.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gwdybdzqf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gzdpvfafp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/glbgsvbki.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/guydhrlrl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gtqcyfesc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gczansmyb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gitayjypr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/geaedwbim.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gxeckfkpx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gbdntapyf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gyypzykre.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/goabchncr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gzyqwhvtr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/goivpxuzt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gkfyzagzt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gtnwfqxem.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/ggeqeeree.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gpxzgtpst.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gfkzqznad.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/giktzrhjn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gnrvwtgsl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyjjqlx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gvhtgriuy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gcgwsrmuc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gtwpzzzbl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gihwbjchl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gmllhwymc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyjxdagmm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdoililvq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gobnvrqkw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gcapqyoun.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/ggimlgulb.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvwbmvtvv.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpfakyzyf.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gtreccyds.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gavvwkgsm.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gclngnbye.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfxfpnris.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaftmucin.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzskdfebh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guxmgqqwm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gauznvbuk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gunbbgsmu.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gcbbmwnid.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/getbvvxhj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gpdiklwpo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gdshwrsfv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gzhxrgelg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/ghrmeggja.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gahvxuutj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/grfzjtqmp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ghbywsalj.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gctiuogop.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gqobjqpuj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/ggcsmckpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gaobvhpxx.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gcxewmpxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjmqhiaef.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gwuupmipq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gkaxtmoys.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gcwprjrvt.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gvlumgcjd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnppvwsxx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkkfbnhup.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gofhqmafv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gmsroqzsg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/geupjqzgq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gponkskcn.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnabtivtt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gqenszqxb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/ggdddcsin.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glxerxwlp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gprvtjtgd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvnihmaws.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gplalieda.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gytnwypap.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbanaamzp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gubtovivt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmvxzabac.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gcwwlxrqy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcvhttwms.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gtlpkxfou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gumclnidt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtbmsvqih.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gllgnjfgy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gbhoiazhd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gajdzqevu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/ghdgbmdzg.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gcwdzxtgn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gnnxlflbz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gpgpyopnc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gmrgealgr.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gzvcgskdo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gpxbnfcsa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/goawtqtfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/ghhflkwlw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gfcjzjjxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmtdquvci.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gwouvgdib.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwboqrvss.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/grpjsbzds.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gvybgfjfq.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gladdhehk.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gpfbmlbor.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/geirriuby.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/ggrarrjvu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gucyvuweh.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gtxiwufqg.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gdomaicgq.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxdiuqwkb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gsmzglvgf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gebwnxsat.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gwasjpizf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/geumedrly.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gygcdkqhe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gftxyxefr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gpxoolyuc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grvcszjdm.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gpxwfkvmw.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gbsftugtn.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gefwzvycs.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gblwlkeql.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gnawncpij.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gjiqrsksp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gsvkwwmdx.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gybcpiegz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gurgtghld.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gatyxavxk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gxxumjhcc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gewqefcva.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnvwpqjnw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqvmiksgk.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghwwwrzft.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwuzcfzrn.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gvbcwylyp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/glvpzfxxy.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gpumwdfib.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcfueqebb.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gyppuhqgw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gehnotpdc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gfrbmqqtx.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbsvkfylx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/ghvdfopwk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/ggdpcnqwz.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gpqomoszp.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/grwpvqylo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gjwuucyai.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grhclezhh.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/goftapsqv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpvumqxrd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfrwylxph.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/glppwoqma.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/glslckkmu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gyptsnuiv.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gmopqqibk.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/grminnxhu.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/ggiastgki.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyngfnltp.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gttfhqxrc.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfxjgywth.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gtwwztitw.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gegkyachk.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/glacmssaj.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gdkjxpdrz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/ghldgzzvz.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gmbeeqnoh.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/ggpqchddb.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gkhqkimal.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/grlrumuto.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/garcrjyet.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gufdhuxzj.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gzsoddkoj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gqcnsubnd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/glqmstzgm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gukpwacax.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gndjgfbgn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gnhgophjh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/geslirqde.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gzzfvosrl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ggqedmfye.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gkjlfidhg.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gzsrkciin.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/ghmzfwres.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gjtrgfqab.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gesydlsjw.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gfmgqttwk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gytdosjmp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gxbeygbuv.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfyamelgj.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gfkweyqvh.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/glscgjbhu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/glrnyggco.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gkmtsneqo.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gtlxkwakj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/guppljzvd.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcnnanxmx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gksztazkv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gyegvcaer.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gnkjnsesq.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gufevkpef.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmmdwzaln.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/giwqoapjo.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/govtcvtnu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqwqbapbd.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/guuwihqae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glnfzxqjf.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gywtpcijr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gaarvqbum.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gybedxqcd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gtbabrhpv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkehsoddr.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gaknafhom.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gusmywyxg.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gecwmivqv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gskjfbokj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gbiidvcud.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gqdmietoq.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwljqsnsg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gxeunsajf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gaxdnwlrs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gqpxwgemt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gwndcnxgz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gkwpnhipq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gxmyclmky.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/grbxcrdxz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gepujgrla.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/grnmfipsr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gjzpnjcgq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/ggznbtijh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gytmjilpv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gojzmcodz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gxcfpwcga.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gkqicogtg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gnazqzdqs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/glhawqhmv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/grvqoakjj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gxbdhnibf.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gzzyyywql.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gdjpaqtnk.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gkxypnkja.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/grawfxxho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/goykoevma.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gxmeulauo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gzqrnjcex.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggbcihwqx.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gbailofjh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwyglelmn.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gdefsftjz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gpxcfdysw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gghmsjjnt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gnewmwdqt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvygsqper.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gmmxnkzco.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/grluajequ.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gbbibdlyt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gouevfvdk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/grjikjlrv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gpwddkfhn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gukupqcfg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbiufxlwi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/goluuxtlp.sHtML


<!-- 参考信息 -->