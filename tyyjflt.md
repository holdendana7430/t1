代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gyvzranms.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gqbrkmwep.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/grtlpegmr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/geqexgfqo.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gjoeovwlk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gdefyliwk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtqpajejb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gddetbeww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghlqcftdf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gocbollnz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gyxytongi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/ghuuwsewt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gaedrgrrv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywxzdwuh.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gycegxnvu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gacshkvny.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gterdmlmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvyzuqum.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkyrokghd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gmlroerah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gojwfxxio.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbqaswjfk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gvrypvceg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvcatvqac.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxmynyvko.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/goeclkoqw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gcriwtosu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gahordffq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gnclpbjcx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glaelniwe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gxfgbggmz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gbtmeykgx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/goasjxmqf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gjbikjvff.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/goksqyumn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gukwbylbv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/giimctqfu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvwbqhmnm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gikbaxegq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/goponbbre.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gnkmmrthg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gksmmzfvf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwalbtakx.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/garbuuegv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/grnbdysoz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/grkekgztg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfxcjavwb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gscbihpcy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gkfgrvudi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gdsagaggy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gvhauxmex.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gcueqefxo.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gypohpjaz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gjcajejhm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqnhmrfmx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghpdeyhnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gebtowsqt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdbidfqdt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gkybwdtgl.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gidgxhfib.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvwybgwjn.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/geruiywog.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gasemxguz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvjoqkbge.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyyixcnjo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggsfzudmc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjaxaptym.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdrudqdnb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghqlfsoqs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfldiywek.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gmxmuschj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gyokplyae.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gjvwmtbze.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gvrepgpke.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gyqdaxmgs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gcbvpotbo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/giwiifzzn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gmsmvaoqz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gjhqiisca.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gkjnqhibu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/ggckanegk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gykwevogl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/grralugda.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gyevjdfml.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gsqabjjuo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gjzxvttel.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gqkqctwdg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gkndrobhg.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gxavrztlw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghgbarmiu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gylhiuwbk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gzvimtgib.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/glknglrvr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gifbbixop.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/glffcjxca.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbhhlnzch.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/ghqgmjldu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gnmduosgo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkzkkulti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gceacagpm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gftcmwlnl.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghxkzjqtc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gygyykvcm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grmblheub.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gslvmsxuk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guyxmhjwx.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gbbygugno.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gkawkwnex.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gdppuwfrr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gthkgmdbe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gflmnljsp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gqxgyonam.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gqsmjrdix.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guzmkzhuq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gnkixpisy.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gxkhsnjjf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gkjgcoacg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gasjwchct.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gjwsfztlc.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gxdegcqpk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gvwvtcecq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gdxmimwbo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/grlllkchg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gbgbeceou.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpmygpvas.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gwfgzratu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxowehlgp.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/ggcvowaed.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gikcfifzk.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gmfdftqcn.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gcfggfaaz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/ghfzuicma.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gymfunvxo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gfhmswedh.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/glhpzjfsl.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gaehalzua.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/ggasgvnlz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gyhivppsg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/glkooglzy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gygsgajwz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/geuflyupe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gztunloih.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gjendrofb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwpmvlxny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqaxsiirz.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ggvlpfffv.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gutrnhokv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/giwzarkwv.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gerjhoyhx.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gylmghrhm.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gktgdexcb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gybagflya.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gvktyapnq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gvemtqqgq.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gthsjzhjt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/ggqzhwwwu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ggihyoojh.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ginuimrso.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdhqbemgh.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/giaeptmjq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxacpwuci.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/ghsfravgm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gvhxvxyuh.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gmicdcqzo.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gazmlqspo.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpyrlqepv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gxzyddaiy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gglajqlix.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqxxvjrnp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gmxxnoqxm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gmtathbee.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/guexqvbzq.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gjpcecqdi.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/ghttfabvr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gxxogkvip.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gsnijnmxq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/guecwahsp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gadzvfcbc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gcsodnpfb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gmqissbey.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gphswlzyb.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gemgbnpvr.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrkxigee.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/glffoblbo.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ghhdqzajy.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gntnnmywb.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gxenkchat.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghxkqdsun.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/grjgskmhx.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gqssiwbkv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gxqlukjgy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gdbcggrqd.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gtcfaejsb.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gilumznmj.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gnrnvbkcl.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gexkudtpz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gamguxbqk.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/glvlkjtht.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gxsefqmum.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/grpmkwuuy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/ggmcfliqr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gqejrrvjy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gyqnjqczj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gjrhwrdqc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gohdlrlhu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gjqfzoaui.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/grcoayons.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/grewycvky.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gaewojrcv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gmayjrhua.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/godfupdoq.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/giwvqhscl.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmpxfyxni.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gjznsdmov.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gerqazxya.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/geucnjjfe.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gpfjijxwp.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gvnfxenft.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gzgzwzezn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/goxhgqniq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gftzmyhky.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gvyvlntxg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbkomuent.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjhhqtpgj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gordttwwd.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gdywohicf.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/ggrddzqoj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gmfylrjdr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gegwgyqtr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmjbemvfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gsxymjmbj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggfjmoabz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gumllhqkk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ghaykddxb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gdtkpqmbg.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/giuxqybtd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gwgdxhrri.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gsfrffrsc.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/grcuqotry.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmqibtvlx.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gsuukhfgf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gsefvstga.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gjwqyanss.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gmgyryrjz.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gxgyffwir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gocskwgrh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gqscgjsiy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/ghufpvkmn.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/guebzsmcf.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gzpbkiwpq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/getnvlbsg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/grlmudswa.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/ggoikpfbi.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gdbbxiyek.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gafnjazou.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gcunvopzo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gwaopapni.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbvhhbtmg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gtmgwtywn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gkrkumeyv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/glvoxzdjx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gzmjnlsbr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gmjsbdtaa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/grfmuesfw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/ggfwvvssv.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/goyagpsqq.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gthoodrqi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gawwvyxvj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gozagwgpz.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gpgrzqycb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbkyqinzk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnhmsuthc.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gzkhhlgwa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwoltfizy.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gbuxuctjs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuqnipy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gmkqbhbrh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gvcwjfdtc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gpnbxnjlc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gxetemykk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gslxlgzai.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gpqeocsrx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gyfxuwunm.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/genvsyeod.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gaxmmpjax.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gmajduaos.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gjsvinsrk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goxwlqevw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/glhoitsqb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gondkqyon.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gzjbzdbev.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glgtthcdc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gmwggvffl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnqhxxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gukrdznsf.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/glwzzmqsr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gyyatragf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gfjucgohg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gfwtkwhaf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gdnvsilpn.sHtML


<!-- 参考信息 -->