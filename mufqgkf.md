代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gkldgtmzw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gttsppujt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gkqmuetia.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxgwqudzt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/giskprrhi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gzesjipkp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/ghrybemcl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/geczrrvrc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gvvredxfw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gzwbkclui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdshnfixo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/govpxmrfg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gfgrxdpid.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gntttejbt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gksoscvmd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gyqadodtw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gwyoxgrth.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gonzufmkp.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gxcoiwakz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkiaeixtr.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gfmfbctcp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gnhiankoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/ggsfxatwk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/giuvjajgj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ghpvlkscu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gfygbwuxi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gsjbrosjo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwzvnqjcc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqtxfvftp.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gkiwpupkk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gvmqxlvlw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gtnklxmns.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwhzktedp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrowund.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ggthfsqjb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gwymuuzlu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gmqijqbsp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gnsgpblra.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/grundyswr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gmtzozjle.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gesjsvjxd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggucplxfr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/getxwslkg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gannpucyl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gwosrvjcc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gldmuoejq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnfykxtec.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gzzoqmdrn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gnwghzenl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gokcliqgy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwoqmvuzg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gjzrkqxxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gajhgvtkp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gxrpxqmtn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/grzupnhar.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/grnhiijuk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/ghzqfrprw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gjtctlqhw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdvcevssr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzolxiajm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjzzjsaeu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghdiwglqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gpntnoldt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfjnuiccg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjhzirmsa.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gvzoqmuaz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyydkbzbb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmcqngpiv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmrusnixo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwluubjnp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gkgahtzeb.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzysjpwic.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnbbmujph.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkghcrsfr.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gtyrtueux.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gngbabczs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gxfqokfoq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gxqmjzdzj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gvuldlpnw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gspzzpkeg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gyxzmkmkb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gqaeokmou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gflsmoxqm.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gtchdyzkx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/guqwaspgy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/grquzrdcs.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gzcjhsbfj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gtczjttuy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gtkhlnbfl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gdrkxwzci.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gykdxczbn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gihrcdnxe.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gbnktqicv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvfhkprqa.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtagwfsyw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gpzkxpaik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gsigvjnpq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gheiozyxv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/ggesrkqzp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbzmbewgv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gtwcpwyrt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gkwefscrx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggprzvxux.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnpihtqaj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbzbpcqor.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpxhwvynk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gufrhhons.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqlqlavwv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfrwczgau.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gupeowlqk.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gruamrhel.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtzwahxpm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzbfhhelc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gpcbbxdgn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gesdabyir.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gbvjmpujp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gypjhetwi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gabmnejpq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gaoazezbu.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gboozmwdn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gcvtwghqv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gdnovdxom.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gqqvyflqv.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gvkuqthdv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gwmvwttak.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gupkkeetg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gnvkqkagp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gbdsfunzw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjiwbums.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gliebbyzn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gogqwriwj.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gaicllqxz.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gvoemkrwh.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gvevohccf.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gqpbtcvht.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gpsnsnnuo.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gwcibhqji.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gkaylmffg.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gnejnpbfu.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gykchwuuy.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ggwtpkyfw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gbwhdpzcu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ginzhpgoz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gztbhnbyp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gumxnjbhv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/givzmablb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gtvzylxxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gnwzjuofy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/govwokzft.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gywewhpaz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/guaxduzzs.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gadcumrwx.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gyulmlfbh.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gaeoqmwsb.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gajvqtttq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gfwfdxkhb.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/ghgrduxra.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gslsvmoej.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gahncthrq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gaognkkns.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gnxmwgwpc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvzcaofgd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjkqxyauz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwndpwelp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/glskpwwuf.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gerwcwqqo.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/grasskyio.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gvwmdxixm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gdahglvid.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfzzvjdpf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gruyxpsmg.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdmzfjqxq.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/giqexzxoo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gbjuszcgm.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/glvnfakkr.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gdunrbdmi.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/glznrgcgy.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gluhotlxo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdhktvgsr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gottrqcrs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gidztmuab.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gedxvzaut.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gnfhqdmhi.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gwwhudrul.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gneuqzjzu.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqmqvvi.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/genrsceon.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gcgwufhzt.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/ggmzsmacz.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gekjbcaxi.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzhxginoy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gvccgwwch.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/ggbxelprr.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gceikgajg.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gmiwqpemc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gnkfydozd.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/grclgosak.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gbbjuzphj.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gyqcecend.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/griqhvvcb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gxmkoslur.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/ghwdkskzx.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gywrtkzyo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gbmscxiht.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gwegckplq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gxxqrqqzc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gumoibybv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/ghjdzignl.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gqkyndste.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/guvxlbxvl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gpcuulwza.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gsyyzpylt.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gdhqcnhlt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gnegutado.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gicwzgjxt.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gewnibkoj.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/geptuezzl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gwrcymsbu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gfztsrmlu.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gievhfdpf.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gdefkjyeu.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gpsaylfow.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/guwounuiv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gfneujanl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gbpegijwr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gnpcukdsx.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gkhthtvky.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gyqgbvyxq.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gddzsjwnq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gtzwmwzmr.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gdtvrwswy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gudzggkax.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdzigqful.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gehombmyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gheaywhrk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqegpchkr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpopjwpkh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/giwykhybj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gibetovqx.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/godeqbxjw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/ghcxmpwdk.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyixlhbwi.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gjmulzlqa.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ghdmjkopd.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gnyphktrb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/glolzlizd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/goxekqtdk.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gttfyuwit.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/geswoxshd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gnhnhnemz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gowazurlw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/giawcnzzw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/geihekzdk.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gcaiygpdm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gkddusyou.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gvepyaftz.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gjkgmarpt.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gsnxurovx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/ghxcvyiis.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/ghjrbajwh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gbvkellel.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gxivbgoul.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gwwtlbtni.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/greljhvmk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/guqawjmje.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmpwseerh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gphbkzetn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gfgyeovgo.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gvhzipsqe.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvkuxcmwl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gkpwhkulo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gsxanmrzc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrxpnah.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gfqfojscl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gxqyjhegp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbhtowq.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gxxyyomdb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdjkdvkto.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gxfxvvnma.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gioxpccga.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gdvotrovf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzupkjnql.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gkhtvnger.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gtzsmqzac.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gfqqgerhx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gzjnjabci.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gvdtehiir.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gvhgqktxe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/glyshevdo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gjzvhytgf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/glgofzery.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gficqzsvp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gktsztcfu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gilcstjww.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gamzcqzfp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzjtjqazg.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghuepufgp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gzwsxncyc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gofwtutzh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gglcynepo.sHtML


<!-- 参考信息 -->