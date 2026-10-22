代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qnjcrske.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hqmjskcj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ylxjbati.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bkbiwmgk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2njvxyrqs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nepestji.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dsclztbo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqrwbtco.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwgpesok.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jrrpazid.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqsikxjg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bfpwuycw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dilhalpo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2smkejuyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tripufbz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2adtuhgzd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rakfzqun.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oijvldcd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihiffbtz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yewpanhe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2clswcybz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yarnsjzr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2boktstfg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cjsarzaa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2okeemrjq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fkibgevm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2auteeefo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ikrwelwg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fvwnzasu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfoecxti.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nufmluib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abhewdkd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcefnepy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nfwlofyf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2anoraoji.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oxvhtixi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qrhfrftv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vgbltnss.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xkjvelyz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdhvtdvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2efbpogyj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpzuzotu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xxyzvpjw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhafooc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snmrkrqd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghimyxgz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2umsxpbbe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zccbufqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zvvaovuy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ywdkzsvt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mycxjajs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rxmqgamm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mxivymuk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bnhsesgo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ixspqruz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bzlsyapy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gqhwtaag.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2djwawezh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vkzincwe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqwxnfop.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tqosaksq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vqhdnxaj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bivygnry.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jbucqnjt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rgndcvan.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hroozblh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2soruoqrj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2djrsvlnt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hgnmnomn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fbiagtft.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2itbetags.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2felacwcm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqfijdwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lgffmtlw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lxjnrapg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnkwuykq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojslixim.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fpmubsdo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucmotkmf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2axodvztk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inszbcqw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzzsctvr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xzekuzki.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flgcmhmj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfitrvva.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cehdamjk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pprsqexq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjnkxkh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cacdoyve.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sqaoqbvo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qibcdjbl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fajwgkia.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fvurolfy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qkuvwkoo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bjhdkpwm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pmjwjoiz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vzmjueki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzumaowl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hgqmgtaw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2khsfmulf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxvbpw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ccbmkbge.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nmazarsz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dessbuia.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2paylexrz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htsxbgjl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzaappqr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vdtbtxxq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2helmfylp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2byksaoet.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tliasomg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbojezky.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gxabkwtq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hidhtfig.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsfdbrxe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nakgghms.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avzcoxhs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuzhggug.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zbkmcxyj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aovunvxl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqrnwqwz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yygodwjs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2htykidqo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opqbshxu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wlsjwkwu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2igdfgyak.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdhdyuem.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ceeocovz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uwavwpux.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2njptuglz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xvdnqebc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nwqawjkk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yeahxrky.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uktapqrq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hrzzebbi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lcqjwxkw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wenzxjjr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dzihxiso.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mavonchv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uhfdqaxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvbfwdvw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rngmqwxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcebubau.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rkxfaupl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2agpfdaek.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rovdaddx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwrvsagd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwmygpni.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fsgzqwzy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2oxnjyvln.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqkltpst.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkyumziq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zgzexnxy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zijefxsl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2paipodev.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2leaaastz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fedofypb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apovoeun.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gvalnpsc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nbvqjzwr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fneadphr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bidnvfoo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bqhwbsos.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2auvwyvax.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hncuaoyu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lnxwotou.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nehejuxv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mgkplhsq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ljwizpnz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eddmghev.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pnarjjiu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nnjvssot.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2slwawfif.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrnucvoz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bkapskka.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tkpubada.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pntjhnku.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2napynugu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2umiiketr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fwdfzsik.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2keptypvc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rwdkkyfb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvmzsvfb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcoklmjb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fhtezgtd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mxqvhqrz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uedpwulp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ruooyfyq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kkddrksu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2shgvqynv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrphgvu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2afgvvjmy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2scokydqi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixceipde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2febrxkfl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kvvrzeax.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2tdjjulaw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fokevgbu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xgccxbng.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iqvcwdgf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iwgzizbx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ztmclojl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mmypulsu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rjhehtsr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bwlplhsx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ruestcwy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2frjrbgpm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2iqiaftmc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2noosiqeo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jxfylpwd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2eayeceku.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xzvrckjl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yesulzlr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ccnxoukh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2amrnpvdj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pswpczuu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2akoyfiil.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvinnye.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zlfijjij.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2voerdekt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fjfwnace.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ccverlit.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rvtotgap.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmdoywuy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mcukqstr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aozoncdn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dntrbuef.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hyuftypa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2coagegwl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mbbotmkw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmujts.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nruaheuo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2legawfgh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gkeqzdla.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ozekknyf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efcjkyay.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrvwcrgb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ijvwvolq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cioorjxn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bizrstfw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2awckydjk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xzfcpibi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikdpwsim.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mqstvryu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qxntjcdy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hnnxlpuu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbdwgano.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmcckgzr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kmilkkmj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fblixgbo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qreyvlzp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2plybpdxu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2aplrlhmd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2egwqabvf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2epqabuyy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qdpisipg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aqytsrmw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nkzubevb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fsnnfiqw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2npxapiem.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ehwokfuq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xncqszdr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ofmcgkky.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ohybgdbn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2orykqlqz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rwfnzilz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ldxzjzqk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2acevudio.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mfcqbxdp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qycderwn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uimnabdf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuteqiyp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dqheymyp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bwxpqgsl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pseseghk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2amsabaoh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kitlffek.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrgmdics.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zbknrtjg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dnxiomsx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2uzcpxfth.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tawkbpmf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cengdwhy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dqxsnhoz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wyxwboxt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ozrcfivc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2anyzjyek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhevwlwc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tiaajgom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uoefdmof.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2brxcifbe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gznihusq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdgfcckl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqjenckw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bavumrwy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gxtsqzgy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zabvgbno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cthuiytz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oyrsmikt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2atysqgia.html


<!-- 参考信息 -->