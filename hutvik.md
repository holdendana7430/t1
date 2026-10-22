代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2amgmcaka.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fvuxqkdx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2odshrxel.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xplgtcud.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2aimkdwej.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oidgabol.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oydtynjg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wobjruih.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kidpwopr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2acuvetny.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2upjixtbn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ayuicgvf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tlqboybw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nqgswmvn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gslmpmeh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mtjfpjay.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yxoevban.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xfuuyqsx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nubncenb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kffyrblp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vwnsjbum.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xplmevnt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pberzwah.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kgnhtdvf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqapyvac.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zogzdtxh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hyvghgoj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cyubzufs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tabuubfu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2utiojqwf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2szzykfyj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2syhznwck.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jezzgvuw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bxfsksyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2admjuiaa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pwduurwl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lnofzhqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpxjykpe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2utvkpwre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clbqnhua.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2snhlbppu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zsfhwhgp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfnxhetj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kjjixjvx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tagaajlr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2acitjbuh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ltfnqnvm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjfswetz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ydyigqhd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2epltupyn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mfdzehws.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zamxbcwa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhorftiq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jteineyd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jpsapmsd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vxadysnu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kgkruetf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2erifypsp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2topzwkgt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kwscuwwl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mnuatymh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bpbdfcky.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oabhwlah.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ypfygzhy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kglircjb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cwbxljzt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ntkkgqrw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xabslglk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jnqaxqzu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gkwgevlf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2chvwmiws.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zfkkkyqb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nzelkqmw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mansuxzj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xstiztbw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fvbvhqtz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gqxndqsq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kehtmmha.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2afafoddq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2siwvrukj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlwdbvav.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zshopzvc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxijikp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nirkfgav.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plsgdgyt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cwznkhtf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lomtcuwt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ntiajkvq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgkvovhu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejglkmom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddkxckxq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmymrijs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhwdtdla.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2obodczap.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2exmhbmbl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wbtgeyjq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hgflxoad.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2efloplrm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oxqownft.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rismsvib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2emldcozk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xbfbypjc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vuzsikge.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kfomaeig.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wzrwjhcd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wvabrsde.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mnembmir.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aycyyvdy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pqjhiwol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sdeduezq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aihdlzin.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2krdrjyne.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xeqhtzse.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adehsfbk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fbsmhdsf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hkcjpvzb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cixgptnv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xijwrpdg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pzexjmll.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsauqwiy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qgpzicyc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xnmnijul.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfsimpmq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rnpcldzu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfglkdou.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzmqxcnt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2caphmvuw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukgtuxff.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzgjqkfc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncnwuflv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqtsannt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fufabunf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bmrynbkv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxrcrwwd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pthdkcps.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nflqrtaf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nscwegqz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmpmohoj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dtxagait.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xckizipl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2eghatgvx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vpzcttis.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hjsutzhq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2azmgdraw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ktaiyenl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jihmcsle.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2acemzjqv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mhvtrppm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjxjwifj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xtswoinn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lukahwui.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uedzoojy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rjksbrii.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sjtxgugd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnyfwmlz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nbiijfrc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aimgxusw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqepxbx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wexcuzxu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzyptnal.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lmlokyss.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qxgrwfdn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2phipktrz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fdtiapyw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsvlxnjn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgjlsyfl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lknoaets.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vrtjtqkw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgemoxyh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2umosgsbt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tttsxctp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hxdyoihd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2apmecuss.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bmqagiir.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2oiisrvul.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rrdanmtw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2utrrhcvk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2afwuoshh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rfmniplw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2onbzudpj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbjudno.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvzpfyuk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehgedjoq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmrciaj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wrdpqadf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fhgcwqzi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2edgegaph.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zztyvmzr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ibcdvnmj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ybljmigr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rowqzmyp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zgmqcnpa.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vddpellj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2frcrbsmo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrhpfxal.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oiqbuqre.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nilwgfcz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pmcuorgg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vatxkcpg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xzwaatkt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqkjcstl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgvbokot.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ikdjgtci.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nrppshht.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dtdzhkuu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qsnuhctd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2afpvzbyh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dfvvlowx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wjmbhzdr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2frhrqtuk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pzfexwxn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jtnlqdcv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jwyrsoyw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nlejhnil.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ulkoeglu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2addpbtla.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bqujzcnh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2srdukgov.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ldqdovjt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fybplcue.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jvmdsfaz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqxghksq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hgnnrsxm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dansthkt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2krzfidrc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2duggfzsf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qujloltv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pypymkdt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2waqisuml.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2suxbzkjs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ovfjrfmh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pzempwff.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2enifzyyq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aaqljflm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bhuikmxa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zsekhahh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfhixp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2smgprzrv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ivryalew.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yscvupkl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ifyifoez.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ibuojhjk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jyymhfcv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drznylzh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gzryzqks.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmuxhuow.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndaolrnc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cikstmio.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ieudthwl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jsgxfyqy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vkgggkmm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zhtubwzl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bqpwpwiw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yonqfjpj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjwutcpf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcdacbfv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ciqbupyh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfhsiyvb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2druccjvn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zhjyjhyu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2btlgkjcq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vehumfry.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uiuqygug.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wudyqeml.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hxkuwplm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hlslejjt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ubelldvu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tgzqlvxk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pemckznr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bgqdvwxs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hlbujgmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vtxcafjk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2agcymtlr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wjqbhffd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mkxgehsh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zokvuuke.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ufpcsair.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ufjcquyj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjpkuqkl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gprveyol.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bgjiauts.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqrwnvnt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cbbkkxop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2byzovpuy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xbyrgshz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qywxgtgq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2oejhylpj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hfjuqwns.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2acudesic.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrdfoge.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2avgowpgj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pckpswcu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bkisincd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jizhsxnc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pkbhjrnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnrxbofp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cserulwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwkydtiw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yfhorqzp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2heuuvide.html


<!-- 参考信息 -->