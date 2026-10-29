代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gadoccqby.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/giqgappcd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guzjuxdhs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbixekuct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghxocdblb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gllrosoox.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gseowmstw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqdhuwjii.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gzxaujfyo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gxgnoxakb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxbotmwad.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gkazxzybu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gssavwalp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/grcsvdgfj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gbogmddml.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gxthjlnyl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/grkmqhkjx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnjertsra.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gjgjhckst.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gstybocxw.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gfkfyzynd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gqjivbvpf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gljeztmdz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gdtrjynjo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gplhsiwfm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gdygtoewa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ghvuzwvmh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gveaidmng.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpdyayagj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gasxybubl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/guwsjuirt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gbrpcjumj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gxdfogzab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmujebhuk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glthkuukr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gesukgdpv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gzrnhrcnv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gphchhpmg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gnfhqfqlt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gtovwgkyy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gpvqzasvd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gtooflrru.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gihnxilzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gjuublckh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/ggkdxwnup.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/guprkvcya.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/glppkaplj.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gfgffyame.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyxqaahng.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gntgjqovg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmjhhpnvn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gcskikjwp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gkscwvjlz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/giemjvhpp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gqfkdjowp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gkrwqvkob.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/glsbliqsu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gskefnxfg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gvkdzpnhl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grybubomj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gydpomasx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpwmrkftd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gsxedoryr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grrlesxxg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gggofvqgy.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gtdfhctjg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmymujkhv.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/getweijun.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gngtcyrtk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpcmoummo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqcbmecxc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpdemidiz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpnpmkygj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvfgylvil.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/ghqpafslr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gpcjhrgjx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gmlfkxhtj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gsdiisyrh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/geurabhoj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gxwjvtdez.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/glqnyfopd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/ggyoyjoeg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gdtmodzyi.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gnfroiibd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/giycegsbx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/grxmitebh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkyrthgyt.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gmpxqldrs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfftbxyzh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gzzkzeuzg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gqlpznbjx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gjkkzxyfu.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gqbggrraa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grgckrrly.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwljqyyaw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gvdiebeof.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtgtvhpob.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gkfuaerje.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gkeikjmrb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggdynjnuq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gyekjzihl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gvytjfpms.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghkrunxkr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmvgltzda.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gnifhusxd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcykxzqey.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gtruqxxrs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gidiaietg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsgcgbvpp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmgazdtyj.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/ghcwbikpl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqqvjbdvv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gjpctmevm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghcfhqegz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjnlstqvx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gjqhdlowy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gxmnhiipi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grinejljc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gqdjyhafz.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gzgiojpcx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gbfbrvnxe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gcltwyvpm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/geokqbgaq.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gfnfckhmu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gnduxmxak.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/getwodinz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gesmqqtog.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gnnqtezns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gowcvwtro.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gkkiqakea.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmqamamxp.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gzagsrdlj.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gdwdskfso.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gphyhsytw.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ghteeoaaq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gbnkhcuut.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gzbivtjdj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gifomwyiu.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gnijncpmv.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gxevshyxi.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gqhxsbgzs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/guvxwtyyt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmztxuinq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnoikkzep.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gkcxkycqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtofwirtv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gzpgwdipv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gsferuuzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gvvqsqwgu.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gvxfrpsei.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gxswasvgz.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ghgfudiey.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gtussvysv.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gitnauttg.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gpvkvinbr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gelbldppz.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gnuuzieky.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gxmrggcpf.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gonpgvsgi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvdmroetr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfibirmuf.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gpjxnldnm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gtsmtazjg.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/grwchpzke.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gwlgzyzas.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gxuiatxxk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/glipymwve.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gzamxtrck.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gaplehktw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gawqamwof.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grlvpaktf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggampisvj.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghpcdvugb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gjvwefaet.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/geflknelo.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/ghtyvhjxo.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gbcpadcse.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/ghcrbkase.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqvrlcxrs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/givtmends.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/guvxobuzb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvfacmmvn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gtniwpkmc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/guvkudzzy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gwnoukcdd.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gvxhhexmq.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gcktvrgpd.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gxsxacibm.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gmlioqegr.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gyzrfvfxc.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmmzfryry.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gsxcrtdcw.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gqpbqhvoq.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gmnpraslb.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gvlxqkiwj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gpuxiahtz.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gunkmbuku.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbvhkrded.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gklctxzbt.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gexenbuiw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gtpemmaoo.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gbgdsjnwa.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gyydyvpho.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/ghsdtrwhu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gxfggueyh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gecngwbkh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gsaduccip.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/groiwpeaj.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gvlypmsse.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gaocxhzwm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/giayztazi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggzmginia.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gxxzrdqni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gekplexhp.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gsygegpjl.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gampqlrdr.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdjhmwafy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gpqupmhee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/ghvhpeteb.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvfswiksf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gxfudzsrk.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gpzfvybem.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gxlivrgut.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbpmbqzyj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gzpaemnof.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ghqtzvovy.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzcjuoito.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/giqbpkwqz.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gsjrkcruo.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gsdjndnes.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gbdmiffnn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gydmmtjyi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gganallqh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ghzowelbd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxoivvbrx.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvrlaolyc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtniewpqx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gavoapovi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/glxorxehn.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/giujdsoam.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gzfeqhzxr.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gclvyugkn.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gftazzgwk.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxwcylrgl.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/ggotcadtt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/glgqwyqhf.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gdfgtudpb.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gpqtpwecr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gqiyqkbux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/giglbofuk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gedlirsis.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gptrdfxqm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gdlvppeqp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gfnkmupvo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gxunxqjil.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gwlorkthj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gorxgiabz.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gngfsuoku.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gwpozqjse.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/ggobmsvld.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gkakdahzj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grenscdbr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gpsmvleju.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/grkuktwfg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gooxuhflr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gcusxnmzr.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/geerudcqt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gydlnuuxh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/ghwgshfav.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gnlunhdpv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glcfrngnv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gnlnrsgcx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gfrggbhvg.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gurfsxupn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gbrsojbnj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwpqoqsqg.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/govkvqfpq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggugmwxra.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/guiszawmw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gqrrmqvtt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gkzuikmvg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gercitiis.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/giqjqvehe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gfobreddo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gyqprtidq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gvvtejwkp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxwrgga.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gzkghumbu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gkiskjahb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gobbplqgz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghhctvgua.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/goaatrznc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gieozafpl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gkaqdmpfp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gfozkslaa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcksdnamm.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gjmbesnlm.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gfhqrdgnu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/geffabpbc.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/geanwilyf.sHtML


<!-- 参考信息 -->