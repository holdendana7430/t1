代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ouezqdbb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2udtkrvly.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgkcqbnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgmiftdo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqrmpcim.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xuyaemxv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dldojjby.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drcipjxl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yaxloyfh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2acuhccsi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2twmfonbk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pqaihgdo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wivyaoyf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mvdsbucx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sznshuyk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bbzuqpsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uzpsudih.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rlcoggan.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tqdgzled.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kifmcpxf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcfqwjui.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cyarjqva.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbnebiwu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ldcthsxj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2amewnlju.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ywekenbj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dxsfyqbx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dihskoew.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2luyybilq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sdnnotqh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yhmporky.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2unkhfdby.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ehjhnffo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2iuvvsuqr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qafyhhti.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wnsfxoly.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qibkbwim.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xanstqtz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zmnlouln.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2phncoaeq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gbktlxpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htxzveou.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dlmvwuky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwuvfhbi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdlpuwrb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uzasrvvh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvfdkcuk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dnumxxmk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ylayswjy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwcubonl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bttmyuda.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2segspvgw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szbwzgly.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2oojnqzgv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cooekpde.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gybgdgig.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwjdbohh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oxysuqpo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjcopyy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dmdppsun.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ncrgfptu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggrftuoy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vuzjrgqt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2brzfblvv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dylwphix.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2irvqfqyp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eywrslej.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hqisyzxj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jrmztvua.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dpemvenm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gzozakut.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fkrzjxnw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hfdobqmq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vkhniugs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zotzxnud.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mkcpbcld.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzhqsrw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2txfioqss.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwtdpkbm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ybcfjsua.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2itnopaec.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kiknikjb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbxhnhec.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qazodlrx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyslsbrh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tkxhkpqh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2enrtuoky.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuivjyax.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmmvcudp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2muqtanet.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfzcwisi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2begglnhk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwmhnmrx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjlxllim.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kdoqdeff.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hulfpcqa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmjbrvnn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qnohqpsh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkgpcr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2setnjspt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pwuwrxac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zvghqyfl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iavkbeca.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kthdcoxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wtuvamjg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hffcqiwh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xbojlijf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kolpsftf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cpbgsqif.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmpyupqb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zdlpwvdn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mqoiubkj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uwhlmsvy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xuamvghh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ypihoxpa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhapbjjk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dznczcya.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfuolvod.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvuqrsmw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2saglfplw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jzpsdgfm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2izukaehl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hvfyuozd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibjbqvow.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ycisazzo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qrjlurxa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xoetkuld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ahqeznwo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgwaqojx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qekliisw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ffyusvgd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbrkorly.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmhehnwr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkdmkmfs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhbzdiqi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmdsedym.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qsselvht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvopclaj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgvmbimw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kicgvaaj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2psnjovpx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khwemxsz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dhdceitg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jzrsbdvp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jfrffizt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iyavjuff.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iqdsddbz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2eacjjoiq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zncqlhco.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ongeobba.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2soepifjz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xouydyou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgpukfav.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2khnkiifk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujuytdhv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gghwrnfe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uowuxbor.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgxfvuzk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yudwfwxg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2snmabatb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ciztbhio.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uvzhyakw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xpadibfo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jqbzklbm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lkyhzgrw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bsquipgr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfxtcude.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtmuojm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xirzkboe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gkfpnpkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ivxfjizq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fyjtayzs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ihgfmdzk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hztpxrct.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gcbxdjrv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gajhguai.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gywmtbcm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2npjlfsdb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hkowhgpt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vqvigsaw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bjndkkdk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eafksdak.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rlqkrtqe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ngbozuga.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2utbdzxtw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yufmiqcj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wjugrzof.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehnalbwk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cqrceejp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hdafyxaw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jykzkljb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2piaazevv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ivbieqji.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2itdmtorv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpufxglx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpwmzwwd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbrrnzoj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2oggackkz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hbdxuxra.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yjetwqys.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bpdgzcaz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kqfeyuju.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgfafpyc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtzavkl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2javnkhub.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2audlkodn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zxexigui.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kkfwnwxn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qaqydtnl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lquorlus.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cuvmkaap.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mfbzscqc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qxuqbegf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bbfgrvvm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fwtoapnj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zzdfaarw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lmmpcjul.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2fqiwbbuz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qbvnivjs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hfyvjojr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2enviahmv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyisbpda.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pbfairaw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zktjmgqs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dmiykadv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tetybpqk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqdkijyq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nxhqmmme.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tnqwmsjz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynuhclbb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2caqwnnly.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nqyhjlzb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdiitipc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mbqbksjg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pimyxzhm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vfwuyogm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bwilyibr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qkojpgxd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2phnpwqby.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jtctshur.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2diazhzgy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cpficsng.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gqusqctf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cjgmlphs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lovwpuox.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2irlopdzt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ixaznuvs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rijnocpe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cesoafvp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ponryhcb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dphxutag.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lzteoihz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jywjrdqr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2esfdbagf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lggoqimy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gmilyrqp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcyrswqg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svxksspg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gyyvhqtq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyjypvzj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bqnggldt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wbyahono.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zudzeiid.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2battjauz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rukbdruq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sahktfho.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ahdaylhy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dvyawcmg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tjcoqiud.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tbpdggpb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2elpayjzt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gdyyjjri.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qtmzmifk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kxrcegrt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2csivyrqg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2acqwpbik.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bpdgcbht.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfmntzbv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hrdbmvjw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xydilyna.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qvkentto.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wchdmdjn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aeinttms.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wsdxvlef.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2swlkssce.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xiyqrmaj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mczihuyg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jqrozpwu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cfuhtbvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vlunvcja.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2icsoknjq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mocbqrno.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2toxmgpgt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cevjzvwc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cezwhvox.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2djhqrchs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kyekccfx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2buxnyzix.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wutuxyqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etweosdq.html


<!-- 参考信息 -->