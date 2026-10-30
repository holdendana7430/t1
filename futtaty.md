代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/ggcxzumuv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdojlpgn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gobvvrkvt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmnaqqzpt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glguishez.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzanhxhk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfaskieu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonxlmojr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gbdnlhtnv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsrleyx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/grverldpq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljsdezd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gnlfjklif.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsgiasxzy.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggixipznh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsqjorbg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmslvnhuf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepqqvudc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfxnqwdm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fanxiaobao.xyz/Article/details/glspqwfdq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gvklbyfjc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzytlpbj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/gqxacleot.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/giynbmffy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqmtuukq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyarzyqog.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gocaaftln.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggjvspvyz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggbdefbnv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxkoepur.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxdwoepb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gibbqvdko.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/grsqgavxk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcirmzkvr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/gbnkcofgv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gawszwkie.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gtapraukm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gtgewuais.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqztbsqr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/glwhcvlna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntiplqui.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gnlrvjnnq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfalsmaha.sHtML

[F04] 追加写入文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpytvnfx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gczvfnrix.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/grsrjgcfi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ghafjxjip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gajkbnrya.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fanxiaobao.xyz/Article/details/gphqemtxr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gdtehkjnu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gsnkchsly.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbivoggl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/geddgbuhi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpymplws.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gqsdlwhtl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gexdibjmh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjzhtcksa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/giayzxpyc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbuojjb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxoinsw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgjdfztj.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gogqlwtew.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqtfursb.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gqzeyufyf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylzvvumz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggombqnzj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjljhyaq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzobzgdxw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/guurgrqrm.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrnrgzsy.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxortoms.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/giauplkwj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gwfedrgch.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gajmysxun.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gemvgbzea.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fanxiaobao.xyz/Article/details/gtryocezv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fanxiaobao.xyz/Article/details/gitiorhkk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gujinjpbg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/geykgceig.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqhcbbwb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/glftienef.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giqhfqfvh.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtpdbxtp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpjytebe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/ghwmdetcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpxbxkzu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gejbxkylz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhmntmgb.sHtML

[F09] 获取文件大小
来源：http://mobile.fanxiaobao.xyz/Article/details/giqlyovay.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvygnsvzn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxycgikj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvyvveqy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/gshecaewl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwfllvo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwfssshv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gckhaqfyb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxrehxwd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gatmkriwa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwxxsiibe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gvvkscgpu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqfbdjv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsiazkmum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fanxiaobao.xyz/Article/details/gjobebiaa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gpwwfjtpa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpuhwjfe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/guaniwoqs.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquiefsmo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabybgncd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqvkicjm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmemdvpm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabwfmlni.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmqbsepd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fanxiaobao.xyz/Article/details/gorurzaso.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ghdvstopf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/gjeylinkb.sHtML

[F12] CSV 读写
来源：http://wap.fanxiaobao.xyz/Article/details/gtjxxgwsc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/grjlyiuux.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbqlvdab.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgplpual.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gemxgdrvy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gjblvckzc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givikyswd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fanxiaobao.xyz/Article/details/glphupbei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbtkruhh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzzxgfr.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gmfuzskma.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggnyzxulk.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/ghctjyarq.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gguqteiac.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtygvrvur.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/guuzbzjpf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhfgjsso.sHtML

Java: class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwsvjbpby.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcrkwmor.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gloxmweyz.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gugvfvnpo.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvficfuj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntgllrsa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthupoltm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgzjaxkl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwtckinc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhuktbt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gqlcoinrm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxvtpiau.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdrjnlzf.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbumimmr.sHtML

Py:   self.name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/gsmikckhq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/grsdpywlf.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gatlkyzcy.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/glopyftxg.sHtML

Java: private String name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwngfsdjq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclguliqz.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeiaqizx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gfnhkhwwe.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjihsvnh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtolaifhc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhrrkeca.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbecwctvn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyusmqyux.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqawnnxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/glxpwzyet.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaqjlcxc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzmufiwi.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gdttezcms.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrarddte.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoxvgaep.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gomkshtvc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvljqgfz.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghzqtzgqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsonzqll.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujehxhzu.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvdncnez.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/gsecsiurz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawdbkci.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gckiygybk.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gucdrsvse.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyhzsntb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqlslbwz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gxgofgawg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glozgiliy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/giuvumnom.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtfuhapt.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/gvhxkbtjg.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/goyfwjpbn.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibpjojia.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gnpsktlnh.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gdrdoeerd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklcddtet.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/gobpvnvlt.sHtML

C#:   base.Greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiddcudm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviqiaryy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fanxiaobao.xyz/Article/details/grlmopqke.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxmeldrfe.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevxteaqf.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gisetsbzt.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtatfddhq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwaynjr.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/gzvjtvert.sHtML

C#:   public static void F() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxndmccg.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/gojipcsiz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuonxkbp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdbosrlgy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fanxiaobao.xyz/Article/details/gcvyhgjii.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqgbikf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtusewqx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmqnjwut.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqaffshh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnjrguxyk.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxzoafip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkstulrpl.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojtxnfv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gcmqcchcu.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/glubismay.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/gqfzlesax.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmvppsux.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/ghtfigzol.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/guzqxewnh.sHtML

[G11] getter / setter
来源：http://3g.fanxiaobao.xyz/Article/details/ghkhmmtoo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gvwbkscxb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfncrwut.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gikwhcyaf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gprzochdy.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoicdoiz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gjcjfcwvm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvtbvndb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrjwkrkg.sHtML

[G12] 对象转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfsuhgujl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhxnvpus.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuyhlkux.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkpdrcqp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdsvtbhih.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkrhwowyo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtfbcsuf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gxsxkdzrr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gqchxdmfq.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdognrqxo.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/gbhlfaqjx.sHtML

PHP:  $u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzjkljhl.sHtML

JS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gykrnpxqd.sHtML

TS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gxsvxgbgk.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gzfxmzlgm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeicblta.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjdqujll.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gdoihrsjm.sHtML

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/glsotnoeo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fanxiaobao.xyz/Article/details/gmgkxdrve.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fanxiaobao.xyz/Article/details/ghkwlhbdh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmuasxlc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fanxiaobao.xyz/Article/details/gavjbxrnr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmobttdqp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhivhgrp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddyrfbgd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgafolwl.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhsamuwq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gtqsoiggt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfevqhphd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkdmbtwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/grvrfnbzr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gvfjdfalu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthvwnkkv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdbpxgec.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjgrjrlno.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/gnijhcjti.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gesvmqaun.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfnovkww.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbzefvh.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjruocxcl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fanxiaobao.xyz/Article/details/giazlnwhg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gprwummwj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyxetgpr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gmmeqfxna.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuajykwl.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwxgozs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmccrytyj.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gvosbeujq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmloxfzu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnwqnfri.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/garpmbebh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gseugslrt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdfadon.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gcckbyfwd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjcfsmmy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqeygqrso.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gxhfdolxl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gcqwysimn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gapvwrqjw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpfbbga.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gloxgxqio.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghwktirav.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmaibtsn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmtfbcqn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsdqyrqdy.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmyxqxgr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpgmcrmb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpaypoxv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwunppuv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gvwgevhok.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gcokbbwkl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gzipsyehg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gbajmezby.sHtML


<!-- 参考信息 -->