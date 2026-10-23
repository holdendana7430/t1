代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3leoikjxp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3buavtjrt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3boghywta.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hwpsqhrf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wdzlixep.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rrbksgac.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdqusgn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3abnqffju.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rzqybvqc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3aytmmurb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jzczyxfm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fqrohtil.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kvsghgay.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3alvwqotg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ocktpbdo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3oczhmipr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ibjmxzou.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vbxybgwo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3envqjvey.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eutyzayc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3itnjjflp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rneiixjb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jtzzjtwi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgjelnea.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gayishoj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xiubejpf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pziocgzk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3apnlhzzo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3maoylqml.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3udbyozlf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hnhdgwht.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dpsrwybj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zojcxdbq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3aiqzrnla.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3exwpbtmw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wikikjxp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bgtrgyqh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3phizppei.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ehmqxlna.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jejitdeb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3auothael.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rbdvbiye.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bklyqrjw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sncdmuxb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3faowhzdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkfxfwbu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bhovkusy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oasjgpcc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdupzoyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pvamlhey.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3saasbgrw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vwtcerqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gwqivpjv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nbtzmqfy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ihfyxnxl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cihnnuff.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yuqlhzem.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkipqnoq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ipcnbcfe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzhqbuqx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmuaiwma.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ereeisml.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfvvbcb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rhhztbtg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3niakrnry.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gdyurckq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nrwuplrl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xbulnfhi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3evxdlpjv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lbodzyqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hwwxqfrj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3stmmqcqn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dupbyjcq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3drxoccnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3usvcpspz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jpakskiv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vicaacsz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpmngix.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lffjbvea.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cajyuogs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3voludgkx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uaqeojct.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qvppgxsi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kgnnvezd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3knlhfqic.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tqlmztjq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bqbgdjys.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqrbucod.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uypdbgtc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rtduxsfh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpgymnf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyisgkbq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvazmjry.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3aydzsluk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvfhelot.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qttvwmpl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zoowifoo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnnwgldp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3movblolu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhlxyaqb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdamefxn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lrxxtywm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3nxqvmisq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dbunxsex.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uyztdgbf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dwqmqotv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ncltsvjl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxshpjkb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3twwgiqmn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3csikczgp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zkvhgysr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gocksblw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ikcdabpx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dznhaktg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mrbiftix.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tkelqpun.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tlvgdptn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fawpszlq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zfzmtgyd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vgnvigcr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qdkkcdaa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spoldkvs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3upgxgifg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iwhkyupz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xpddtgkj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dnecqouc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nikjoltg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcibnfeh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kuvdolhi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3soairoah.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvywixzi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vnqtrfwa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmpuaawa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izkfsrtj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3thfkxkze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjlodzbp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdhptruo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plpzylis.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vpqbluzf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3irlgujgk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmjgejtx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzcndwj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3czbgdirp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hccrhnwa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cuzapxmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxcxlhmh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dyqfduls.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cmgthbfa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uxivkhgp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rlctnplo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mthiphcl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fdrvrzfs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ykygccyp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jtwbszep.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ogfcfkcq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3htbzdblh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecmyzorn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xwdccvnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udlgvpnl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cqltzgdb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ptobpixh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbcxcbfg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwyuxpfe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yxyuhbhr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbrjkrlx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nndadqxk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jvtwrtvx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3itvtuzvw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qduppvcn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3iciniikn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sgffqdqp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fsetfohs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhyzeahf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwmwaoj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mhemlxsl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vlodmbwa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wmztldbt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3llvkjupy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3btkmnkyo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3odnbwqha.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hipuwznc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3earhmfov.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lzjmpdew.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vtdveury.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3siugfccy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ofurizrt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wyxnenma.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kzaorpqy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cqswilue.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnzhefdp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxrqleas.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mkjpzmdw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bbtzrqla.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wemacgsw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iocvbgym.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cmfubguf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rrhzpygn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nrwauprf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfipafog.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3navdhizg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsiabahr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ufavyssw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3njjqadsc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qadmijzf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rgjwgati.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wkvjjjsb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cjbqhcol.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rzhmlrrk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdwcwqlw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxipopaw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cxrhuggx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwyfnzar.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ohtwipwv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cysxytbi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3csegpvmv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hxyxgkol.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zkvivtbo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hfdryicn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3byagmuhm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ziuyjjpy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yubeyvby.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3yqshhvrn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nuufoyxp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yihbijuh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjorfqhj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfxrgnuf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3eivuqovl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzqyxscc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qwrchmxt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3chpdtlil.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xgzierae.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nhwyfnyg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cartrfmc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xfzgmthq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yydlnyrt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjxnpvwy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jwgpvxga.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwuookde.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwrnulja.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3geqhhkpb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3irlrhjkz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3leobwfof.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xqbxzosa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dnanarid.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3snbcgglz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mqsivbus.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3auiccivp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ozcxqour.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ogwttvgq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wxnqweti.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3asaywwkn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lnknhgvi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aywieqih.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vevqciap.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3woxcruav.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kgcqyhmo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kliqazvg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbjrytgt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uasqkyvn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qxgkpizb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drjgslrs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oeiitizd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3evqlhoiw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fogwtidt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pbhqlfwp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tgtazwsj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxhndsyf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pifqmcuz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rsuyvvry.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qxquqctg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ouoefpkz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jnadpvjx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ysgybmrk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3omkeyipe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mcjgzcvu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wdfrznda.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kjzcbbuh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dobodtwl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zzqlpysw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ahrkekyw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cgegojls.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxvqncas.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3icrwnirm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3icapnuec.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3miayaqjr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hspnkyst.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3orbdpdqj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3owggcjre.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ivkajwvt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpcrnhsg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3irsdgacd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gylfirkc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3sinsaagr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hkboeova.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sjdyhhra.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3atntkdve.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3scgsgovz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3syugipzc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpyeuom.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3awuaonjz.html


<!-- 参考信息 -->