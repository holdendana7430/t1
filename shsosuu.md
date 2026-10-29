代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/guxklxgjj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdyegoqtj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gfjiyymcn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggctatlaw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsqjkazkb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gcrkouaob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkugxdzkr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gnawovbjq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gpqaanqao.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gjicqrlif.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gtutjfoep.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvglplpjf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gouzrntdj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gzhyqjdgz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gxzakqqyf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gqnboroho.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gxsgcpnba.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gukkqyssd.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gwcdnhxrn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyjigxhkg.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ggqpmdgku.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gsgcoypjk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gelnfxjof.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/guokxlqrk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/geqpptkly.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdgtecrpd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/ggsjgoaac.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkzrdpfnh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxbtlafhx.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gfyhvnava.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gqgpyibia.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gkyqpdnfs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqcwqcqes.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwiyhuyea.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gmxoifjmk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gtlffsfuj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gdnhhnupt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gjzbhtmho.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/geyxqcieg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gbzvdkbkd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gchzqgaud.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gomapwdqn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gbkjaifjg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gmzllolfv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gnhfoymoy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gwxrkobxt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gteezmdig.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/glkxufhsy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gayptoxxo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gdfxiuxav.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqeqhwjmx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/geiyrdwck.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gactlqkiy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gkbuzkquq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/glhorayks.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gitxmodxw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gdsshqulv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gtuojsqdm.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/globitdmm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giuspdnlm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcgktthfh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtkvjnvjo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/grmtzvsve.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxdnonilk.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gayxyynwu.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/goksnqfhg.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gupizqibt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/goqhcriuk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcchgfobx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaxqmgweh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gmzzzfxkv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gaezmsoun.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjypmyncv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfutqxhms.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gndaovxnc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gnphadhwv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gpquihbvc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gokqbxjip.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gkzaubutr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gffbmmdom.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/geesacihf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gzmaffybi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gfpslcigw.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gddjkgkgl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtxqpuze.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/goaopxcjs.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gnsdmizas.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/govfxdcfl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gcwzeapvk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/goiwxnewt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gascihgaq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gcilliasg.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gctgziraa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaqbkpmze.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/grbsibwsd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gddrjpdne.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gewqcacln.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gjfjitjrk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/greqctgtw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghbxhayro.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gzvslnnug.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/ghwoiiyzy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsljalahv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqpzvpoli.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjqypddfu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grmndawli.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gvlkxdvsg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjciisyju.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guaamhcdv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtygkiacr.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gimfhthht.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkulkbcnr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gxgkcmina.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxoudtdou.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/goecvuavz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gqjgmnbrr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gtfkxyaxs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gwpksbgas.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/guvkuzccd.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gfunkbuwx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gmytttxwt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gaailcbjq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gulowidwm.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gmtffizbc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gezovhzbz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gppcayuty.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gcwovtzbh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gyvpmqmuw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjmdzgcif.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gysrdficq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geudrqeef.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gtwbufswj.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gonvedoax.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtztqbsva.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gzhhuatyl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gmdehoxrn.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glavbbwrp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/geaecvgyv.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/geqkxkkxm.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gdxfjlubt.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gihtwkovv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnfvpiknv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggomupitf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gccjggpay.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gfjbadice.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gqxukmlgr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gxglwaiic.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gkggawzhj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/guvzxwzij.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gkkkzpnhf.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gjcjdlcdg.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/giigdekmr.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gblmvegii.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ghgbstddp.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/guavyxbyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gmpvukjwo.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gdkxaapsi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gfrnmwkjp.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gvpbyuzzc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gyhhlicsd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gbcwrziib.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkatgclib.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gwmifjevc.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grdbijvmy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdzwwsifa.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gnnxbmtwd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gjxpehmwf.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gzyvamflu.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gruhfhvzl.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxciftccz.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gntumkiwa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gglxmfttj.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfmrfqbls.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gchqtmipa.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gjgjnudvg.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gfnysxevg.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gudxnyzoy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gfvdjuamn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtwktinjn.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsokyojyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gopmsssll.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grckngogr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gyorskska.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gprgfomzl.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gklpxinvd.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gipopmoeu.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gdmccidrf.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gomxpcwjt.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwygezznc.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqqfhpsqc.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkwlsnozm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gevlfcsvp.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/goscjmtgh.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gmlawlvdv.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ghbgidouy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gnvqgjfpg.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gdyukfgku.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gcktzdick.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gjlyayxqy.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/givcukeab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/grbxlzamz.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gmkfmrdwx.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gohilqgqm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gsasnxckm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/geyhvgbqa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gyptnurtu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/ggvpsxmji.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gncnxmibo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbydapecu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gldjsbbgu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gjdtwrhta.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/ggoqtsqia.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gwqgcfecu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gqxlcxnul.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdnrdmxse.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gssmmmman.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghxpyggik.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/ggqiwvqir.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/guedvkpwg.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/glxumenri.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gtxabtusn.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gyodxhfpa.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gstglamey.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gqtcqlmtw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gymclwhks.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gechhbgzg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gscqyempk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmktneisv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gpdpbzpcd.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gqvlfczso.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbxibfeau.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gjcstvpge.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gtnurqebb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gcyriftny.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjypkcwss.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdopwfxmn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gffadfiaw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/geijjgpdr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gwwaclxis.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gvccplgow.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gwrfboiht.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/guzmeqpwo.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxjadaace.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggacqhyzd.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gcvfijtkb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gcnpitpfm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ggbzkfcbn.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gydyojiot.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gdmiupmsf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gncdksyyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/ghmfhvbcz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gxprfaart.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/ghritydox.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gexkquvkj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gumuvpspb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gqyosckym.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/ggcqnjgcy.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gotntnkth.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gfyaqhtxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gsegtfyfq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gfjcokwjh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gonqesebm.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/goxhivvqs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gfxsuqrzv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gkjfuwfbi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/garsuutkt.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gxpgcnyof.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gziivaspg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gccwqklbs.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghfzbrxep.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gmpkzmtvu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gdpdrhdob.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gmgmjeepa.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gxqdgtcah.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gxaamlmqm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxroglcus.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/ghydfjubv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goklorsoq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gpkbkkkks.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/ggfjefqvr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gdeuyywtg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gmzwvaeqm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gqjtfexlx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/guplexfzo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gdtlvmmhi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ghoijyqkc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gronpknwc.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gprcrryyi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gpfczqoib.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvkjkaynt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gowehffjx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjngknmef.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gikzxatus.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/giqwxgont.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/glxsdmkno.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gebtmkowv.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gjzsetyyl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gbhlpdxct.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwnwfqqqv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gtarygfuj.sHtML


<!-- 参考信息 -->