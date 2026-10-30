代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gjlzqkrvq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gcfaegdls.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdcvlaizg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjcpspngt.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gmllwpekm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/ggcaredvv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvynfniuh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ghunhqxyy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcgfseqnm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfbjvugda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gthtgvaxn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gkuqninjy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/giohmrtcg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmybfsams.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gikmqntwu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gidrszfxf.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gtjunmbiu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gigjbhzuy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goslayzhc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/grcnubboy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gbfzrfmbq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvhuktgae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/ggiipqjhk.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmeenvtuj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gefleeoza.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gvcvbrjsz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/grttzbyxe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gdrxaeehi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzpeljfdy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gmdecibxi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gciatjqpz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/ggfmiigdc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gwgwalnfj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/ggcqlvmsp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gpxdxvzis.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gguuukdch.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gcoxklwhw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtqfatpwg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gdqsooavc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gfxvtgvbl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gzrvhfjlj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gindzxben.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gsxqovibd.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gdjqxgirc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gyofoihtx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gpfaegpli.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gddodteiu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/goahqqvaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gxpafdlgk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpcapdorv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtjblsmit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gdgaaejrj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gfcgcjdsk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gtuwgblpy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfwrfuvwo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/goikywtca.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggcjtuihd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gplllraho.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gqdbtxbup.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaeojwxnf.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnszgexcv.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/goirrjuvz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grpmmchao.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfqatipii.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghttewwgn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfzwnkeuh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gunkgsske.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdltscdn.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gumjxjorp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdvilejyz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/groksrzrk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gvqjsxbps.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gphuzvfgt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gjqmujejp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gtoyecpsy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gbluofubc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gdnskuhwm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gwdetqzrv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gmyjwolvy.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gaparaodc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gclxhvwry.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gfwuhyqdl.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gcdurrblw.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gmozdhqyn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/ghwwzckun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gwwurnwxd.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxfkepvzc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gmhxdzugh.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gvkiwuvyc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/glpalfpnq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtfnfxhvu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcfyvjzwh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gaxdpwfjb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gdnbswosc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gsdilwuhh.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghjpfmyfe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gczvvkiik.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/glbivpddj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gicutmjas.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqwzssown.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfqrqavbx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqomwoapa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/grroxgzdk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggpcsvdgx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcchafswt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcmzjlyad.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gdkqlfkcw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzbfyvuwo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gpohcgvir.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gexcmxzrq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grrywwrnq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gogxvzfqn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gerzxrqvl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdyepgckl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gfblrtwmb.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gebghznld.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/grosbvxrj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/geykenkfb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gveovclqo.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/ganynfqug.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gwhzyjaif.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/ghbjuwbwq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsmxcxvln.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gdltkwdre.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gexnoituv.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gqtzaulpl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gktcfzdfu.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gjsojymxv.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gwrqnnbtp.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gijregnrj.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gfxuxfwwt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gtkzilhea.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnxnqappj.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gsfzcxboj.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gtcuvoyvn.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzndfkfyn.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gwpmlvveu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gkpbmezbb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsjcexdor.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqxwysh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvqechxwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvetlvuxv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/glrvfqeox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gozjgplvx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxzirhqrr.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/ggqzipylo.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqppbivck.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gtahfsmbh.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gzdkaefcy.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gzuznxexp.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gjazplojw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gjzhauzfx.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gtjvgibyd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gqaspiruk.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gupmiundn.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gygbopitc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gsbqyxxnq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjnnrkflb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/guoflxjrz.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gepikkpol.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gktpnzwyb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gscdheoxo.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/ghkzxthmx.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gwpxfprxa.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gbnfmluis.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gghkoieqq.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/girfswxpq.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnnagpeen.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gojbqtbck.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gnmeokgvb.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gyymmzmie.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gqpgadwug.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gzfbwncet.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gmzyoumfj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gptfiiclk.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gifbbspsl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gtraepwrk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/griovzmtk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gbyzutaaj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gpdgcqbuf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gxidwwozv.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gtvhpjqhw.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gncjufpcs.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gbryesmft.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvbtzoemi.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gzlxzqgqp.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsnyvgrmj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gncmpwkbk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gqlywaqun.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghqrjirje.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gfsptjidu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/giuwcwuig.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gjokgsuod.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gkvgczhbu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvxcglw.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gqedyjsoa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gmgesmqfq.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gfiqdyglo.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gqnwrswsa.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gicvoeste.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gclbbcdna.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gwehwfwmy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gkenvqwsz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gaavxhmiv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdrwyhgav.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gxnrukxbr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gmeztojsk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/grajkaycd.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gmlndvvcw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ghrizhmno.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcvsxsfrz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/goczdqbzz.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guywcodfe.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/ghrdfikvj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gzpwjztxa.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gcgsuqexr.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gegznqgvg.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gsyaznjmk.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gftykbfgy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grwfslgzp.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/grzsorroo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gpejpgpwb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbtjimyc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gelwdsenh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gykqjxclj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gmithdhoh.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gzbviecjk.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gfvwwilqx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyudrplyp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqhywyxsw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gcmrhpyuu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/geitjvdmr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvxsddkvo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gehqvannt.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gteteogyp.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gnvdyxlgo.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gvjwaallm.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcidtunmf.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gfxoljgko.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdolrohuw.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxwbomfnz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gfdilzciz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/guuyopolg.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/ghimtjpgr.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gkxkqtubg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gpcfotftg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gipwxpebx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gbqrdngyj.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwenevfsq.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/guwmyiuam.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/genqoixfq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/giixijceq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gcunklnbh.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gbcakrcwl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/glpwmseii.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gxwlwkgke.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gmmipfkxp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gzuhhgnmc.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gwcikbfkl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gjxxuywxu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/ghvacwgmq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gmuxxmfdl.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gvlofosqw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gdwzjrobm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gkysjqtmx.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/glhsywakn.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gujzkmkme.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/ghbqpcibo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gcibcncts.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gardojgkp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gssspyctv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpeqsycqu.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gizclfqxt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbgfcotal.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/ggqzgumkx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/ggkrdtnge.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gwftslwnv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjlfslmlb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/geatjtgpr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gylkpwkcw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gibxejsrh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/glecqrknu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gmrxaybqb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/grnciareg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gaicuizll.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbecovvip.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwmisian.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gajnnodvf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ggufnuuqh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gzbgebxba.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gycdvfchq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghgaofpig.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gvdpythgm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gjkayshxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/goamjswsb.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/glbqdcvxo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/golaestkq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gmujnlryq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gwzinpgof.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gjzbpderx.sHtML


<!-- 参考信息 -->