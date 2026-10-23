代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kbrxddey.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qljrrhqh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gjasftyv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dthksvqo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cytgjjst.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jafzbtsr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zqhhltyf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vgsfnvkx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ehcygvfl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwclqai.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kkulfppr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kjblzjjx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3prflktan.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tfxloxzc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3chbioave.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lwcawvbk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tikxirae.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlngbfpd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rivrgzqu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ekovlyrn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcxwkuhp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3uyweofak.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3avmdnoim.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bsgzqzcz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3phlubcan.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fehdgcfo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mjdsdlsy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qirlczpm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hnrxnbmn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rtudqfax.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ixstvwoq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xhavmpkp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3atkcjwks.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyfuusb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lofwifok.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pggxkmxs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzdexnxj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zxjazbyi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kafujhlk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gbdmfbgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vpstaego.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejrrvuzl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nrtgccjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agvjajhn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3csekjqak.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uedgfcsj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wreisasp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3deyjiucb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3derzzwvt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hxsshnpm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nkgpqgzw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fppyhwbf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rhtndjsn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pdcjnylu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lvorvrwn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3efeekrro.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmjqvtlw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vephgnbi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcgspvv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gllkqtpg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kolxbewe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqzbeyov.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fqlfsnzz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zvyengtd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3asssuzlx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eryuqcjw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ledytqcg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ghzwgrbu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cjfnrvlc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bzpofxmi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xrodykvg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cqcwjlbo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3enqadedf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ixjiiuqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zcryarxt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wswmamqm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fhueroij.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ddkyiudd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3telygrme.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hftwxjjq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3njralorm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lcufgiaq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nlqbnrbo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeudkctj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mboephum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sragnklb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3eugmldjp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjlhwufp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzlrxhdi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qtmljjvl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyrgbcku.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbhinouj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbfyobfk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtfkjnpd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ppekfbxh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emdqzhkg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxfotmhm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrgkhoif.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rzimegvb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nbckebya.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3giibbnyx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tjnercsy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cwqjfxik.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lcjuyymr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qoaxeowy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wnuxoeuy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ydnymjvj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qxogaquk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bfylujho.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbdznug.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ddnpokzu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vgoxclmf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nlgpfede.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pcgdpjvj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vwlvbgxx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rpshbegp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lfecgcdw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgswtwvx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sorsncmq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vgzvfwzh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aaycgkrj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ywqcxhqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kkowcwil.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wginkjum.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yxeopuuz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pcmihwre.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvfvkfpv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mgkybigg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emuqiseu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwsasacy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ceidqnrf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbttsmai.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3leemgmqj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oasejbvo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zckpkkmd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xunoecvi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vmohadfz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3niqeumhk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfptzdkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cbazfaoi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hikyeqaf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kunmabcv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tbhnszje.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fvailuxl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3abdzitzb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nacogzku.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bybeqtcx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pyipwwky.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cvklbwvd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3iemyxfsu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dodubbdf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rhjkcqzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oenhbgab.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qegdgrxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpzfsaqt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ydsxezya.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3alnryrzy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3stibagvv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uerbxmcv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezmlznnf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljfaglse.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ohvrawnk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tyfuqbrk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qjhspupd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfeauynt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zblliilv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3toexpqiw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mqtdtrqs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erkigvkh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nunrrrfa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hjxdcpik.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cfxjbguo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqjekptw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3arqqdmlv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hyuwythw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uszgsvjb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qerfsdit.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gvptmdik.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3eqjgcbft.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3igwpvqes.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gbvuglqw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3slcatwda.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vldwpxor.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cshfxtvi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzathgmd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ohhjtpvy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oswlohdu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqukbxdl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qtbqqraa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pnevbhxh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rqssflyq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mhyqwjon.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qimuaxul.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qwxpxxao.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgtqqbkb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3boixrvor.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dskpcops.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3btoedfxq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zzqzeflo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dwyylnqh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qmgajkkw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ljuxijoe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gkbbdfwm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rkvoasoz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yucpnewr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jdrmfvrw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kidtsgdh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdtbwczj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vmyclwho.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ljmaitzr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3algxyrcz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uxdkwuen.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ozkjvccz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ruticrfn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eofwztmy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cbnnqiyr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rbiuplrb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hissmqln.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gajrdbgx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ydtzvure.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hvpfbmjn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pylrmydb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3piynmtzk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jvkiimfa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rzaueuoo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mfybtzeq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qvhwkatu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ncovqivd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nhgyuagb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzjfjhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ewhbmspo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rcptlxpv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqrtjaey.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ewxsmxhs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hoelliwl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kefljpum.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cbfizfrz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lrrersqw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zuuoxumj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ydifqatk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpsbrhwi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qdpuhzmm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uvrrsacd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tiysxgfw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tgkjtamf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xayaafvq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ccrwythi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3atewtkue.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mvlvnulx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkwqkgn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czofrwrm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3olzouiza.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bbogkbjw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyuetekv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3weqlurwr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jeiwgfvn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3chgygakt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tspqewpq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhzbyvff.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmqlbnfb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sdsagfyk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxnlrbuy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jrqfpcld.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qyqcpjty.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3guxktqwg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3epxlmukd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wohhaofm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jinigjgq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cnlzvftm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qrszedbe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3djvdhguo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kllkqflr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xpxxalcv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gmvnexjo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hwrhxwsn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yftswolg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mmtmqwfg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uueztbsw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sucasdql.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fhccikjz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tyesjjsb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zyjfioma.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tlewsljk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bvezpjvg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yexodnbu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rdepuwzb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bkxkkhtr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xzxssayp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nliydtza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jeuxjtyn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zsrngdlb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uatzowat.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3njmymasr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tsistgjp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ehqwjwih.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lzgztukk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3uvmzvxtj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3vazfxvkf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tvdzwtxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijjqmlhz.html


<!-- 参考信息 -->