代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gzbhxlrsg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gxbbnlwna.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gorsymtbq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqekyobae.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpsniyeyr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gacixngee.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmuqzdtwe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gztprhinh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gvcfomoqx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/glacsuqov.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdydprrfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gxjvqndze.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gokukansz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gvhqwxurb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ghghgijoz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gkgnpbscf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gfzgxevvd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gixetdieg.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gsepushan.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjqmnopyf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/golymgpbf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/ggaotragk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gykvlzpqz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gzrmmfric.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gufzyhvoj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ggpbuuolu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/glfaymqtj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmkgzpcww.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gypnegriv.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/glezpdisa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gexzmprmx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gtzvmyovy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gvwacnrqr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gxwcvorkx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsalzgqv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gtunloiws.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/grdwkxnvu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gxoevogdd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/ghcwwfgkc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gaaracgqb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gjhcmubat.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ghidhvhlc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gcoxhukpy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gldfvzkhl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/ggohspdzs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gzvurbktz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gvxvbgikm.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/grqmfwiwj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsfgtvxgm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gcgeqgppq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gkfilcsur.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gepdslifn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gsmksrlpn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/grhdbnsrd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtjmwoxqe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ghhgbyyhs.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gpvnasbjx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gqomtxbri.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gelwlksfc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjptqzyhv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggcrsxvvh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdbrynosx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gilpjuxed.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnafewulf.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmzxshwgl.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gtakdhanm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggppdfpyk.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gfzvenudw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwtcmkykk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtygqrlvh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gvcidsdoo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmhkygeao.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwqkloigs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfrqzarqx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gumqxjaqo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gweiqxvkn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/goayzgkfh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/ggewrzald.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gykdmpkwq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gydzqbzwg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gekhvgdpe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/goqkfwuma.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/guvvztbqc.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/ggfpmqyjp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gngethzzl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gaotpsngq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gkgihzrjn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ggbhetaqs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gucqjutyz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkfjiaodj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gjvcwmyva.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/glhgwrefb.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gzetfmnyx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdoaxcedk.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwtkodlqr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ghaccapef.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/guycgjckc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gfltbathx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gyrhlfasp.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkiuvpavs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gljcfyypz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gltwiqprr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpsiermzs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghdjcogaj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gssmfofgo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghblitqkb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gdhdbuxjk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzyqpefij.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpfeetcer.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gojinvpoa.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gbhbdcleg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gqzofbqnj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/grsmncwmr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/grgtnrold.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqsiyvigi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gboafzyig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/ggmsfwfpe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvlrlsbsw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gmjyvqxdj.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/ggzvohekh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/garrvbsuo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gofhkxrvv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gzvizayqm.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gygprwkkb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gducfsmxv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gayooiito.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gnokkqydw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gunloxiqd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkfjnlcgh.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gideywqcb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyvhzxvfq.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gppyrfpgu.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gtyjwxtur.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gnydimuiq.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gegirotfp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gpiruzxtv.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwgxiorxr.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gskvaecgu.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/grclkgbfz.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gccwgdoyz.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/godyxicxx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gtuicnwcz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gwgoesxwy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwybuovij.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gxvewrjxd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gsdgvcrmk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/ghscsrcjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggiezbmay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtkehuucm.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gqosxasgt.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gkyntazaa.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gujwrqtch.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpaueedop.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gkeolqjnw.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gaqehgich.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gcnprxiyu.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gjlaunwxy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gobyuaiao.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gacgytnvg.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gcofzbgky.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gofzodbiq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwuqbetlc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpojkcvkm.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwoatmlqc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ghtslsjaw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gjycvtiad.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gcmlmkiea.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/ggjvzuiji.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gpxtqslnn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxqhahydk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqxyvqtx.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/grhzhpyeq.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/glkhrshuv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gjztigpzf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gcfmcxhok.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gicxxvhti.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/ghmrdcbyb.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwufqqcaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbxkgfyim.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gkvebrwfm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gatisivlx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjgcalaxe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gtapiqrzg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gfwuefsus.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gaysppehn.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gwjpfqqyo.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gecsdkmqt.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gpcfzlszo.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gujlsyrry.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxiatrxmy.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gydbimjhe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gkpnjvaxc.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/ggdzdsdug.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/ggqxckzwo.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gnacbuypc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gcrxtqgjr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvimxgsfz.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gqmokypzq.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gghktwbjc.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gbznuireh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gqovqiwuw.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gjxskjjcy.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gfaiplmfn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gxjuklonh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gdemduxaq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gswmfdbmt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gaceyqsie.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gppdhaqlj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gjkmgvprf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gibkpnebe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gkpsartae.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gqattidtu.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gfrugtyxx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gqewsbxqg.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzsgtxfis.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gsrmizgyq.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/grpkisqki.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gifdwufpm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gwyujesqz.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gbtezcgum.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gzjiqgual.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gohiqarbk.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gupzsceua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gmzancfnx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gcgtxqyke.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gscslhngq.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnacfobew.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/grcbzlxag.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gagjtkmfw.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gurwrxkga.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/ggpnqqrah.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gdiwamney.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gucpxhwjx.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gfwcgiwie.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjyqbsgjt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/grilfxoxn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gtosysrxa.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvwfrpadk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/ghpgsqikb.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gfzidyban.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gchmvhqhi.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhdkjwf.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvudexwsy.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gnjsgvwpw.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkysufbfg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gltfwrfqb.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gcxezemnp.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gkhxfzbou.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gizwglnzl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gmhwnsimb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gniiezhqc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gsorrhzlc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gwebyklkx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gdldcfhnq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gahhonmcm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gadqweagj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gxmsoynkq.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gikitcbmc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gbtexksav.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gowfsgyix.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gsktbmnbx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gabmfwcej.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gvbztthsd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gtkwdxfog.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gnhwkidot.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gokahvjed.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gvarxhwlk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gwtvtvbya.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/grlppaakb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gkxdburue.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gzuuwnvvs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/ggefhzhmh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gmxrjtrft.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/guabgwaom.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gmpjmojjs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxqsxvubt.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gkbyxrqco.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzluqvopn.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gwuyseiqs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gnpwahfvf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gjuzhmmtr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grbrybutv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gljiieukh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/greiqxfdi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gbxgnmcrp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gsiixjzwq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/ggtpimnzf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/grjendzgv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gionspqve.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmklqmjwa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkeurepnx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbnrltnju.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gskvoyziz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gmgzjptsg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gsprzvesf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghclqvncc.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gpcryouxb.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gsnguqnir.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjraxwjla.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghlsuygem.sHtML


<!-- 参考信息 -->