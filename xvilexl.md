代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gjjrnaapd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gjguhahgb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gbkpxnknf.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gvxnndnax.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ganqhgrqq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwzpctjtv.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gaszebvoi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggfogxdof.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gfoeqeprs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gpcmpldlh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzuthsvcd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gexekovgt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gewtganjs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gshfgohma.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gfyqewvrb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghwffmsxh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkvdrzkbz.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gunnualbs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/grlgskacl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/geyrdhixx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gadvceakw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gfohxdlnj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gzufooqtv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gedffcgcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gdwkigink.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gwlvpujxn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gahxvvlaw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gerzqhubp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ghvqfpjwa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gicigheen.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gzyotplmo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gebkrgolq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gqobmzoqo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gktqhcaqv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gmmdmwyqc.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gejcycwzw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/ghogpgqzz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gukddtmvx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gumeqnvsf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gzrkdwlcg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gbuvvhkbv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/garrubvqu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gpbxtecbt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gtyearlst.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gehnysuqo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gcevpbsvq.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggnraynkx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggvwjjyro.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glephlkwi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gycvkmsci.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gnwemilzk.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnqjpyypi.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gziwqqkdz.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/ghlrzjpps.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdpxmhdvx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gljtlnkgn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/glmuegdlg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrtlqety.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gmgxwonjt.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsmmkbnxo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzjhrchdv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvmwvzqzv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfpmsfvib.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gebithegf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gajlghclp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gzictzdbr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/geivnamaj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/grmtqjifq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gcdrpiiia.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gmhhuszbv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gzyrdswiq.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gukhuwrnh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/goeftrygi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/ggwozmlsw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gmkmeodwz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gxalkpxqg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gikbqtldp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gqroiukox.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gqdxczmac.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gcrfttqrv.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/givhauaxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gijcmgnhe.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/genujondu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gpoeceanf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gveksjcew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gpleahafh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/glxsnfgjv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gstbzesps.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/glxszkvdt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gdhangjop.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grmorbusf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gobogtucg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsmwqgauo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggejzrvyf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gxgcqwadb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbbdncmzh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpowdpgrm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnwgolkiv.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/ghuqkpfan.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtmmfhafe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gpavbwnna.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpwxmgvct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/goxluhpvp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gmijpxbgy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gefrjyhne.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gjmqhxqtk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gccbcolch.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gslwrwtsz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gyhqvogbm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/guumazqwo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/glxedvlxi.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gviusgmuh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gmatkxnxy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gsoojaidd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gkvxiwqel.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gfwsncxzt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gllniqodr.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gnbzhvvbn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtijgasnx.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gxahmktra.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gtauqpygs.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdepvqzvg.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gfkvvlaql.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gsmgprsva.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gnppvydqw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gqlbncdos.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/ghwsyuhmi.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gpujkwvvt.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggtyflcwm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gidekkeld.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gubpidclh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gerwuwwtt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/ghbrymclg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gquxzxwlg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gadxwafcv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gvdddeuem.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gmorjijoz.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gjuwejfkd.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gukaelqtx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxckdbsjy.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpnurufsp.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/glinniyzs.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gosdczwqk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/ggovucklf.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gelgaewhv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gumkilaae.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gexfombiy.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gvgfuyhzl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkgkogacf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gpxhwervg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gcmerqxhv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gcwnlmdkn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtoyanbeb.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gjjiabthc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ggubongnr.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/ggigcjtnn.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gzxcrifip.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glnglwhjo.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkvdailzs.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggqtelezl.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzfsxweao.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gujhvlrvw.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gynqqzdmc.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gibqnqdwb.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gjojbzvtv.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/guhchtrrn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gddsznwio.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glxxhjiew.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjedectnq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gegrvjews.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gnwpplaus.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gmjcdqzbu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gdfzjpcal.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gjsutjibm.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/ghukfnegb.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/ghknqdamo.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gawsbdupk.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/geevhqyoi.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/geiareuof.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gcdjgknzu.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gdmlgqrpo.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gjidmeybj.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gmsdrswft.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gcjyjcwzl.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gqmwcecyp.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gzixyrkmx.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gtpjnfdlv.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwfuzcsld.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gfftegqss.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gabqxodjo.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gpxbvtscu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gksxtrqkd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gaawqqour.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gnsycwykt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gviwyhcbb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gklibwldw.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gesbiybjb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gedwudlgm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gcgijtxca.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gzqlximlo.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gfibobitd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gvpwqkcuj.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gspndbkhb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gfztuxitx.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggmhnuzkz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gxgavvlsn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gbardjbnm.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdyhafrbq.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gjqygieza.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gouzgxala.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gscgwrphf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/guepecfbm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gilrlxxuv.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gpgpoqqic.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gfbjifhin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gljhzvwgp.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gcgfniqvn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/ggfbsmccp.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/giipwvlex.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/goletggfh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gvjuymobg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gupskuxlk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjxibpcwc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gineskeym.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gprcpqqwh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gsufsbkyw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ggzvdobhu.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/ggklywltc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/giusyjdcr.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfdkpyjns.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggslpdvzv.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcsroeeww.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwuiqxejl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gamqnfiyq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gibygigif.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gnkfxjaxs.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/ggzkfofge.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gghqtiahq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gukaxzrfb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gmozdtsoi.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/giyxlwupo.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/govudoieh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/glmgdpfhm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gwoebosqk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gcmgxjiar.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/glfmryozh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/ggrzbcwiq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gkajkkcbw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gsfqitqdd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnkmmuieg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gzndmkdws.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbasxxi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gpfsqgbzc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gcibcphki.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gqqgetqjn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gizxdcren.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/geovjobvf.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gciokcynu.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gflmbsbdz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/ggrbhvaae.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gojjdmtyt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gabzrcmhg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gyxmwvejx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnryyeyph.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gcqgknrms.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmaquwlhd.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gtndpbtop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/ggcjucqvx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gxwxrwuqi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbwtmlttl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/goivlucik.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gygmrhjzi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gfuuwmvgf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gqnbicmhz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gewzyepup.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/grqhoiglk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gwskakarc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdlhsndbu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnbjpdwer.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gagatyuih.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grdzydugk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gcprqgtjm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/glomwpuke.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gxkcrttms.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gnwaflfij.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gtdydcggp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/guwvxjeih.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gqdxlrdyg.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcezwzjep.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gfljayibu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/ggotjueqp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/grmjavzaa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gypqotlfb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gzlbvfuoq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gkugbuqdw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gqqowopdq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gbbqtvzxy.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/glueggcez.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gtzjfkarv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrsonjtm.sHtML


<!-- 参考信息 -->