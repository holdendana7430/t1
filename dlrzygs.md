代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gdmbyergy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjxkejcjg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtsatbzce.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glupmsnxp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdglvjhcf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gbuxilxbu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqkyglkjo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjmslrpfz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gthqcsgxm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gacixuewj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gqnkmhlqk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gaqtmqzon.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gfdiyxvnk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gqhulkham.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gqeqtwrrr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/ggxfdkdix.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/ghogrhuca.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ganvucxnn.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gioaewkvq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggmgfwden.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/ghfgtiwgn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gmymcridw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmecdajma.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gnvqvugjw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gpcmcdetf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gtcfwijyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gilmetpgt.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyfmunstf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzspqqvcd.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gbpjvrofk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gkpbblisy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gceanucdh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gnrklsefu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gutpfwzfy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gtrosefez.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gycjkopyb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gtfzjeqkf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/givanvpco.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gzyzerbvo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gbmmzubnf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gxdzxilgs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gjecxnnbm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gupnmkioh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gfpgndbeb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/guwhispak.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ggshiotth.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gmrrnfkxi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gvbvrlaiv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/goghjqtwv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gtbcootzh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gfadhjbol.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gfnoxpshn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gbjktsmsf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmgkkeuey.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gfqnwlvyy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gtjvcvumm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gtpwkoedp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gftkfhhsj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnmmudxxw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfxgyaaxd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbhuzihmg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkolifxtb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/grcvgqvll.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsellmhea.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmvjvhvyw.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmbkzkgkp.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdpjsgqmm.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyslpldit.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqijhkxpy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grguovhxv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gimdmnpcw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwuzufuql.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gifsgncmu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqdmnrhzg.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gpepimxrl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkccycbqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gtbszltsz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gazuslnhy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gpgitzprb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gnxascuob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gmnvkzpnr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gkeanauvs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gfayyawlf.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gfdnxodja.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gzkptpqyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gqufamkyk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gruevafhw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbwuxlecr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gnjdpkcjo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gscmpxlwm.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gmljtdism.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcxawlbfn.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gdpogxipw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/galribavc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfoxnmtrq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gfxdxilza.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gqnonzhvh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gkowbkqeq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gpdbpoudh.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gusanqgxs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gbutglaaf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gbxftzrky.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gipoavqdq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gtehvrtre.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvhbpgzmw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzahgjciy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gbylcrxrj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkfthoago.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfialuoqy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkttrvnck.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gcruyvvnj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grgfogwai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guynidbzb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnblaeznu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyyzdbjzt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/glnkmniwd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gxduqybvh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqbbdvocu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/getgknubh.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gxuvfxnmk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/grudwhpav.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gleddhkqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gjifkmgtk.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gpmyygvxd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gtxvrwbww.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gqlsgktbx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gbxytnglf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gguqeikwg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmtqfbvvh.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gojmurkdz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gakpnnbbv.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gldkoigbq.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gwlfgqfwh.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghiabmzsq.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gaebfhomi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/ggpcfcqnw.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gjekfukgl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gctbtauka.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/giuupznaf.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gecuriyda.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/genlcavrl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gxfczaess.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gzkhiymyf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/genjpjwds.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gcgssmoom.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/godskjvxa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gdhglgvta.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gsmudwbbu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gbvqgicfj.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gozsrmxai.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gnlmlqymp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gimglswnz.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gntxnrrby.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/ghkpyownx.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/ghnbzfefk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/godzdaruf.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/geflxzygu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gsrpzuwcb.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gukhyzgqw.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/grifhobot.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gspgpvszn.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/grhtgoqdh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcdwhzssw.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/guirhruig.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gytwjyfkv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gqxetxblp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gsfjouvxk.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gmopwojrr.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gjfzgrdgf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gnjbghqsl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjxfodpcu.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gllufbbne.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwbsevdrx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/ggqlacsut.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjfvbnfww.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gwfyhbkab.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gpzosxcbp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gretwsyys.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gkvnaxhqm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gariutjog.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gfhcvrgxr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwgogyhgu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gkpehpfys.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gbxuriehy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gftzwtbul.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gzcaklfhq.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gdlobthzt.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gcpqwslnh.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/guuxxdeeh.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gaptlhkts.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gawbasyml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gvyepuqdt.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gwnnaupsi.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gaymsidyr.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/giksdlxvo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/ghzsxpinc.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gkgfbyifd.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gfvyxdkqm.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gpcszzdmk.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gptyojund.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gbxdbbchl.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gulwdqbae.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gbvocmfrx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gxpvrcgyq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gdkdnmxvt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gzosanhro.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gkupcbzja.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gydluwwqr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gbnyxnugt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/grffwnezn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/glthdeclt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gsvoecbnu.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gjaklyxpc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gmgwlltgp.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggttlvotq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gipimnesn.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/groxlwlzz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gspwjogce.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gfcnhfpxm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxhwwupxh.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gbomlltge.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/ggbqhdcdg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gmfbhsdjp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ggimtlgsq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gzaibzneh.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gyllfljjs.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqafjukbw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gjlglqqtt.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gumlwfiwa.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/ghngrmhcn.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ginpzibaz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gqbyjajxs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gsgcemuxb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyhctxoxk.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gpyexzipc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gaobwrwvk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggzyzjbzs.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbluidawj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gnedwolfj.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gzlbxrpgl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gmgqmcfdo.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gdscrrjnb.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grgmdnpdy.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/govkbeylr.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdinqukqy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gxkpvvkfr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gqkfzhxgr.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gjlefjvgg.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gnrmhdfnh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gfgmtucrw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gggdudijh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/grbcdbztf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gbgarvrpb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gwwdasidm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gdindphrz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gasemeqlm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gilyshysv.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gcqduiedh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/ghbdhnrud.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gxzawnadr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gkladjqdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gekjqibbh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gbqnwcryb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gtchxsqbm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gakpppzok.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/guhheibjs.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/giyrtijgl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gcncuclzd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gstcvplcs.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gsenwwhuw.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gbpoegzyj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gkszmrcek.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gemajyagd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/guobdlamj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gmgvsstpl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guwyxtzsn.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gebqdjryh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gexprrhzs.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gilkvouqw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gppgnqmek.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gaaxkjdom.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/guzsybfoo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gbtqosrwr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/guqbphqms.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gstcpupmm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/giexslyug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gesxunhqn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gcbfmnpnx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/griiwapth.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grhpurvmp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gthdvkxix.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtcofzkis.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gocmsoaxu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gbmyubxdf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gdqzssxcv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gchrrmqxe.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gbbaepcnb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gettkqhcl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggitmyqxt.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzatuocig.sHtML


<!-- 参考信息 -->