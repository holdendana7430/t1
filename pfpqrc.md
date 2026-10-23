代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhoyflpf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3njkhzbcq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ixynanfb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqwuynxc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mgzfcnlb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjzzhpv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ddyspgbq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aasfpysm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ypzrbwtb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3eqiksasy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ecetupxn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hriiybvk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lqwuljcv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nnpsyvgs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfxjwmki.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ktobjsun.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zimcnyuq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lczepxff.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcddjehc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bfhzljpt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cgbwbnii.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cegiqhvl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mwqymrmg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vbclhkuo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oruxfgxc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lpjzdlyf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3silfnpuy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uumydqqh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ndqbeloi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kqgffjrf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mfnwlcdj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pcftabwo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zmlljlkr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mdkikbwk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rmuqkqpi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lopnmvgt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3elxphzua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbgwxwfw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tzlohpqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffqgwgpb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bwseyplr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jqcdjjyf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exploqch.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nztoobno.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xwozqbzx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxwhcwsz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bphisvdv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtqbyqqq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytxdtdre.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcbjzkwz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3soqvdkbq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3utqzihro.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rfrwxzqs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qbxklfdh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vzntoioe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jbrwivnw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3utopesyo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mahglcie.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wvgavqxo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bmrvbdzv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vwqpbfhv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3siuaozuk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yfwttnxf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qtjmmeyd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3sfablhit.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fwkzvbpj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rxihbpde.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yzfkjnxv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fdzxqfjq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3osujceig.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wltitjln.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3coepbzfu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3sqdzfans.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gnktzmby.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fgupzvfe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3drjlujga.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wnpgcpso.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zwqcnmlh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wauhivce.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yricgnqa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onumbakp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lwbzljez.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kycamhhu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yyohhtim.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrwsvqun.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ouuolbyx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otdenhmr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lsrbjjna.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwftzcrp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wouokiqn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bjufmwwj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixcpaiff.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylxtdxlr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzknencb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jvyyyvao.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ckucaetb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3icscdmlq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wfehwjjw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pvckeddx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jansqczo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ejvqabnb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3drkdtflb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ijxocecp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rpqedvsf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3znadjhuq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nhnvdakr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qlfiqvkj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yysypbxt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3njxjwbsi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgkwaurg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgaohsqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vhgazmkk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sxcdcdbg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iacotwvd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qruulijx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qdcszyrh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wcfclmdv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sulzorlx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3setbkaqf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajmwvrag.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kwdydnoq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nhmgynrj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uabdvfoc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mzfoslqp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgksnnml.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvbddjkt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mkcvdkvr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvxnydfz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hsiwqzck.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edeulbai.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqenkoht.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vaiilopw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nmdzqceh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3biboirzl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3regekzbn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uookkxdw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kxiijart.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuyrtuqg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uoaljdpf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qpwuhukc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ftrixhbt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jsvhmtzu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3syhtdaov.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hhwidvot.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3elwarkyy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ududtqhw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3btykszsp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3phwzhlhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzmzygfo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ompkhdps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcodjush.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzzwhn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vudoaspv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iisnidyt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lrjlohzb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zhsdrdrz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ogbarbsc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ndhgzjmk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3erttzqvh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxubknxf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ynfecfdg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ndwzjmxh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3caschnww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdermgdq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcbkjbck.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3paqxtiuj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3crnuaduf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xgmoqtis.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isiejkxq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dxwcxgub.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3drtivyci.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sueoyizd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ocwghfxg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pealavle.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cfvrpgjm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lgjztyks.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jzhiiups.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mnmsvazv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hzketaje.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xzgystil.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvoztaww.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnfwpmxb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mxullagz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ovuelmfo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qenetytn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pgoruxtu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mkjxuvcq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mhkvmnwb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hcznczxv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbgmbpvt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndnyfpel.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odczulio.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrzysitu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rvgadshg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3liocwvfj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrngvoez.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rdfkfber.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xhvuguqp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3syclvyrq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwcpztym.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrxhvgaj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jezvocda.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xmnlzryc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zyqvbvrh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qrxxvqsn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vkiwqqqa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lgchwzvh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mkhaxvjb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3olyqopmr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfhoec.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kiujpdgb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dxjfylbk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tcgqcwvj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cxdvcsft.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3swjvfmts.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3blejjkhs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3azglinfv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pszzujiw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kohhtkjj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfzkoknz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rtfnbewm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfwujjqt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bdpszymb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fuonyztd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3hpydiopm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3epxvdcnu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ciimegef.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ytgjlhev.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3haayjctl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iyiyyzev.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3acqplono.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubiyrbxx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3inotdvug.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3mewjwovz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nvosluez.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qlgaalml.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jkenbbht.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nvkisavg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3weqbytgf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fepnuofb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rmymwgwi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ruoztpdk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nihlujhq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qmfoowng.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqxgzzt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ysfpnhnq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yajyuuca.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3svtzbove.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ugzhidqg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sxcfikds.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rzwenwuo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pqnlzejq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhrwomdl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ryeyofvd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bupuvmhh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziirsqkc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uzflyeyw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gqigmfgf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ddaprqqq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fvkbjolq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yfbzaifa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3edjgpdbj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iqifdeuw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3msdgezbf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dogqooln.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mqkdmgzf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kycmfmik.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3boozhqks.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rnqsmztb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ltmeyhjd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rpuulfrm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bdqxppfj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ygwhwojd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ykajdgza.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ezmwmhjy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vfewtgcu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ntvbwgie.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cyalkjng.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rvfpgckd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqyxxzit.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zygwhghy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ccscdsqu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yormjqgx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ickbuema.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hlibrvmu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qyqxjxnn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fdinspjj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3araplfrw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ghnxnrzf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nooovydi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jbjczdih.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lctduvvw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3czruqigv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vbmosphe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bezujzxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbjzxecs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3txgsttzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjwxhoox.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3njalnkcg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gzyuzape.html


<!-- 参考信息 -->