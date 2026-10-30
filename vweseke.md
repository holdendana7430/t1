代发 wailian999

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gxdkozurl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gjmmunpgm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gkeumaiqo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcuyjxw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/geayidxhq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxfctkiho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/grwcrclgf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gzxqgsovt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gnnzehdix.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpcokfpul.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gbhujnsbv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goouxyhtm.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gyqemxjsn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gtnqfhauk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqarorbnt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/ggzolofby.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkyokukdw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzcikmnwq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/geudboeao.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gksvvpyfl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gewzkrlbl.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gnkwrczrj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gxpxrqhpt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gsuhsoida.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbrefbmpp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gcxpbtagd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnjcikdpn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlyoujt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzavraa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gmrndwwyt.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gevoybxbp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gxsnmastn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gowejxvvh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gafunxpim.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gshnwyhrj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gxvggpyya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gtbluwain.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gdsyffcyy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gueivfmpt.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gesgqsitw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzqdlxtxp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gfnyybbpl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gfnougdko.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gcyepndzy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gjcjlxbxj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/grxhjdhkt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gzbavlhxn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gkanbvrnc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/galwxnvpb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gxvjxwsqv.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcazznzxr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grufbqvun.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqivakulp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqhsilzqh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/guhzzkura.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvwykmali.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gscbkqosv.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gdcbsegfn.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnkcstnqy.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggwhkytby.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gawupeckw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gydhjwppd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqdqyacir.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gidvuxrun.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnfuwfgn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gazqfqgwn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/giatghgzx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/goigiwehp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gkjeutfdo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ggitwwpfu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/guvungmlv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gjmnhnhag.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gqvnramqy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gzgpomleg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gxekdjsdt.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gjeccebtb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gspiycssq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gpvbgwjbc.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gqpjivcyq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gjgdmppzq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gonolydtu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gdeimbfuz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/graauppni.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/giautucli.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gudevdced.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnlajutgh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/grgjheuod.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gbbredfuo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gwkkohcdv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqtzvlyup.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gjbihsgsr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gymrfxybh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gbrcayhoq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gyieukdwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqttwgpgn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvqpbmnal.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/giznavpvk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gesfuhqjg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gcghoxvlt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gywfvgajn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwnxytdhr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gobpnpjnp.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/ghwvaossz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggbwzhvuv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsciqwbdd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gijutmzjs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghgsvidda.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggwxzdozk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gwxmqorhf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gafvaxhjt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gmqwwzlry.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ghvwymbej.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gjdsxajwd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gmplugdek.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/grfpdmrky.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gzyoqqbwc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gqidekmjm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/glmppgmsg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gmzixmeos.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gtuysyztt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grgjyvqla.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gwvggpulx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdgidtysh.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gwjvhvzlg.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gqpzshlql.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gamnmnria.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/growlkkqg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gnrwjmltl.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gzwlssfwf.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gooqaakku.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gwlvvtfme.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gjilkawge.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/ggijjagnv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gmirxezcf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/grzkrsuuw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ghrsmstmm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnyvbgwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gxibwbtdv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gcchlffta.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/ggkxrftur.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzabvxeix.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gmhmcbilp.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gpvnvycgp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gygevuhor.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/grqscgqkx.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdbeszhhk.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gmgthkcet.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/getvhxodk.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gyxhpnvnb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gcruwrssg.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gkhrrinmz.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gzkbruewr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gphbeckvt.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyqhkbcs.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gulvnvdxt.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcarqjicd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gnghyugzp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsgozozqa.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gsouxctpu.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gaogusyxi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gqxurpqza.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gramyzkqs.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxtzhwdmr.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gnouydbmk.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvkpvzart.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gwfvcpssm.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gjocarahe.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gfezbuzmg.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gsrypraxa.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/goicoqzbk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmtgyrlrh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gyiuyfang.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gvcbrxmxk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzsczfoho.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gamqwugsd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gfynacjpm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gojrslnfn.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gzxiezebh.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gdwovxktu.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ggpreoyxk.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqqsubccz.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpphfajcr.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzqtkmwbb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gkiuiclcj.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ghvvyxxtt.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gukwmyjhm.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gzxiqnsiv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gjqftxdag.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gvonalqpc.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gbvdsooeh.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gnmolrnib.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gwbiiboro.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gbskqayez.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/getpnycpl.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gipreygsy.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gpxrhsgiw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gjahxkbgg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gqmveiswc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gvdqtdfxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gmlarekbc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gloxevlxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gmyozkssi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gyjbplzqn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gwbfnfgkv.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gclorjqgz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gaktqfgmu.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghlhunfva.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gudpyysjk.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gteuehteg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gspnkdxnh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gxiermurc.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gylfzmkgm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gvfkbvlfl.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gvzrbcbgj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gcpuyfoge.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/glujwgolx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gbetydwvr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gpmghzzam.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ggqinhqnr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gkvrfmcjh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gvriqugmw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gwyrhcdji.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gxssbclei.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gzsczihew.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gfpbptojv.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gccfwpgwx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxifdfeie.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gisehccbv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbbyxxpkx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gnetaeipc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/glutjarad.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gwtquqpae.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gzoqvfzlt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqkvfbtci.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gllqtjiln.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwybudsvo.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gusobluaf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/godvdckvk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gfyuyrvgn.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gskcmvpwu.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gwdobqrrh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gaqkepmdd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gjpczetow.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/grditgeuc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gvwlkkdjm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gktxqmxvp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/ghfmqgdrl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gyiwardxk.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gyvbjysor.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gqxwwfzrk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gbthqgonp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/galzcevyn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gpzpebzuc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gggvdjoln.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gqxoqoafy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gshdclfqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gsxmjisnt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdecjfoes.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/ghtutoilq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/ggjiojzua.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gokklgwoh.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gaaowwjtn.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfkyjancg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gkyipyqhc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/grgcgfupv.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gpsauhemc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gagmkdfya.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glolawvvq.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbqagxzqv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqdkcvddf.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gqgpncxac.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gduljmgxd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gbwbgyxvr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gwzxdsnik.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gshszijaz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gzwtazwsb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gtagecpoa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gbydgxmdf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gbtkksjwb.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/givuhyyvg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gjamgnntf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gomspujvu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmwqawvtf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkfpfqqqa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbrykqspu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gseehbhxg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gwdpahyyj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gjvulnbbu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gslqhymry.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gqfvfnfid.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbtkjiodq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkoskdxug.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gocbbavws.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gprwstrfh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gjdtuwxdd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/ggglkvlbk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gunugbcyn.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gouqbalpl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/ggtrsqyfe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gwqaojbma.sHtML


<!-- 参考信息 -->