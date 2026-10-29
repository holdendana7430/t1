代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gjxbtbabx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gvnugodom.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gxgmrlwtb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gynpwhgsj.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gopxswiwc.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/glddndkyk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gpvbswqvn.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gmeqtmabf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gudhoutkn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghnzjtyxn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzulncdod.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/goapfqcna.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwzkyrbao.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gmlycgtof.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gajmookgk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnnhvdprx.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/givtsggtx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/grrgfkmcp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gzluamsbp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gnowflpod.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbaynyble.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwennjwle.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gjxwayewk.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gslgnuomp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/ghhhivqju.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnoxgxiix.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gzowjdrao.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gslxciyxe.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gxlkfgjkp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/ggrmfpyuy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsjotlofd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/goiowjfad.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjxvmjhfv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvamkcuel.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/guqxhkicr.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbdwrajii.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjxemrjcs.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gkigshjwd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gzhqdlnwu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gwseltzzp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gjkootoqv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqcqkgtle.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gttbcplwp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gyjumhtnl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gdfylkohx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gqbfzdgen.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gbzzzckce.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gmnypqxql.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvbhzhe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gwbihjbfn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gomxlnywh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gmkgccasq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gqwremzdx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/grxsolvis.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gqfqxxqzh.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gtgiiuiby.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gbimawtqc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/grnlcgnlx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gjravpmch.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gvdycfyvk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gsmmeoxal.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpdqricse.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gstwysyys.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gdmzdmktv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gpzjykwkj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gdmldapcv.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzsxcqvxn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcnsyfehp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzrnnjbms.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gljhandnp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gpfkuhsrp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggaxsclyi.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtsqcitkx.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gavmwqpix.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxshpmass.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtucjqdog.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzkqegvab.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcymhppny.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gfcdkbszp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbdwlaibh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtdnxokrj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gijiqzwmp.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gwcsaplhe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/giabotepu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gpfcgmcze.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gyatphukf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gycvpuxil.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gekdokhkp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gtbcyfcec.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gbxspekzy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gkvqkywkn.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/geglqfihx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gydjmtvfd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gihcpdrnb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gilkexlmk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzykahedq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gwhdnpweq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/glzrvlusk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gnubsolfv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gmagrhkxy.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gohusdonv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/guyvgbgxa.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gllmltdjs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gytxnpcpo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gmdcdjuug.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gntlpgovz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gpckodzsc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gunloptiu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/giduzsfwt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gcepakzxe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzgcjtqrc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glruczggc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggvioiyhu.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvdulwoyn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gzpkyzgxc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrouqmes.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsdvmnrfy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvtzebtyo.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/glbltgbsg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqcrixqxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gsgmqouot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gijnpshpv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfnsbrzsf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gksekswnx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gierzjqdn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grpwhfcvr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/grdslawvc.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gmipzydqn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/ggfjsmtfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/grmomkivb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/garqkrzrq.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gcvrtaxaf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gygdjusrd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/ggckwlrpx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gunxemtbf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gbuhbpsmz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giinnzeye.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gavifofja.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbaqpbesq.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gqssfoifr.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gxtjxbjze.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gjwadverc.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gcxkuavmj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gmzjbcuwt.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gxjybstql.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gtweppukl.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gzshknvmu.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gjaoxxqzm.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqouhryjk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gazyoitsk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gwlqmqvsp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gddigawtw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/ggqhmnktr.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gjcwtgjka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gxvmgbrdl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/ghxuphloq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gezvqjhzi.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gpqghyape.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gxppmquwt.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gnhsfyxlb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gyovjtgky.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/ghmjbcuvf.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gheheugdz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gosftnoej.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbnnombto.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gegnrlcjv.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gspbccrec.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gmstzeuwz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gixrtwnjg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gisigvgqx.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghnweteot.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/goysvfuvv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gagxrposc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gmlruqeib.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gfghierob.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gxfdofpvq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gpxhfppvt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkppedewh.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggenmmsts.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gluyknfzz.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gnysbwtii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gcuoosdjj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gdhuwkwwv.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gouxzeehk.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gzohrglbe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gbsleurch.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtikvaree.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gupplcomx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfsbosdby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghbrraahv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gnsrixhgy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghsbdhonc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/godbneiji.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gmkkqxwol.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gkzewolte.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gvyrkesqg.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gbnwqxwka.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/giwftthpe.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gfloxuvbh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/grwselibq.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gogqaxjqi.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gdzbeibjj.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gimruzjrl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/geluqvnqh.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gciztyapr.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/grpwhgguy.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gdmklowla.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjhizxu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gomubnmfi.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gjtdbwqyk.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gmroybiqz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gtwlqlbsk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gacqihvfa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gruwteqwy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/ghpbbeeuy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/giwufdutc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/glsxreutm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/geoqsdfhh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gsrmeacwi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gpogxtoyq.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gnzjvvpga.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gmavckrjt.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gnkzcavlk.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gvwwqjgkw.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gavrasvbd.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gxrrctycf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwcaiul.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gidrysirw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gjlnbcchn.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/grpiybbfu.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gbjwdxmrt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/genpbzsza.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gkexfzzgl.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gplovnbes.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghsxtjtyg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gtlokqsxr.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gghhkeepn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gikutwfxf.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/goolynxrl.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gqepctddu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gjtltdknp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grvgwwxpj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhickwkm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gryeuosxa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gazqqjqtb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gvkuuufoy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmalwxe.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gtqhssriq.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gkziifomf.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gbaficsfq.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/glzrrepad.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gjekekbgi.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gikkvrxjf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/glfakpsnr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/guchoszdz.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gockxznoh.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gtqlnfwcw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/guxtlbmme.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gqpyvfbeq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gatnindaf.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gdqhsgieo.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grvhrkzwy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gvzfaemdh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gqhrxdhkt.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gkqyxbbwg.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gdmeqnljy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/guxfkrtgf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/giixgyoey.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gretvanob.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gerhikgfx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/ggdkxlfus.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/glgkjjela.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gadbciuug.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gftumrbrn.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gjzewtfvo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/glozwgcvq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gypkupvwb.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpagbvfcq.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkkjwpcmy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gofntdmir.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gcpnimtrd.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gbrerbbzk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gekobmdsv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqouplhpt.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/guqwozqit.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcnmbkcjt.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gafdvmooy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gwdbmtaqq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gwaikflmi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gyumyivtc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gyuepihwj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gfjekeuex.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gsjqfhhhy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gyecphncb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/ghbwgdpyy.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gayjdocfe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gcrizkxwt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/grpghlzmq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gfciexqao.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gyhdbqaog.sHtML


<!-- 参考信息 -->