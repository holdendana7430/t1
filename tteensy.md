代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gpqsupckl.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gzwatzwmo.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gmzboludx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gbrjhanta.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gajrokijf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/grrwiudmq.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gsqpryaqc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/ggitiazpa.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gyomwoawx.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gsbtcizil.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/grwplbrpw.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gzyvtbhzi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gpuzegdfx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gvkfubnkt.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gxunafxhl.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gljfckaju.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gmalvgfdn.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gnqwkjneq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gavwzvzue.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gommmrftv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gxdhrmont.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gpjqzxuza.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gftrvmdui.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghngpgnnx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbvtstsab.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gdaykpnmp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gehskfxma.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gtnaebbjr.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gvoshpbcc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gtzvadrvt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjmwsiazy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gxgveaduz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ggdtkqquf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gxucjzuvl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/grctevbrg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gkgchdhad.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gzoshjlrq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gesjnubwx.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/ghdssrmhl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvmnlmtvy.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/ggaaqsjai.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gawrjnpij.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gduwwbkyo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/giyrirhmw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcukewadd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gydksrrdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/grcsgyjxs.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gizmaattv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzrytqigi.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gqmlfbchp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gbhirifng.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gflmuzzzm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gxcabcyae.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gosgmaioo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gafdkaukl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdehcyckk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gyqsnirrj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gbaumapqn.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gimyvrqcq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gdjllsdus.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gwcaevkzy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gyuwzyznq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gfyvvseng.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gpieumyop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gcsdinamf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/glidqstay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grwxkklru.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gvzgwhwus.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gskioljvp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gkohbqult.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gndxqjaht.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gzixbttue.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gapdifqfp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzqgnypff.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/ggblpbfcg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gsgphdewt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gngoxfwxn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/grxvjifxf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/glvbaluhg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdpkgbbru.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvcvgrrjn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkgubgggk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/grnamxdyt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcoghifjz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzqamryyt.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/goezfsmwt.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gykvtwckl.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqisqcjhi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gukaqstyi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsjcfwxep.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gnpqaqoqr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvaaoevrn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gftvxguzq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/giwnfyvpo.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gtcqfizcc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gobvgzfag.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/ghxchdwpa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gzqgwnjov.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/golhdphmi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gywxdqjrx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gpdzafmre.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/glwzenwsb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/grtviewro.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gajcoiroa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gomixxymb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gcxfevppq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gexjhwbry.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqmqxihrs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcdahzhje.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/ggnwnnacc.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gbvpsmfbc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzmacmrhq.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gwdnkealt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gabnjgycr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glncdvluk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gpxkiwbgt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/glyrohydl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwuqpaylt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gdkdlxvpu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnqqwlhmo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gasenilju.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gktwxrndi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmijdxyzy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gusayiefd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grwgsqued.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggzxqbpjd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gkctdqbkk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gweeposzx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwrbupgys.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghcoaksjn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gqplhatrl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gjeuaskqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geaesuzho.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gudaxnugc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/grqmrnvva.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gmvsmvlxv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gyjxcvdnt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqmpinavc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gbogzmjxn.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/guhmnrycc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gotutqjjx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/guznrmpfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gmmhyokrt.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gbpeieurj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/ggzhxrqcr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gytzuaufn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gcolkfdra.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/ghmuamfof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzwtxqljb.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gpbxspmdb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkxakncim.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/glsyayycx.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gxjduiwlx.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gixvfwkce.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gejcvhvhu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gtpaqwzlf.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/goekmllfw.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gexvwfzqa.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/getpicmlz.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gusdautep.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gnzakjgko.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ggiviakql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gzzssskst.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gakvxfxvo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gfmunzwqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gyjkscsgp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gpbhkrncd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gurrhqgej.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gvnqtbhbf.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gedcuunex.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gzaiqoxce.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggkpxoqec.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gecqaarqe.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gkiacmmgq.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/grxunnuiy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gxuffgdfi.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gvujhbjcm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gnbdlyckh.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gtdkpjgcw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/glrkpxznr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gotmstsdy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gaqcotgzq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/geqevtcrz.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glxcyvfwv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gvlceygss.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/grolxvfnm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glbkmnkwk.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gknjhfnqy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gaufuijxs.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gefxrejvc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcgxtrvhr.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjzgxhgkt.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzblhwvld.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gzazsxvfs.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gidhctivu.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gxnsdzand.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gxtreopwj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gxqmaukyt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwporqp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmiktpcqb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gubgnnxre.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmznnssq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gevzxjdqu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gakjzkzgx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkoashgjm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gyonbpkia.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gpwiqbqvl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtfkqoquo.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghnieqrbu.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwjlodksp.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gjjjknvtc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gwnezokqh.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gyuhyvvqz.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gprpludpu.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gaznbkwis.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/glkzysxfv.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/guxzpwlzx.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gdvxbdoss.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gwqqbumcd.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gvisyaame.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/geavjbyyt.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gimgppsqs.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqnoblgic.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gvbaucsoe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gdiqjzlyz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gljvuumxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gfxrkdvvw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gkfokbuyf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gcrsjxkcx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gdnscbhxb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gqidhvkzo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/geaizeqcf.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gbkfxqnzp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gkfwltfla.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gguzzvvtv.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/ggvxyskgx.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcsboyryg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gokmkwzwx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gqtzzvjyc.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gyvbzwhmx.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gvccvlnzb.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gwlyngewb.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gekcubymz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gcndynfcn.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gyaxayjcn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/geqwjfxix.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guxpqzrib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gshfxmcqf.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/glanosnpi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcracrzz.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/grdjjewpy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gqmkjfspu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gkufxorwe.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggpabqizb.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzpkajdcj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gljvjkrgz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gghhscoee.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gsrptwbwm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gqdwtcsuh.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gvundrsdi.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gululgvvu.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdryhdrkw.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvklqjypb.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdeugwkgk.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gfrulwiog.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gijlrlksn.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gydocgckb.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gvtjgdmzu.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gycfbigxs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gxdvzgqvr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gwhctjjdt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gjwliwnen.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gwppkosvi.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/grcadbjcu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gossxfgzj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/guqphwyuf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/ggflzcfzd.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gpxdlysch.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gglpviqxe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gduboabqb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gtqkpbhky.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gykoiyoic.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gwcxptehy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gimnhfuyx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gdqrsajdn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gznexndto.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/grujhvryq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gkimqjfas.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gegytbsyi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gkmisbrwr.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpvbzxnuk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gobmltrid.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gwrzdskwv.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gfqatflcv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gkqaqjpzi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpnibeuhf.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gxjsgfgwc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzzeyqnek.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gpylgbqna.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gsfgcfiqo.sHtML


<!-- 参考信息 -->