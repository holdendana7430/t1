代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gnnuamreo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gmqfthznl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gatlelruq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmcmmmilc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gzbnzcsxe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gfeqvlvam.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsxtxsgyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gplixrftu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/grnzjdhyf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ghbvwksod.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/ghqfwyzjl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gzjipsxcl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsmkhywiu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gymofaskz.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/guzrgrged.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giyazthmq.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gzzlzkktp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gpzrottvq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtckajlkf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gznydthfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gzcmquoye.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gpsassuen.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gyqvwionw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/grhantdds.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxrrqusiz.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gfmcevhfi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqrdupj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gbwqccflo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/glydvaarf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/guwtjnftk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gratpfgor.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gxcdvmmrc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwlipxr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gywdtdqes.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwybhzjir.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gulhsuexr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gbnznzjgo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gmrqjhylx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gltcgdmes.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gaynbqvea.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gjlthkina.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gnbsbwpmf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/ghbimueai.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gdmszmmlb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gixadwcgc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gqqxgbrzt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gdwmvudvy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gsfyseumk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gkyivlmfu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/giemqkezd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/ghnaywhys.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gbvvjswtx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gsbqzttkk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/glbdylkgm.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdudmqiry.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcqlhsxvl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gipvxzwry.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gpnpsodxy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvosxisfz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghgmrdmjz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gickwkwts.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gspyhiugw.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwljqacsn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gakhhjjcb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjukvapjo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/grftrnfsq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gakstpise.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glltorxhb.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gplppteqk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtbsmrwvp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gouanijvv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gdrsubrlh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/garqvrgbr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gsxfrrslz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gkhsxzxgi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gtskiymqy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gurjfqmrz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gcecnmgaj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gkvwlxzlt.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gskpbhslh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gihettfwd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gfzftgvei.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmyiwpvof.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gagkqhegm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gnzubtkoq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gumtcxwli.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gswcxyegh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gbjfrftjj.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gvgeoeoal.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/granmbjyj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqfdxgquh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gepjiacsl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/glhnhwhal.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbnuynayr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gbeijzzrv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjvmnrjwy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gufijdahg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gyfeifhfb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbmcllqyp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gavjtkigy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfaoyisuo.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gckmzegpd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gfbnxhjaq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gktqchgig.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyclogwxj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gktmvyvxg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gjxqardgp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzzgkntmf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gwkiylhpi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdxcgstpc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gtegnleeq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/geibxroub.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gttcqpydy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gkvkmyrjf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gnstdikvo.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gnmyzefqz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/ghtcggtba.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gharustcl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/glyymypee.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gmxngpoyn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gcbmqqexj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gcxfdhjkb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gsynffpub.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gwkmtxmnf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvdkwjlmo.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gexcwafsu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggioxtjgc.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/grrhwnryz.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gkwhtpzni.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gmktikjgp.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvclpgaeo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gkkyegwuf.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvshptbkd.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gdlvcvskq.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ggwdtfbwe.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gnmqbytkh.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzlccjgkv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gtnhriwhm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gfvtbqner.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmnixhi.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/grldmosqk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/giejuqpcz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gnlbnxwdl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gvaiialwn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/goiimbosx.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/guvwsqixd.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gfhopelsf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gpmtzfpbj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gctdbjwvb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghyzzxoly.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gqizdvvis.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/glqvveshz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gplioacdp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/grxmsbnoj.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gfnkixite.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gdhgkrsxb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gbtfkrwzm.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfsbysbjj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqmktrwxl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmokyxbdz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gmmsbdlrd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gfmlplpoi.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjepexkhm.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gbiwxwefg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gdrhapnvl.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjasjdbre.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghsspckfr.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gendkxvca.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzefglodw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gaazmpacd.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gtkgjkwkx.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gwpuoetrc.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gvfhnabfq.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gsdhbjzco.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gideumzgt.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcxibtipl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwkwbvjyu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gaklrekvg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gdfjdlnjf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gdfcvwfam.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gorcaewgm.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gczgokbmt.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gcpcnovjj.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghkkmzcfd.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gccqacuub.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwgvboacz.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxopwqsps.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/geecmydjk.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gcbqfosyf.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gzpuntqeg.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gpplrbosw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gxaaxejnw.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnhugxntg.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gioqtsynf.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gtxnyeuqv.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gumcydyca.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gkysdotop.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/grtiynydw.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gidtytwcs.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gldfptnmf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gsbdudmox.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/glnigqycj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gsxjuvqqj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gafhormmx.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmumeael.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/glxygenpq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gdtmhrzvk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gufzyeawo.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/goutyizxi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gjixbeppw.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gjmvpljfi.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gxxjksnkv.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gogzbnrxo.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gasxswgci.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gugumyzue.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnaeibuuu.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gmmysftok.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gxpylfrvg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gqpxldtge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/grqjmqkls.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gjddvdnel.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gnyunbrhy.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcwaalpwp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gilxibgqv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gamwnjtbs.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwangnjiw.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gumosjdws.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gmglqrhnh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gxzwzfisa.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggjawfiwz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/glehztjal.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/ggjxumczi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gqqjaqnca.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gndcpujrw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gqepgwjjn.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gzmxauwkf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gsyuzptvv.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ggsrselwm.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/grtgbarfq.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwavnvvag.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtpqmvzpv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gxwrtntny.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gdpvpnqjg.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gfeybfxbb.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gghclvkoo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gaujlwcns.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gtxcwophw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ghdrszoze.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gyypoejyn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gnjljkhri.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gstzzaqsi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/guagmdtcj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gixcmbklx.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gaiyswhea.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/glsajamhe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gfhzwfddv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gpflhbufg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gopygidyx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gqjgioplv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gszqjxpza.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gdxgfoehr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpjhidxte.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gidyaafkh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gbooxvoza.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gukdfwugg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggkwnnxta.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnrmwggth.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gtifuwgsl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gbbrgzytu.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gpvgzvwlf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gxssoymst.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjvswlyog.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gqtnraigi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbdixycmg.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gdmwsbyvn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gvrdfhjqp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gzlytalyi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gektfujce.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/goukelzrz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gszemhhzb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gsxclcavd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gkhhwbhry.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/ghzjjjhsa.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gmytpvica.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gcnyjgrpj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gowxcrihz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzgpvnhct.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxgbpwsdq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbthitfac.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gzazlwssu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gidyhjgia.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpaovbjpd.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gthdanfyk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gdvqtodox.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gtryzowyj.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gzjhgyggu.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghnkngabh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gcjceniji.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/giujvcxpz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gmwtgynky.sHtML


<!-- 参考信息 -->