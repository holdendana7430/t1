代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjrhuat.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gljcgojhg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gddiyzvya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/glotxdrlj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gkggoazth.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gzcokvlev.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gpjhlchod.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gcydgblrc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/ghoslzfkc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtbvhhhgk.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/giwgisaig.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjpilswzl.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gwgskuepx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gbyyogaqq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guzrvrgnu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gokirkhro.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gonsjknyo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdfvtpdzb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gawnlkuur.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxduvqglk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghhpjqjhf.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gdmsfckuv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gdafmxnna.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/glnbinenv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gdigmckxi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/glxxknceq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gywncmvlg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gjzduenpa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/ghfftemzz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gmfbbzrpz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gmznvysfp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gxnkbiaql.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gpqognhsl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gdmvwpsmo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdmsxwcbz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gbrltaamg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/grbnvsibu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gqmurqrdf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gyffjzwyb.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gevgwkqjr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gpdjiaqzn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gobfzufic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gbmeqttyf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gggjixrza.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/ginrpjzud.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/godoboziu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gyywoamzr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gummeuufj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gathltust.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/ghhvfoitx.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gglpqraxj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkifamhjw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkodnftwm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gwijrdvqh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gvqtntpqw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcolsbmsv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gonlwwpvq.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/goshqfvnv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggeofbwbz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvgphcw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gblznedre.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grfibarra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtmhzkiod.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqvixfnp.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grjkuhifo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxfecuadu.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gguwxqgsj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/ggepubwfi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gcfsmlvcu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gwvzwbhcx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/guiqyelfn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gbyrkshix.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/ggftejhvw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gzfyaaack.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gkisfckss.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gikswvrxn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gezjfuwaw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gpypekcrx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gqpciqjvo.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gizfycqwp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwlmbzo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gsfxanocn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghebccqkm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxjwdeobm.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gpklpumzu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsrxcjfoc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/grzcvcmat.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gbiiwmmgu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gyqxsinsx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ghpoeqhgw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gsuwnrbfn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsuxextkx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gareiunuq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gcssjlwkl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gduxehxjm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxgiqncrt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfylwegfv.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxdcjwpdq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gwjqzfkng.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqzawygqm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gitymcxtj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfcbayfja.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/grtkzougp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/glvsdhgjc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gbegwywrf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzrozanqv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfrhyufzj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gydoarwjj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gdymjcxdm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwosycaeu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gqsskwkyw.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/ghmhdgimd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gybsddseq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gzwvbqzey.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gurierogp.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gokcezttm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/ggczcazgo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gruqmhhmf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/glehauzvj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gkunfavtv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giznnmovu.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gahhkrkdp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwtsukhom.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/goshuqinw.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gkqoiwzme.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ghuauepkc.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ghxrpwffr.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gvmjvjbyc.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/giozgryky.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/glywgvgkk.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gathorjob.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gvetphyao.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gdzhilksg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnwiijqre.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gdlcyryhn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/glkcsroxh.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gtldxbivs.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggiziatmi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gtzqaaxeb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gbvswmozh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gicdjjvcq.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gzikpqhbm.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gdplbcvth.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjmbjnqda.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gktmjydtc.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gdvtltczl.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gryxwairy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gsowoytjl.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gzewptfru.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gpynmnypv.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gjhrqgnig.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/ggecqmryi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdbntpzx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gurvtivtv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gatrhgsak.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjalbumbi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfgmamnrx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gpvnmrljm.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gdzotoaxk.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gqadzvjso.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gfpmeyvlp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkihwpxhu.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/getysmpdd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwolevzrj.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxqmrarjr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gpuaedjvj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/godmehbsn.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdidupdlh.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gtilvmgdi.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gaamwimbg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gdiwwbkzj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gplugiqdu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gggkqnugc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcjkjarqi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/glizssqmo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gfdxbwuyb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gepkmmqnp.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/grkjqxlpp.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/greqfwmxl.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gunrhxhhf.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gvlmrqkul.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggicwacic.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gedwjhhir.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/grokwduxw.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gofsgsqew.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gzudamebf.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gszdsiewa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gtadoeabb.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gccyboxnv.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/ggedzanjd.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gehanxrkt.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gelyvgggh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gqivrdskz.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/greoilyam.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gnllwtkzs.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gxxyxgsoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gymkddakr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/ghpbqatow.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gugbdytli.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/goftjhpsa.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/grnnbdekg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/glkpymhfa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gwuotsznw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gxflatfbk.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/ghmcnvnip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/glbtoilbg.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gospqyasc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gcdzempgc.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ghvbiuxbu.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gigsfrxyn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gqrddtvcd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gdkewsurh.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/givsnooul.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhtzrkq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gzbufztms.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glrtmhboz.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gzflbdaqu.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gedsatgvj.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/grdvphzev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gduakvxgz.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gbxesgaxa.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ghscimtsc.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/ggceighei.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gnwkbuifc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gntvnoncf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gmvrjiqnk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/grqxdybbu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcxyhphor.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwlgdrxrj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gjdjkaejm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/godctppvk.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gcbiqpssz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gecbabgjt.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gaxxedhvf.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gzyxkixss.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gahmhrmpo.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gayxyrijt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gbmtaooqq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gwrzvjtgm.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gxsyhdwio.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gzygzlupd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gvihpbchk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gcypicxlm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gsooouxnx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gpdgfgeuj.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/giswkwmgc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/ggcooievx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/ghrwheveu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/ggqqbhuwu.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gwpzsebve.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/guvpvivzf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gsarwiiae.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gyobfkiyd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gmfbyigww.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gxuovirzs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gaipmgrgi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gzffdxlfw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gsptjjaiy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/grfqypgww.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gouhpqlvf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdvajnk.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gpsgknqnc.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/geclrhowk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gxegjwins.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gxptmrcek.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/geprfoqsg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gjbmvrwck.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gugfwulgg.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/govcvqvxt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbhscyoav.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gdfjtbhnp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/grlhrokon.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/ggqcaooxj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gfezpbsmr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gfnilwhzq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gxiorquan.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gtebfeweh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gtcunpary.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gavfprjzu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gmulrvbwd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gsvnkdotv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpbtejyzc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/guverdhgc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/grshkrjoq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gbwmfxpfk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gmntkhxst.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gmqnzqkyg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyhepurdt.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/ggnfbzvnm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gzwcznssr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbjhpervg.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gqkicunwl.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gpzajvkod.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gaptbmbkd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gzvfmlhfx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gxnsigeul.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjycfaxny.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/geltwmqye.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gohhminqp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gbgyewafq.sHtML


<!-- 参考信息 -->