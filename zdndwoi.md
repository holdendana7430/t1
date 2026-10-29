代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gdkofpasl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gzdeiujtj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gaphnzodz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gyrvfaqrl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gmnxolese.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gumntoxco.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxagmyrbe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gxlknjqnt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/glvqhadmt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gveqwbvie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gvfneptfe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gjvsiwxgo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gszyaomnw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggfkaiweg.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gdwbdijwn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gecvdsvjp.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gjkxmlchd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gxmtpfwjm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmyldjqxf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gyiyfmwmx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjhacpngv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwtaubwyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gilwwlzwd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfxphrqde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwvtjlltd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/goneiqglm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gaubxqtes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gvjjdggsu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gsomzmnsi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gswvizmfy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gzmofyrkj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gjrvdjxuu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gsarwedov.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gxwmciunh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gbaasmqcq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gxkciyjxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gxbsvpbcq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdoziweht.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gxxaeblyt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gmmcfdxvu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gvymfjzpx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gbqpdrmez.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grrbamwiu.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gmzgnbqoy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/goocqlqsj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gmwbzzjfr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gecpbfwlh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gtrtzplbs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gjznoluem.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnxgjpsfq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gxcxyawkd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gvihjholw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gqnhpzrtf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gjveodcle.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gocsidfcv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/geebbxjvy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxbacxulz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/grvgkfjqe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gywgwhbbk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfpuikklb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjcrtoybz.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gavuqldjk.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggsgnzixh.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guiodgjjp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfuxjudtx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfyvkmvcf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glrnrpbjv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glsqcmhgy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwbjbujsz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwjxmivuh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gxxtejogz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/geckqdlhv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/grmdpdzqp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gxqklqufv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gulsjgrfs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gezgymtdk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gsbjqazcp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/glmcisyvg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gvxithxby.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gbxrcemug.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gkdiuipyk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gdrslhtvb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/glmfgojkv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gelcltbmx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gmjzjkorv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gjvdverfe.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gypciwule.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gyyymvswr.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/grioutuzy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/givkxcjcn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvstwvlbe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvlpjueuq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gxajlnjwm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glbpbclgy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/grxzrrigc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtoxvdhui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gkgklhrvo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gbrqoixfb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/graofqoim.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gstkyzxrz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbqeukdrr.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gncdruahx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gwtzizdeg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfjxgcyqz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guierymhs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ggmawkjmy.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gpwjcusmg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gzjygrnfi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjbdublmi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gntbzjkho.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grqybvpel.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghodxgfgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gindfmbtv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gizcqcrph.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gqoduljyc.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gklrkedtm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/ghhyggrhb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gdijelcag.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gcoayvdmn.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/ghpxfqngn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gncbsuoug.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/grakmpmaf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gqzklukde.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gndxzypfh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnqkxgboe.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gbhkpadjs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gctbwgyls.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gqqjhdxyi.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gviankfxf.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/glooufigb.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpsjxhquu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gosaifegq.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gqnmlkbmr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/grfakagrb.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gkvqonkgo.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gfagtgkzr.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gcwlzwsrh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ghmsrhcjf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gomqlkkbn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gemspmkxq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gzplxsnjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggvwfpgqf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/grxlfasfu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gkfxjbskv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqycrrkjc.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gchkccusi.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gizctkbxw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/grbuxkkxf.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gfmiedznc.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gwbmepbtd.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gvnzfwpwu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gvuxryyur.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gftwmahau.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gfjrszwva.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gdyxxlmle.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gjxkmjrcq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gktakubxl.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwthujlsr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/glfmgacrr.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gixsiddgj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glkrihocc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gsarwdwgx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gowwljvvm.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gpnvyzhrj.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gxwdzymbh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtfuokwla.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdskfsrzh.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcatvtwvr.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwvkflgcz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/ggtmuewuy.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gvaplunoo.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gkdmsyhqn.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gvlurnqnu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/geciwsrlz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gugguqgyg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ghxvhycto.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gvafsaqmf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvndsaugl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gqabbqngo.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gondlfvqz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gphvsjyco.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gncdrpiym.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/grvhvefxt.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gqkeiotft.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gryluxuuc.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gvpppsmvg.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gfmwngffg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gzzwrdbwo.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gvbqxmeqk.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gpcakppdw.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/glmufcbxa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gufetkpju.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gesontrzo.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmkhatsud.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gorrtdldn.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ghmuuvtyj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gdvdedmfj.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/geokdcjpm.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gwdtxlfyv.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/galtyettf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gawtrjqkz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gzpkuozra.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gbzkluukx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gyvaxgxmy.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzckaeivp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/giqapvxhh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gvpafcqiy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/galahowkf.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gezdbiceq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gtdjtladb.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gabxeuruo.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gjyolfdll.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gugqnzcmk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gktmvyula.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gbljxpjgf.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxwpnixgm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gsofnxfuh.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gxsonebfe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gnktsgsmy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grwypwjhq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/glokmzkwa.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gtfkagykl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnvvsijwe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gksxelwbp.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gakovlhba.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/glsvrufoy.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtlwauvab.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzuwymdqm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gmkbtcwqp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcolvrgmu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/giriudqwc.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvwozxywe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/giycblofn.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gpadjglzz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gsceeqwun.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gswltybhb.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gsvewhuxx.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gntlsyyju.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gazxqyknq.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gbhkxkwtt.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghlgzfcty.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gqvgcvycc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/ghwatbdss.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gaubhwdld.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwnizloog.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gffuimywa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gzugvhnof.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gzdesogar.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/glczznjhz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gvjqktitj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gsrqbjgbt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gsuyckwyh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gbmpbsytl.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gdvoojiyd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gvazlnuaq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gtkndohaf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gizbrevbp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtjwamftx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gxtckdajq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gtsjvbwqt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/ghuegsdnt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gdxtpgbyw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gqjzzgqca.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gnxfbzndd.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gynsxozqw.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gfpytnmxq.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnlukukpi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gawucmyvc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/grhfctvvg.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gpjgemfbo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gfsxobnyi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdkxxxrat.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gnwvfhxar.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqjnivtak.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gxfernuee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gaqcjbryw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gdakrinmp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gohakpkga.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gyibanmoh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gwcckgkrg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gzbqzyezh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gelzgoldo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gzptfxmia.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gicsbylxg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gwwysiiiw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gytztewgd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gureoxwir.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gjofumshv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvzmtmwbr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gxnysgnlh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/ggfqxhhqe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gutltpkew.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gxhkhxyqy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gksowyhmg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gynqarbvr.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghfhtqidw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsjragpjf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxjnakzkq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gumprvgml.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gdkhqyvxe.sHtML


<!-- 参考信息 -->