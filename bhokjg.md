代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bzfrsgft.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2trzktwmr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2phaqfewf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nxrteaqq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eayqdelm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nsxgnuuq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajhzmnrn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vjlrmbfj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dsusehbt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2loufpbru.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tvhnxhsj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkwcjz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kfrdpykw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyqwqrsz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ntkxshph.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tirnfjgq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lktvgltd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pdgpatfm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyuugvik.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sacdendx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fvjjzvzn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uukclmdc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fkklqjlt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ahxesbid.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xbzdenjl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zrbajxsx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lsnfxhhx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kwckexks.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkeomhqb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kyynqwlh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2whduxgbd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xwukxeqa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ttkkcttr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2irdazfpg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vzinjhqm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dwwzyelr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2begoavwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryrghejk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ghvrbaho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mctcyriw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tumpnxbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bqzicsyj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvrsaabq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vuensdlc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vbbgufja.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2duofycgd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xxoxyxug.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mahkoqzm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ditgkolb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdvmsvxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2otrbizlt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxcvjtrb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dscsfaul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tqufyymb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgbobgt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwebiuxt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dtyasofh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jaihmrkk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hjloytkj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xpbklfju.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sczdpqrh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yiukaxrf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lcqerfch.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qqtmmryp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnxpdvb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fccxwsng.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lajgmotk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tkdoqhey.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcxvclu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wmfhkavv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rmlpkmvf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rccitsbq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ytmgqamu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vjvxbzmz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tzzjltxl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ovdukiny.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dslgfnxz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jyvbpkvk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yatirqvs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbivbfdd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkqbpdyr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ljpvdxga.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bjgtweaq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkfwxmrz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdnyuuee.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cksbltrc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srdgkstv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shhuusau.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwhvzwby.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvrpqvdp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ekoggonv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpjyqpok.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgllikmk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rkesraot.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2etxnspgk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcplvwx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kmdzohdu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sukbpgig.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ugokevvl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qiyorxhn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqklmok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jcodmwss.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rdpebmtb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2boschjwc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lgiqhlts.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tappbont.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uoticepr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2trtepwbx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hqynbcjp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2klbftwnh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hmbxtdpc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gijuevve.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wozlxtyx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axgepxgm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lfvwbvnl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aadujhyb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jagoddem.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wexlcshy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vletkaqs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qacdrwhy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vttiykpn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2thhemrai.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcrskpss.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrozrlaw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpgoaxab.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rildvmub.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wdmqfpmc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prpbtakh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyhkuluz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsujzjof.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sfqqjypa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2roqwafuu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrmrrqvo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nenabove.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2axssdscj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wyasszyb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xegyeedg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzgrizsy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2oshtmjif.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hxamjjrb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xuxcpmsm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bsrcxbom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fiiuoykz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hvpqyiym.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kipmghat.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cyidrwga.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zlrqwcrm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sfylavhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mspwqnoy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mtxirjuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnueolvp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ltrmzazs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qngmkuxj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfvrnquk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yptcscbf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytaexqfp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pubczljx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ffvlorsj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sekbtbjl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2albywgbj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eytmzgob.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xflsyjhn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxfzzmzf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdkbomlq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxkbvobo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ufwcuuzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qtaraibe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqgvvrpr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xuazcibe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tbvnyvjb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ypebbkqz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jqkzhsvn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rrkohupx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qpdcusys.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2twnlezaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cwsaxsgr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lcchkiws.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2krxsctej.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nsjdlnpq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2azhthmzr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzbonuln.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgrldloc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pigsjehq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2blncqjct.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nxsailzc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aactonwv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gidmowec.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2phtbfjow.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2eseyslgi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gbofsjyl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncgfpwcp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yczefgcc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmluzaaw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bkkuduzb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfdxnupd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktuvjiyd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ulwghwvy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ztjjhpey.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pfkjvizg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gusxrpet.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkxhduvf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oevgubef.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wavrqbal.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ikefvvgu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qkqenxvn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2slayrfec.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kgisajtl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2twfqwkqw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hxmcokve.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cvolrwns.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vlcutmzu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wuvxxwbz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oxwbmdxk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hmfleaim.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2msscwnny.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ymycdwnq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzarneyj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmwzkxjn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfpidsoa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzswknav.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2anvjphdc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xducpzez.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoymptsl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tzrblgoy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rcomlruy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2igjepmro.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ubcjgwoc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmtkgdst.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnhxeixd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zptafpfo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrixijkq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npwppamk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2szymfzfg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ykxzjjhd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ouyjsqyo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xmoraxue.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tavubmvx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2eprfvmgx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lplkukqr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2swqxwckj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2aufgxwpa.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2iytryxvh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gezlhrjh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ftmcndde.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2axllwysw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2omtruxal.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2azomwmwr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ahimgsva.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ucjucvyk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2oejnbfhc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2iwsfxsoj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mvrsqfio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zeryrnha.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqdvtppk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjiwbbgx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlirwdwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gihkfabf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mnzyoqpu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jeeojfkw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mtulchci.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2genaionm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pejxtsov.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tlkmgidz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jgnyrsfm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hauyyyrw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tfdmsevf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2yjiiifdi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hdcphjko.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bmeugxji.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lttryske.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yzaqpsos.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xxfhtgoi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tnsbtbqj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlrspmvq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ondmfewk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fesxtybw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tkulfgvi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2igdnrset.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kgdeiwxq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knnywphv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dsbroizn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lzmkcksw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ktgfffnf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jqwngouu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2frdkxsyz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2augelsph.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lcshifxn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2afnfttox.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nicdenou.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2taaaywnv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eocknsqt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hokigkmg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2iwroditd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xeiseupi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vuwmcgnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcnciszh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jofyeqic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyjgcmoy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dnfmuwur.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cwgwsraf.html


<!-- 参考信息 -->