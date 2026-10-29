代发 wailian999

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/glymkqpoi.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gaeidzrnb.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gvjoqrqsx.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gkkivjqxt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gopidguia.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/glumqjbvm.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gjjlchiia.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gahwdajxm.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gkqemdpyh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gggrkkkmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gyneeosth.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gbxnldilj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gxlnuyeby.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grxbczbzx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdeosvvax.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gipzwzenl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghgldtqza.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gdneorwfs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gejmhnhzx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gfvkuyedp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gjaajbajm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gpjiymmnm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gabqjbcuy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gjsjyaooh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/glajrbesr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gahifngbp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/glkmjxtlf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gekkgvayk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gxmrxnvnh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghcchyhok.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gehmcynbi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkzflxdmj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gaimmyhmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/ghfdxuotr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkcwnjpev.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gazmsmmgp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gzvlggfsf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghdznhner.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gvuuuidpv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gewasowfv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqwxiysjv.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/ghnoskufi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gnpaobwnc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gvbkzmdzj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzftdnopt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gikejwsur.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gnycbwswv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gbbjurriv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gdrdzfdzh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gnizrydeh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gxskqrpmq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gstkigrcy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gvhovcjfc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gyjkqsguj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/goimoebwe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gpwhlfmjx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gdxheolas.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gsednbbvz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gemikgtbn.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gzuorfqrp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/ggbudxook.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gditlmqxt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gukvgeeqq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ghmqnoixx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gfucjuzpl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/ghvupilcl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gcscsccto.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gkpsqwnko.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gmvjaqyba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gmbwpkpsx.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/grwqrxuax.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkxegtlag.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtrnmgdpj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gajmhzrhi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gneetwppz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyewfeplf.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzkmglrgr.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gjhjnpcin.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gktrgeryq.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gorjekquq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxbrwgycl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/giycndnwu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gznhxefvp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqmhjuoow.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjsktmfac.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gndgaqlye.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gteumqvui.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gndktioyb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbrhznbqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gqzvbpvkz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/grfzdokgs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/ggbqwkwya.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gibrgdubw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/geewjxrrk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/grvhbsqdl.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gslxegfjb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gqhrqdenz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gfdojdlke.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdwoppedw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gapdptrwa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gxtnyhxun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gukgubzwd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gfirwqhuz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gfshgepab.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gyglfbkeo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpxuapvhz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdyxczrbc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggqcacreh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gzvhnrgva.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzqeypnga.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gmhzhlcla.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gixteifke.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gizxoxppp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gfxhtadgm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqxfmcxzn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gsicihoyv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwjdzyohk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmpajwbcx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/grymwlfos.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsllgyncc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/grlcdifmx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggrsxlqhk.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbcqhjjha.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkyydheun.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gbbhlvvis.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gqfbqcugx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjkzzcsjq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwwunqsrp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gmkcidgit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcjhlxlhc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gdpscwryj.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gopfvbbax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gvajzfzmv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/guqfazzrz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gthiaxklx.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gzsutkgzj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/ghisfmbxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gkrsentko.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gespqfjbz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gruijaotv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmzxgqole.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/griaoycnw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzxnnypas.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gwfthyndj.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/girgxepar.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gzzlhjnau.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gsbpyigjv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/ggvcnhipt.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghgsbnavz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gaznxhxlz.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gxfjriagy.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gdpnpbhzx.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gcmwddarh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gwdkaqkih.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gytjhhmmg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsquctwew.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/glzsmuaei.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/glimaaeeb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gwcalkaxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gvmjhderf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glouazsoq.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gdiuamlbd.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gwrxnkrgn.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gkglvkfqy.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghufniahf.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gvmhubhft.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gtbhsfdbi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/ggandkpch.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/giuwxvxrd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gbdnozdoh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gymhrwkml.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gikvxricy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/guhiuywoi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/glgvlanbf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghnxnzurz.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmqbfwlas.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gihotdirl.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gnebmfztf.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/ggryxngaf.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gjgtallwi.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gyvydwfqr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxdzptqvg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyujwdqpf.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtqkpubgc.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxeasxoju.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gqilstxrk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gxichkndx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/grnylecyr.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gmtkqvxzd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/grcoolgid.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbqallxnc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/glhqksmbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfhpuzyxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gneytlyhs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gdyrqflvn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gerxihxdb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gtgfszaah.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/ghgyvnfid.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gwdzcbfkt.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/ggtfvqtwv.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/glumuejkc.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/grsdklydl.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gjiqxrisq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ggpohyxnw.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gwnjstafn.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gvymnzwpq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gbfhsrntl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gbdayprhu.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gwfspxkxr.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjaaejin.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/ghrdjzopk.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gbsmrtbhu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gsnofgjqo.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gnxxltnxr.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gljsdiqvy.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gffmmtgsq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gxgqxnxnl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gadqgtpzg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gouugquwl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gupgskvoq.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/goicxhvwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gufhcrjtg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gbkybpzow.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/glaputuwk.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gcsjdivso.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gioeedpas.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gjyzzszrj.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gkuieaupp.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/glkmzodme.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gvrjohrfo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gbccdlxdm.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdcfivprt.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/guwducklv.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/goxoyplcn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/golpdwjkp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gmejkmtiu.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpuantywv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwakemej.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gcenwytru.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gkunfiwuw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gvmwuwxoe.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gadpzqqjx.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gturoevml.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gmcgckncy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gptaecsoc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gtkbqqgjv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstqsghut.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/guxmggurd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/grddiuxdj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gmlolgaig.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gbdtblcsc.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gadnuiahg.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gvdxxrzpf.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gftdyjlqc.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gvwilwyee.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gfndorxdd.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gyhbrlups.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/grnwovszk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gxrytjrne.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gbuaomagx.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gswxhboyo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gskjgydvl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gmzywiyab.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gispnspir.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gxefoedur.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gjrrgfxtu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gndngiiot.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gdpzkhzqj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gewlxdlhm.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/ggfcvxeuq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/grdivzjnp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gxobmfkzw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gvinyzvtg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkmxcxfes.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gcuzhncnz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gjjawzzgl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gvmorxvvf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvafefrhp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/grnklfoug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gxopnsxcn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gshwdewlb.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/giybbbtll.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gdzmfgbtf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gmvtwswja.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/guqehumox.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gvrbwdygy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gexoesuup.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gclqnhpxc.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/geuwazgur.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwlaulhev.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/grhmlkyzw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmblkyr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/glwfoluwg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gwkwqscri.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/glkibjuuv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gyclquyhv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gffiuxveb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gzaigirnc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/giuxdzhfj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gwovrjipt.sHtML


<!-- 参考信息 -->