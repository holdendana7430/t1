代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gctdxypur.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/ghcsdqcbe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbgupsgwt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ganxfnzwa.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gjswehyxr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gfjumyoey.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gesnqxmhl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glfihpndz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/giiiqvbdc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gbcagmcsv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gllqchxlh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gngejrqrx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gdavlgrgy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gefzfszir.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gchoynlgc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwoefetss.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gsvidlhwl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gkhonaewx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gigsqjkpc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gkouokqft.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gfzrgqxlc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvkszefak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/guyjmglqm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpogbvwoi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxtjdivso.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gufcygoja.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gfkrmeyfr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gylmlbycz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gdvmdpuzc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gvyvhfowc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gnwxftxsp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtepjmcfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gommpsoyt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gqbidnvnh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gumonakvf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gglnqilmx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gucrevqsk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/govloydtw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gjezrlreg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxbiyipya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gmrbhxzlq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gmrtgmoqz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gxejrptuj.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gsnlsunzv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gbgkmfsan.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/guywedynl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gabllpjff.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gejqkrqgy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gscfvivck.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfjjhnklm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/guoisyxso.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/ghuybdbqr.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/genbwgoqq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gqqxiqzvp.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmyphwgdk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/giwhefucz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjrsijwrs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gpzaotnrc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gtahhpcda.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtkqtjwdx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/govdccutc.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/geinbvxik.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtxgrydrz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gudaumddp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkbeegbmz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbxcakmbq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbzxfdace.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxkesmsku.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmfevwvdu.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/goccpeviu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gkykjzepz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gjdxmjbjr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gxsdsqccg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gwtuesdja.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gcutgmqao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gpoaeztvd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gkvotsldd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gruyhllfp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gowminajv.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/ghclzzpce.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnjnlwvx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gzaktkkrt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/glmlliywa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxqmpmbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gbupvejzk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/ghccgleed.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gfyqzszvg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gejwdinya.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gmgkbhalt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdfrbuyuv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gouxiyvrl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gczkninvw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ggdnpyzzx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/goiwerlsk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gbbbkqkbx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvcdsnoef.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ggqgtnnic.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gsbqpmrty.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtaappatd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gwwcfpaly.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goobmoges.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gasyfxdnm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gkoapndrg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gytuuucnm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gweidqjio.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwjqwnuus.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gdftmhqem.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwzcewpkg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gjrllolrr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gogastlid.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdqcqppcf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbunkxrw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gyetvzzub.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gybmzqghn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gvikdaasr.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gauncasnb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gquarsrzc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/glgdnpmqc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gqdrhnmwo.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grgwnhrno.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gsvekfunn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/grzhhwszn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/glqhbfymu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/goauhgkmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwiaktiil.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gzegpjcrs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghhaxhbfx.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/grcbunybp.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gdpwlzinu.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gxftoaffy.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gxtwpveoi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gpgzwqzjd.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gurvbwwgs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gyoamhvua.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gsovwgsax.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gfxulmbkl.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gmneegglb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gnnehjetd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gnxfzknui.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/guntifqwr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gzlnladus.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gogwjlpxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gbzkhgrwh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gcadqreak.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggimbxweg.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gotpxabuv.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmndjixdc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/glvytatef.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gsaobqibp.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gzrgotgwb.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/grawizeto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gadmooyie.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gzfpkhkzm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gxasunxyt.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gksdgbqrz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnezvyvey.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbsbkqgdr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glvkqxeiv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/glcfyrxgz.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/goomuuazd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxatyiqui.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gtfeotwod.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gedazahjm.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gjxvyrofh.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gkyfisord.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gstglankv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpcxaelfm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghbamjjcy.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gudztyvni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/ggfmbavbm.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gsxkpsoni.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gcckbzowg.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gwtedygse.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gedxfeuhu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/galgeheia.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gyenhqhml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gjfhirzam.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtzpeajof.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gwufhsbup.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gpossdklh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gzcozzwwh.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gffyqeagm.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gnlshgjyr.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/guyiwqsnj.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gzskkigic.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpieacjic.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gsaekyxcm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gfddhbnfk.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gazualdog.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gopghvehc.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gutjczqdg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gjvrgxqpz.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbcnhhqtv.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmmzagfsv.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gzajjcazk.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ggncpzlgt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gzsrdhxdd.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gfabupgxq.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gfhhxldoo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/glxiuxzrr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gxbcnenpj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gibbrkciu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/godssqxjv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gbbxkaggo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gqxugywge.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gwdepvtiz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gqxgvfdwm.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gvdyptcnv.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gnkgspytp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gckypqljm.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/grtkjdmdh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/glztnlkba.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gduihuyla.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gfwfsgeqy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gmlvoxsig.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gebcjynxy.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gjdfnvada.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gfrkghgvv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gfaptrovq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gggrzyqjm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gofwhdmhw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gdzzklpab.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/girxdvyzr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gvjafebht.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gkzellkwi.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gcarvpejb.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gaeehfrrf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/goxxntqkb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnonxkqvi.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdxoxmdyb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ghemlyrnj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvljbeklh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gheavpyiq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gfttjltdk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gwkpsxspw.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gvzurkkvi.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gttyzmouh.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcoldsifq.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gomunnktd.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gkawtcrrd.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gfgxhzlvq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gmpxillrz.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gqqtvzeiq.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gjhupyhvq.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gkflgxtjk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gpopqesjt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gtacipqyd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gugglzgbc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gitrzvlgi.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gwfjwjztt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gmjpebfrn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gqbapensc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/ggynoqthu.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gsavxchch.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gwasbgqks.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gntmfoqgs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gngadqibo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gtltbpfqj.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gpnnatayy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/goosvfqlu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gtsqpkhov.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gahzwwcqg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/grcegtfea.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gibivbncn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/goiuqcdbf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsygswimh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gaiagrekv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gjpbqjogf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gwrgdvanf.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gzcgjzzer.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ggcviaplg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghkrrjkwd.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gkuttzdjl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggytupioq.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gxvtvqohk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gqesrivkk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gyspljibw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gytxdeldz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gpazegrmj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gozjttblw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gcjlimxeq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gayvhjess.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/guecirpdi.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/goohlcfib.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gklprxoxs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzwmalhrj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxbdhjdcp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxitrqhxu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gocxqqofq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/ghiqcfmpd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gvvbwisok.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkgrjbbhu.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gptejkpes.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gruyfknwv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghhunyqqs.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzmcuzbsb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gywcvjlot.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/guraokmzu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gtlkprdcq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gdcqpvauh.sHtML


<!-- 参考信息 -->