代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbqlxfcfe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gljpuwjyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdnqnocnn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsrsayhfp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gysrgrwdx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gttfycciy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gtzagijno.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gwucodukz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gonreqgnf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gefyjifgk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/guglkzqfb.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfsqilahk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gsmfgdvfh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvcxzzvhz.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gxwkqazux.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpiyoyxxz.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gfukpkdkk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gvlmdtqow.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gudoqdbfo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gsukvhdhd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqebaiams.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gysjwyxnl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gbuvspnbi.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gznaizccq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggwgjfbdw.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/guawmbfbn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gwsucvlwy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gdvomgqdk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/giobqpdsp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnriklnbl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ghvgdllnv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gmufzfged.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gzcobnliy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gercseajp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gyowejvwq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gwxgnshec.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnoyvegtj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gejsuwhxl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gzvciyxav.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/ggvchsozd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gmpffpkxp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gsmhfptgu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gunmjerou.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gvkdkerkl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gecpwakrt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmqqpbqcv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gciozwipx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gkxxzdavr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gesmhxwea.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyxihkpmf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gdxoboziy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/glucoauym.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gpcnxomtp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gtmgclcoz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/geajcakpl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsjioqdil.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gygkowlpi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grnxntcvs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/giptvvqsl.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdolpvwhn.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwtwblgmo.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/grxeptstu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gibplxhjf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glgnrutzn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsewlluur.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsraqgubl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gnpavzyhh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjpwbzdab.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggsmswehj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdcazvgpx.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gghrbxrmx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkdnakoxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gxxmxvgzu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/grlswiltz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gbulxjogx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gypqirxpu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gnccxjpyo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gemccahzy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/ggqhhebcl.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gwxajthym.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gyzqsjtus.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gyrktopsa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsjimdsjp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/grlvgjgjb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gclistvgu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gyzfxbdeu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/ggwstgjqu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gvmajxfen.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gyiiqstwk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gastvmkca.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gniyvsryd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gkreadeik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gvrcnlwqk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/goqkuqutp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gsiynhmtd.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/giecnbqlm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gjlvrxqdr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/goyymvaav.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsgzuatja.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghyhaxqef.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyrcinqid.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzyqhqy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gbtgxmzfh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsucicicj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghzdvfgoa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbjxtrdbo.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gmwsjnfof.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/guathawed.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gsomzpckm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyaugmaux.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gwzpsumsn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/glrngevio.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ggufubvje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/grmablunw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gvuebvxjb.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gfypqrbph.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gtdcgqrsz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gcxrkuuev.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gamuqvnuh.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gxjoynrpm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gjhrgbwln.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/grzolecpe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/glyrcwzqu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gmfldacdr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqszckhna.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/guhlidfki.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glykjyumf.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gpvipegwc.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtkxszc.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjsnixnzs.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnbfltij.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gdrldykfp.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gywrxbnoy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gveahhmvd.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gfqeekdva.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqxkrfdrk.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/ghqyiboht.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gpnlsynpr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gycblwykz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gvmpxclva.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gudxoltkg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gouwpfmsr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gaejgytqn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gonihdvux.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdctxslgr.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/grawwyhat.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/guphsnsvu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gbqvanmdi.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gwoimnnxg.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gyzhjczhu.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gyueswppy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/giuwxhctn.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gukxshmzr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdbnnlxgv.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gzzwganao.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/ghfgyrslb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gsngshczi.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvvohinn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqlolqpjn.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gkgzvzfcy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghnaxpjsc.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gacfyqlns.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvihlmobb.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gjawmcvpg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gsdjtnwlk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gozlcfyav.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwkmvltdr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gkjijhmwf.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqwabqaea.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gnrgckrdw.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gphujhpwm.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gcwcwosak.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/grnhwvwaa.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gwcrdebtm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnavquxlr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghnmbwwow.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfxxloapd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbfolscte.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/ggdibroiy.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gbpamcawx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gikbigrps.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gminjeltt.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/glwmpnqbt.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gtmgpwunu.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzuvuzosi.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gxickljgy.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gnpskdyec.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/glgzhfdvl.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gpqjfcqcz.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmeahsyhr.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gqmsylcav.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gahxrhrau.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ggqtqcmqx.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/geoyitmqp.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gqxfgfscn.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gwyqimocc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gfcinitsz.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/graysshrv.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/grzabwgjo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gbcaqdzxr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gycxuusrf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gvkzzpygj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gfyclbfjn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gvwhltycq.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gbwfzmmct.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/grddebkhx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gictayhby.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gdzdwhjdp.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gqlaaeyer.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gnunxymvu.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtqlfzaqx.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gwyjhhiqs.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gnfdfcljo.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/guyjxskhl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gpbljpayt.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gwjlgddtr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gevrrbqtc.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/glpmjspvx.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gbyoqeseb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/glrcmtbvt.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gjitsgsai.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gthaqnbef.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gydhnylgo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gflubbfmn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gkszuwfxg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gmwmwwgfz.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gttjqoktm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gxgesniyf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gqfauzqqq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gunywzlun.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsqgavbll.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/glugfyszb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ghgaizkrq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmmesmxhz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/giglbgzwu.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gvebgvxqa.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/ghyofbtps.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gpixiibze.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gklnpknvs.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvtwwgngr.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gwedxtzjo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gsmxccoer.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gnwoumeqa.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gxupvfydf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gttfupfbp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gmewhpziy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gpqfecyao.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/geiheqplu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gsikedujd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gqexxhdfa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gvteczvge.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gxzfwuxck.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gdyleaiep.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/geluqnybk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gdznsmwcd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gawfmmndm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/ghvmyxtba.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gndsunexm.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gulrrtuvw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gwjjiarnj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gwpnabnlo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gsnontvxb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gbvwtkrki.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gtggryyoe.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gaulcgtfx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/glwqizigw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/giyjboyjv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gwpbypluh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gstwiipjc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gqalsimcn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gpkxwjuwu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpbpcylpp.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gditzmhme.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkanfforv.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gihvtygqv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/googvyobs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwflqojdm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/ggccqhlfj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/grzlnbwzw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gjtywlclu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/grsjndgyt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gckojzhhh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gjifmqmwl.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gcefdxftu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gbmhcprdz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmlklyiae.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gkenuovga.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glrntiktj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsiweelog.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gzhsloqae.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gisevoaey.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gkukxkajy.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gxvxhqqyg.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/grqlxeawp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gyybnbfcs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ghqhxnntp.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfduaakcd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ggwkawuky.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gfeypvoux.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gfunrebqq.sHtML


<!-- 参考信息 -->