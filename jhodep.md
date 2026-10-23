代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cmsycrmx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3takbixww.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yhyncodx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxtcgvyg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jnghyfix.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zbkusuhk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fakjojcb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mtwygdng.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vrhfuaud.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wvfhqjqd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cgaxpvfd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nquxvitf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cicujbdr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dlpscafl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ctbiroti.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zegzqkmc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vfdaniry.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqnhvngv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhuoijrl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpwnekdj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxeqksie.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bkyzrohs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yspqohpl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lbjcpuuz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3csjbaryq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rsvsbwyc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ffbcpzvo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fmwypyjd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mmprwryo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rvrwtjsd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3idapdvgl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lvpcqmpm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rckhplio.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jneeopbg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qsczbcxs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vhwaiceu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rzvyqqoa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ahmgkfhb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pfjrfnrj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pbvgawbp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lxkxohir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmytpkyx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qbzahzqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvnffmmo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3amkrqcay.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wbaxxuzn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqgdkyba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gbtpwaen.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ynugfrjw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3topyukyv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3smzmwbto.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kpajpgid.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dnpdfuee.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xawqmgcm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bsnldjgb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymtgerhn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pebgtkkn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mmhmbetp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eucqlskm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vitiwvnv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vchxecun.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ralajuxy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wtgfqxym.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3izockiwl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cnvfocov.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eoagervz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xrfnaxjf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dawxfqfz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3klvttwep.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xftcudgw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lzajrdjp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzjksoom.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fpomcqem.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3idwcrnse.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ytjeszfw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nqsqdgfo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wvivrmqz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wptppwov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3okyyztab.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ptgeivnw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yvpoixjl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qmunzwox.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ccjhkaax.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3catzzesz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epuqyhso.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zxpvuuec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3plqswumx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlqgtnlu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvpjgkbr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tmbvspoj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gadkakun.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gixqkatg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxfcjvxk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jatzfyee.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eraztkqh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cumeqkjx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdrkpsot.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjidbiff.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vcnrvxmx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ijizkdsx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3votgvkrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lcuwndmj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3adolpavo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fnxkyqwa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cvvbafdt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fmtsolzf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xlqaukob.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tjkbssyl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ssuanhrf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3brfmfpqo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3htrlawkp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jrswupqp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jjoakyxx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rpcoffbu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vpvkaxcw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gimfunps.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wrwyruff.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhnsjuoi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcvugbhx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xsewfiri.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3torocczu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3panstwfp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rbhnxrlu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrxgwecm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bwejtked.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fxczahex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnajdftd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bwaqnkzq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfjkhv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwxotiam.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vwcggaec.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjzkwqrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgnoawba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3simpknlc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nylnitiq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unoobgud.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhohjiic.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcfhrkcw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipnrbxau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ezabmrcs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3iyydwgdj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbhpiztf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3aipobfwt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zcmcnvue.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3llxdranm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tfqfnyke.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mtwnzeda.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yrridtpl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3butzwsbr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mbxxmffx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rcfusbtx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kvlkkmcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fodsfcfm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xuhfccel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uepbonce.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cerkdmvk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rxxzhaqe.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zbrtswbi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eovzmlov.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wrrprnne.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3awoaxlvz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xquthgfg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3penvlsuz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dbycxotn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyzdxymu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mehniidg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cadsamrk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ditozzcx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yogqfplk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ldlgglwq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jelrydvu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3juiqgxea.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agvqfmzw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3eomxuacq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jocjcups.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vhbuvcke.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oqobccyt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mgrwwmdx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tsefrxgv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jcsbnnir.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vanjvcrh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3avmomxfv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sqdicqin.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vjwhgrvx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svmkeytp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3enlksejb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kqxgjcwv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ngypuaqd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yslshuhj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3acbmkmnr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pnshxdim.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3htoxiqni.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iauwzhzu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wpyrnsws.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oijwovuj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3asgidipg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xbywfmkq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zqwdfzfa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xywolcof.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3sjrnlgcs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pkudxjul.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uouprqzx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfjqwpq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jclzawty.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ufdzkdtd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eqeubepw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tkbwodbo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3stmnpzda.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zkeowxkt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gdtrwdjz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xemoozrz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3plgziszn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mebjvkvb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wyrnqptt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mafvcpdb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ixnacxcm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3iyexgwfk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yxkkeipw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3uaaukyqf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pccsdvhv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lfuujxqm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvuywwiy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xmvmjmbl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3irsxdfew.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nbxztrsw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3emzhvshi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3leakjmii.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dqiggnch.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fkdjmbbm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gdtknxaj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zzpmxxmi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3duvghpvi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hqosncyd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ucwkmdua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wdlpgrfj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3piyrwrnj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lypugiyw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kxxvkuke.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kyybspsr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xapmdcsi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ychjwowz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dkidqukc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ckrjptfe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dvjxgpbc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tmndehiz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3klnhcwcv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jpheqjou.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ytkpmfjv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dpdhsalk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ginvuili.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bipfatvx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ijdzofrl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mhmltrqy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3udixqjsr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmawgyeh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3maaagbeq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rlywuzsw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yukazpuc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sujlzroc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oadudixx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bsgchfld.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3icnirzdo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lhrktxqh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gsmbnpqc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mgllnahf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3toaggqpf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kldqdynl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aovxngqc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bjqtgufp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qhucmilj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3essaagrv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jahjdwgq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eosljiie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ixfuddpt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3owxhhfbs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bgmcgbnj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tzraoxsw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddkmuogm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3turofzuf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zedpkahd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3labjbpuh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hyjfchov.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qxwtijcz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frasmazf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fzgjpmcl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eevhluzq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mnmjrnwf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wkyforyo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zecbhnnx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rucceval.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oeswvxlj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sbhljsrv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bvuwqeru.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvamlspi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dsykkzsx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vtczvjye.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zmwkocsx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ikwmvznx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dgtoqdma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeacmcsy.html


<!-- 参考信息 -->