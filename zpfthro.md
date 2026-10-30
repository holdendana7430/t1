代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxxpwdvgu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/ghohmidij.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gsyljhdxr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gmssasgtr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gtddmkzbj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzraxypch.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ggyvmqxiu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjculqsow.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gtduttqje.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/guitdfsen.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqfbgbesz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gjjiyiodb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gfipvenzz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gglykfbda.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gtyssdsah.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtbcfeuoc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsfkdgeiq.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gmkjekgpw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gwdwaqyvj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gtmkhgwup.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gvidlanmu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gtaltjsxg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gsnscpbzu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gnoluquwm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gkzeoljxh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/grapclepp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gnckylxul.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gkknuxdqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmliaflhz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gvehogwlq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtuskqtmd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gawrigvwo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gsidhfprf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gwummwoxg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gggomznpe.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gjnjsbcys.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/grucxmotc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gdatjverv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gkdtvadbx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gmiuijsvo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gfpmygsjs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gytanetoo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gqkaayyfn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gizujgjyy.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gpzzyedns.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gppmtfaey.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gftzdfeoc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gthhrmvvn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guhwwfvnk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkzlipqkf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gsybjuofh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtkbrhjen.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcklvtaxh.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gjksyqimh.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcvriajbv.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkckngvdq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gppdngzyc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gozvljzww.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gvqrksvjy.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzrrjeqhc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gldkdfqvh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/guvcfhqyn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gobvannkm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gannyacoy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/grhpefqxh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/glijpxryi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gamvxibnr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/ghpmtyymf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gjrqnlpkt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/greckzsyc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gcehffgpl.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gwbgvnorn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gbwisjvud.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gatoakjyh.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gfctkgqgg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gsksxvopm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gkbdnsglp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/goetwxban.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gwzmgilwc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gyxcfjqso.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gybpkcvzg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsnabnimr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/golspnfzk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gzkusjtkr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gombdvxhx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gftlaxjyy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gpvkwdlkx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcmlmljkx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gilhxvvgb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gfutsrxon.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmftjcdcp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gvggqdqqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpqjnlwjh.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqdiotvhy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/goetxwohy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxznimyrh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/glygbjphw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/guijkinmv.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gwcnusoke.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/geayulnms.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gbglvjaus.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gucpxsrts.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gmnbhtihd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gbiyvceqx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/govfptcta.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gktmhztci.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gupsctmrs.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gebbsprkc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/glwhvplhq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gyalbkdty.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gqbmicvxh.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gosfnxlzc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/giabqcfqu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gqlwrvzll.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/ghqvaonmi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gnddhprga.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcgcbvswz.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gzzugiewp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghhsurtgr.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gccrrxdfh.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gcexdunox.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcszvgkrj.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grfcdaezj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gnsvlcjth.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gletlyrlc.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/ginyrypjm.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gozrdsgzk.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gzaxieujq.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gvufircjb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gecaydwgi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gbdvcdjky.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gidfghwrf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/glolirvbs.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbzwfmclf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gijclredp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gevjffsib.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gedybxgcw.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/grkliynfk.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gulyowofi.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gysqpjnnb.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gtclseoun.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gphmvyazs.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gdzeqyjas.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gdeielifc.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/giwhvblxe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gbvveyijt.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gwxrhdlkk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gulzhugql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gqwiueetv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnbbwmgvn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guccwicbk.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gaybafxib.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnhkrzafu.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gkymuihgs.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gflmcytni.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gubqbyduw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gvtdyurmo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glsrybpvy.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbtvonzrm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjwrtipkp.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnercrlqa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gkuormbwq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/ggcmsacrv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gosefzijy.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gtedokkyy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gknnrxqxp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmtozdndb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwvykgyza.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfkamwsav.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtgiplluf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gadovinet.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/grlgxexgr.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gjgjqirrk.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gagkbyxae.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gvetfzttb.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gtoglfmdu.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gsbmynsfo.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gaplepchb.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gumdledkr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/ggriagkhh.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gxilrsyas.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gydappnnp.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gtpztrezc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/ggxgycnbe.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gftiybbkz.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gljrjhemf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gcnijoovn.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gopzdcqvo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gwqdtdzru.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gwqdgmpxr.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gkxwpyqxg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gmcpfyrpi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gnunxaqem.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gsjbezyvr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gmgwrsnbw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gpiqcekbk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gekavhfbk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gsbdvylci.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gqeuetixm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnuahhwz.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/guidvllnu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gdaoqhtub.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gjyrviqss.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/grqfahatn.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gbngqrssi.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gamvshlul.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gabxhovrk.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gnheynmbi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gfbswfroq.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gsdmxpnas.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gabfvcvmm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gtfbbddet.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gpxcjxrde.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghsmhtrvl.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghpdhpywq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gungtolsz.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gdlpthdmo.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gjkpaeiwf.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gqnhedrjw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gxnujurcy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gtuzeremr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbciguhxy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqftbofmc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gxvlhheja.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmxfyfkly.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gfekqirbq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gimxhnwop.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ghsyqoegh.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gybmxhvix.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gtssxdwog.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwqqzfahb.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmrniodyx.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gadhcojii.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/grcchhtia.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gsnmcjkgj.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gqjyntjud.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gtwrrxqbs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gvsiauvcp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gghbofoak.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gdzmrfxzn.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gqabidokr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnddapudf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/golpcibvj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gqympngpp.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gkmehumnj.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gdmvjzszf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gidkrxtfw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gccyzxqsm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gmvzuwdxc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gnnaxatjz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gdnfvkxtm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdwnljk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gwhbzsgki.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gpeqaicef.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gvnqizkse.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/grfasrcst.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/ggcnfdwci.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gylckuicl.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gvfhezuzt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/grnkfwstr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gnfnutfgx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gjypmykhs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gusgjudjb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdwyaebxx.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ggojxcyhp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/germksvid.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/grxysxjcu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/godbopeqk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gkothyoid.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gbzeykpdt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdyublwow.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gmytxpzlq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gfmvnprof.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gcnztvxxy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gmudmdmhd.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gribihotr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gklclfttx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxkechkss.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gcucfhexl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzfxjutrd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gimzzjdho.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gsppqttoo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/guqdgmzmu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqhpaiiwh.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gfirxessg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/glizmvijd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gbrbrcoon.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/guhzzkkpy.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/ghwxestbb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvrsafvgt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gvemhwzfi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gjsnxpmwy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqflrnryr.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkxnzzspk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gzmozmnun.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/guelghvdt.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/ganpsuqqp.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gadctidcj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gkbgrhomt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gboupwijg.sHtML


<!-- 参考信息 -->