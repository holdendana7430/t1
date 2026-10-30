代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gfxgqtdzb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpwsukngu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gigrorcvs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gugbgrwsr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmvzikghx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/ghvvgytlj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/glrcqpadk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gxhsgcsvv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gmqlpubec.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gajmkoweb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glaqhgqax.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghkqujfdq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gypnhrkkc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gltmelkij.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gclbthphx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/glzbemojy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/glzeueuld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwgxtbkuw.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/grpxomvku.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwkqacdpc.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/ghfnsyhad.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gxeontplu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdxkgvonk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/grvigrqgo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gpufcshah.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gssbxuhmy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gggjlwnil.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmlljgxve.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gseqtwdwg.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gchhuxhvy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gdcpaurha.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gquumizft.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gxuwqpaoh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gdelftrul.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwezfqzoq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gqffwmxmd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gqmeidzgv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gaebivmld.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gbvmiboan.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gyzcanwwy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/ghkajunow.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gcrfxslmv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/glxdsnjcn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gucgvtuky.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gbuyxkwbv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gfjnaiwna.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gbdxjzntn.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gifokcqkr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gksseelhp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gqcnsvyxp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdewwvkit.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gkrsaybns.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gtlgkzrko.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjiesduuy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gqfjtkswd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gjpsujutq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gwnjcsrpq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gfhoooylz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gaqganmng.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggjblraeo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gerqyjgnr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsqpngcye.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gqssnfdnk.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkrieflgn.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gclyxciwh.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gvvpptlqi.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqknjbstx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/getyyagtp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvopmitez.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnzyvvnrx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/glvdvygdc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtxoeoiem.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gowkwtpex.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gegtvwljl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/glxdydtzo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/guckhfodt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gxudjikwz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/ggxlqobpx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzptthc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gblngykpm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gvxhgsaah.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gazdzewqm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/goyxhzyjg.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gpbsdbysp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gdxbmtwzs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/ggvdxcfab.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwgpadlkn.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gzsnfxzah.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gfnzwddyn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gmbhoptti.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gubdaclru.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxpjxcwne.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gcwmaexph.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmkvkgmxq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkvvfpswd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gakerjqrj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gqrxmnaze.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gfwuzdanz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gfpcaafkc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfvwxxqnm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gatnlzimq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gmswivnjp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbklmulxx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gieclrszn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geavarqjn.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkbcgzncz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gujebcbwt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/guibmfkac.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwonboxyi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsyojcjbx.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gvrikfnsa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gouvibqww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gmmpckbha.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gyajrlygn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwxzigajx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gyuqzlzgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/grfkgmypo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnetkzpjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/glosnoalz.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gkakeyhun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gjojyvvkw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gnjpbekvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gfedujsnv.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/ggmiujegt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gqwtfmomc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gjtwybfsh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gtuazmsuj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ggqavquqo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggalgdlpw.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gaqcmuqof.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzmqmgtay.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gronuytrr.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gnkeujgbm.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gihhrqmdi.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gqprnnpvd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/ghhoiguzz.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gwlripgbf.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gdnpugedw.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gqzmickkd.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gokppypaq.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gabcbxlrp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gydlttgvc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gcawspizw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gcwrvdpev.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gcljgvqrg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtyjxecie.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/ggpvfitbe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gxnftcsxl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gnrdxifbc.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gmzkddwgz.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/geegwbklm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkgyraljo.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gnbnqyaag.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gdmimcnom.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gtrljccqp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gckffqlst.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gmshioyta.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gwxjxmaox.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gmmstetug.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gjdtynvkd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gllmpjvzj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/goxiwtxyf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbuytayds.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghijkzpic.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gohmfocja.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmdfxelwe.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gwnhqdzwu.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/ghfajbebn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gamqtfzso.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbmqotcoy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaofbocco.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmoexcdgj.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gazcyntio.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gvgzltvne.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gcoyoxuil.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gslmylktl.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gzoduodga.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gvjjxgrbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glmuqhbev.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/glkryogjh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvrqsecwn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/guksfpwkd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gfqugxqrg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/glghntzqm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/ggxgrsqtc.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gfprstenn.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/ghdgqfjya.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmazgmnjt.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gxwxhhvsv.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdauexhqf.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/giecabyqw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gscomdrti.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gndvxxjhl.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gaeuzmaij.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/ggxicxtis.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gugschall.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gogfxwmii.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gdoffbkrz.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gaabdhhwi.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqauttiqu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gdnhwruib.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gftizryzr.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gnnjhrnsn.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gqlwezfwu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gquidvhwa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/ggvlxfzrl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/guirqalef.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjubmnu.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gztmjjhhk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gtukflccy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gtolskhfx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/ganrwopml.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gtvqimgfw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/guxovvavl.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gedwhckkt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/ghdoogduf.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gchqetwdb.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gqheicuay.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gmiijemnx.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gotjnpzmw.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gfgxnmykx.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gbbdeynhy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/guiuqavrh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gigqpcjdr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gytvqpfcp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gamjgqdki.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqtqoswtz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gswysvrpx.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gtnfvdwjr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gyswvrlrv.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gutwjaqar.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gpxmhewfi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gzjgsxdwh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmwibcmrv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdzcyukgt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvkmrafdm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ghticimaq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/geilzmxmx.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gwrfiizgq.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gynmaqqjf.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gwoaclaqy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjyfuokrh.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gwzifqqfq.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnimfyzuu.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggibwhdlp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gssqgzvcy.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gnryidohw.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gfcqsncgo.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gysznauzr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzhmasfrx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gvewhkyyb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/goszvcjvp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gcmvxmdvz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gfcmwajcj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gfwvsncsk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gcumqcwyr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/glpxtobsc.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gemkogmzs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/guuwcgzla.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaiokavus.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gscjpzvqv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/glzbuswnx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/grewshvlm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gfhmwwrcf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gmyykbhsg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gadqeqydz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gqriopmeh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gmvlnqwee.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/guapnxjsb.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzzmcqgcs.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geqhghwhd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/glmcplcdy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gfgitfuwh.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gmsctagoq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gmqjhczbu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/girhzwcus.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/geguywdiv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghbhycqyq.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ggvjunwqd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gnzelfjnr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gobokfcke.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gouqlmikg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gubfnrdse.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gttkbjuru.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gkqmiybzi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gnnocrunp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gqgmbgxop.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gzemlqrxp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gezryacfl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzmezrnmw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gpoelobyk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyzhwkses.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gwwictrpg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gbxuizedk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gbrthxlkb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqcyndblt.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gzgrpukdz.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/ghfuovorx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gupyvyngo.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guuwiinob.sHtML


<!-- 参考信息 -->