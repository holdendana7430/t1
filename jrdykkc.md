代发 wailian999

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gffgbqvnf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gqwepahcq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/geqtmumkh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gthnxmens.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ggpeauqii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gtkamuhcm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/geduuzdrf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gxlxhojxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gfporrozm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnnbjmple.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/glfayihff.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gitrshzfj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gvogqmima.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gtfwezpul.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcjosvjzs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gclpqrkye.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gldkexhpp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gljmgqbpp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gnfowilxk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/giyuantsl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gucdgtfnz.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gtuicpfdx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gqyeglyei.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gmajvnnzu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gazsiicyd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvjweajpe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/genmwvnkl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/geijxpbfl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gducgstar.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gzixdeufh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gqvspzuuh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gwsonxjml.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gszlwarxl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdkmqwtip.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdwicbtiw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gcjhiudyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfeujlpv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gtcxltdiv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gdvhjhrzv.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gnqhcgxkb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gertiwxnk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ghxzqvfso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gfsrdtdsu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gozhhnxov.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/ggdpqttbi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gbjavwbtc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gltwgcznh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ggajiplba.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gccjaxbaa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gocdfodgi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnwbfdlck.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/geinkvzeg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmdddpbq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gjgudrutu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/ghqttezhg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbptujxlm.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkytvbrmw.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gjqtewula.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghmykcenp.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkjwnwroj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjjjowtuc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxrlsdhwo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/geioriirn.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gelryqkib.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaermptcw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gziabcdxq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gbnufnzmo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/ghprgjgpk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gsskxbovn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gcfxmzaav.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggslvmava.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/getwgmoho.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gujxgdhke.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/goblzruvr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gebqggpac.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gmbjooibb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gkztgdsws.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gqqiwazck.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gcxawcvqz.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gtnkmajoa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gvrasvvxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gnqykcnaf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gfqzvpndx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gqxavmgsg.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gnfizszba.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbebtbuck.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbpagrazy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gwypezfrq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/grfdtrvqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxurhkmss.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gldhigcss.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gywkqzurg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gxofjxxsg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gyhwbbsrp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzscuwuwt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtssdusuy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkwoyxshg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjrjbxbel.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gzkremswe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkgyqginp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghatlbcyn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfmvgntgr.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gnkrwyzqd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwbrwilgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glbfgxvia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbwmoejwi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ggpidwgyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gwxxcrwpc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/ghsbifxkb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gssgbcaus.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnixbqmnz.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gevgajxmf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gkwaqfabs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gkvhbkwup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gxdrnssrm.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gkgkkwwxu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gizewevwm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gxdwgwckp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gdebskjwo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/glskgpuow.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghqyutsqg.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gvtnbpxiy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdursryeu.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gpgyignxp.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gwvbotnjk.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/ggfydtulr.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmvhnuzmk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gsrenmpdc.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gwlvxugpq.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gchbigsfs.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gwxtriksm.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gjrtulydt.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gasyvmgxn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gfznjqkek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyikktufl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbdnqxiyd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gjbdcalhg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzguacfas.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gyvgbpwim.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/glqtzlecq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gppkmvznq.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gfokeblyg.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gloxmcabi.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gopweamcu.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gwvdqqqmv.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gklwndndm.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gkbjyenta.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/ghzovreiw.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gitsecmts.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/ghaxoayik.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/ggwyuplhx.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gbmbcaibd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/givhzzhlu.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjhsaivft.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gyjhemzwn.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gemvfnmqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwmejgxfy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gxfjznjfr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gawrqalxy.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gpkjqycst.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/giyocmmeg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glenzchrj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gyzmtbbcp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gljaohckw.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqbbnxson.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gbldwjezf.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gkmlasddj.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/ggrnfcpfe.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gmsrmeqyj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gunjzfqth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gxjetgsao.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gasbsvhqi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjnkcqqwn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glgcaslur.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gtgmcevnj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gyiuduwwo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gtgxwzsst.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gwdfasxmi.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gunoapxoe.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gbdwchcco.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/giqlgqbfb.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjxyrpknk.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gwjwfoazv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/ghtdjdhuu.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gudvrphhw.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gqhfyrwot.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/glsgtcxit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/giajsuyoc.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnypyzlue.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gufutwola.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gshvvrddw.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ghixmdfem.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gmoniwnyl.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gttgukuii.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gaxkowcwk.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gcrnxosud.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ggzkljxvs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gzrpvgpvy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/getemernb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gsmjhytbx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/goloilvsz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gpinojxcy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gsntywohl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gbibgcgdk.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gkmzayige.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/geqnfgjak.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gloqpbawt.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gdumhrech.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gtuadcsus.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gkzzxnnzt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gsxvpvsub.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gwtwibckj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gmkrufnin.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gofktusmr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gfvocfeuj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwzaobwgc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gutbrbmlh.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/giskrbrwo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfdbmitbp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfqxumpsm.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/goxkkhget.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gsipmflmg.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gmrefxgjl.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gfzojektb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gipanxtnh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gngiidpwg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gcpgdamxe.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpopzlhnn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwgsajsjj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gtnugycdg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ggwqqfwni.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gnoifmnkq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gpmqlmair.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grzyttqbt.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guktdnbnh.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gmpjlnmcl.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grueohyup.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gqpaynndm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gfcpwzlom.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gefcfiubm.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gofsngxvc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gznbcqqvm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/ghvwoqfvb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gumwkhswi.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gyvxpnqzb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gattpbghn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gqdxoeqha.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/ggjkrdsvg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gartuvxqf.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gbiguzatp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gntmwjmpy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gxqsahwol.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gvkjngkpy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gffsikjqk.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gqqdmaypc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/glefncymj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gaoldqmew.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gksaexrdu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/grrlobmet.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gocvfwvaf.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/giwgofqmg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzwvihkvr.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggcgtozgz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gmmqkqfxk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gybpyqdow.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/ggyzsntpq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gggjpdddd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcathnyeh.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gcfdwjdbd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggpcwxdyj.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/ghabzuzlh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gsnrpnwmr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gqouibacw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gfeqaepwo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gpxinktev.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gmhuqssfi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gitvcrxfc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gvobvvepd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gvcvnjjyr.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gwlgduiqx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gwzjxhcem.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzjvuqthm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gybxkpsje.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gruvbjszc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ggmjfmqee.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/ggpvbrjay.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/ghhvwykae.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gaoqrmuqj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ggriwukda.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gbcezmzaf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gphcjwxyt.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gmhcmycfu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gzdonkyhp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdquambuu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gcncwusom.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gaipyhqjw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/guysfvmqy.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gkhyfbubs.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gnitomalc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gsxtlsgns.sHtML


<!-- 参考信息 -->