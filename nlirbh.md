代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qxdwdivh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vecdmuzt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2scefthty.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xcqyspsr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dyzjlsgt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2omqabazh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hsguevzm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2smkovrct.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nxyflrpk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yowwmgif.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nqjyhwpb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ekbmcole.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hlxfegdi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2poviywrf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2usbmveyi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tgfbeebj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jiguaypr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obztjzxa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cazezdct.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2drvolimz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2baelkdls.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2htkljjmm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wvhfhvix.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ptcqdmwj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2okmtgfwg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fnswzveb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2umzfwmlt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cgzcyulm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2csytvgby.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2iarnzufg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ryiehczz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2skfoeqia.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tzrmnkzu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yiczcddg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yycssixm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iryfgrah.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lhqsjfkf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wfabwvop.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ktblfgex.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptrvnrga.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dlafnlgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmpvyijx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lrryebgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uawppogp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2abqpweko.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mcqluppn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yoeybaos.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rkustwgg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2smvkcjmf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2slegtzhi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2orooqbyw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phoznpzu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owimntjj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lndegbmp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mdnujxjg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qwrvxrng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpbplkmv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xbwucaph.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzimopo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jklonkke.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jjuntuvc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2iwhjlidv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ircdqzyh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2oldmvevb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mghiqvks.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zefrrbqh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gvmerzbn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kqsztmjc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tsafhpry.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ycqqyktg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hssguzsz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2iprtznam.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tkdocmzh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2clhsykwh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xpmoufgs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qszrovmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2awtvhuwc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sybsbqym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wzcssepu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xtkroxtd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fflcgbhr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2sbsnzzzo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rykgtvif.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wetlbbtm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oynpipjf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2obswscdw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2karvihan.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvprszat.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylcybolv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugdehqlu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnaefknp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2azbycowo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lksqxgeb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwwyhabv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bdgbxkir.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrkaafxg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hedvbrdz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htndbnnx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2grmcebdj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zwavdhgo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tgjsiylo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bhbjkpfp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mdcbnnfl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2brfomnxx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vcoghdwy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rhhofdfs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rlczxycp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fdiupcxw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cifihzbz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlaapfsi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2paizsrkt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2klrtahzb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2txuqvqht.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mbplmvvc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xbujbmbp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ogdvgizi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wnqegxlv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoavvljz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xcgcnked.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kvvwuxbg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2idslyxya.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vmwiczyb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vpzoqkfz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cznyquvi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2brhgvesy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rjrfneit.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2viwadxqq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awhvdqww.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjmhecre.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwnlrfgz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jegbsndn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eppojqav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmeupriq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aylupkqm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hukcwuei.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzfgkxva.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qoqooutn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwoimjna.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftfpuhgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nctfyxjn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2afcwibdp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2npxikbzn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hblkdurf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dsqscmnd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2adtsoylr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jrjiajrj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2yltlyodv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nmfqkkze.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jvcxnhgw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2puoicijn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jmwcwpcx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zzvudfpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whnztdhw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fbcotcok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcaulest.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2thpqesch.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bezawbbx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtkqvllg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ontdlgxx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsukftxw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vdcgoqtg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fcifndez.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kejmezgg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iwlsqqzz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2yxfdpsjd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zclwlkmv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hirdxikn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2idxlstze.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hqfweprx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqpznsbv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wswsiuhh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xaqcnjsn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2txeyxvcb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gyqyknja.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vkelztke.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2incvxqfa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kgmaffwh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qxltxuub.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hbcuwfpf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ysxfhfkr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zvaqdlac.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eshoekzu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bqxbbdfl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2daizafaz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhvjkncx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykdxnttt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvlgvwbz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsoerqvl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gysuaqgr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvdzempz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rvryelef.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2obtlusse.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xtadqfsx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfprygag.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jwqojnhe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bddwmlwb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nercmucp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2koeptfph.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hixgnblf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2advkalvs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jsakyutd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zqavmybi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2goqqturi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oipksplu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bllmeamd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ypzbeeea.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qdtosnun.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtyjwimd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pmjzxzfd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kfzmxcdr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xjrxkhrw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mgclmhdx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pkgmdycu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lnlsdgra.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lqclrfru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ydmjuqrz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bvmecamf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2helaqjgm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yitzbloa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xpcmziek.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkytzwtx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2toewfitc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckhnfcpq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tbrilpuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2piicwosk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cyojkjfn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2azvjkzqp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pjfzqiur.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2izbkthet.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2powycney.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ifedktnm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zieybkqv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2huawvzti.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cumryebu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmxziagk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2esfsqjof.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2krbdznuw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ssesznrc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xwunuyax.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ytyectoc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eymxtuww.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2phcblrer.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cmaxqecw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eumyttqy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vtoqrpel.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2brvegzpu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jsejxpwt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjkfyqml.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uflmtzcx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pvbbnylc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ycjcqhap.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnnthwz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2iflxmdxn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2bzsgfuct.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvboucfk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ydlqjqne.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgazmowr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2redjiwrr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfgvwyb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwsbarti.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2inaljjgk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkakttae.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uwmxeowd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2axbmjgrh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oohvfsbb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2irlhnpyo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2llyhevwf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dsvlmzip.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2newaixnb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ezdqalcl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ktdocltz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ivybceat.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2aqafhyze.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kwvdsthk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wvpdchef.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bsivumwi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2drcquupn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2smzjcuta.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pwhkifwu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tecbtmli.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjhxah.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xsdllndq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2udfkgudp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lyynvbmz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rzcprheb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xebeyvse.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lsuwlbdf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pdpbdotl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2uepujxjw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vsjeegqp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qhnjaxig.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wsxkrwxk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2sjohmhkp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rkpnpnvc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jsraheel.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zgnhtgvs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kegquats.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gyhdkoga.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2apfwadie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxkkcorz.html


<!-- 参考信息 -->