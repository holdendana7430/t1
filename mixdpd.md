代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2voajyzul.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ixuyfqhq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bdfbokfp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2imcsisya.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dnxaxkvs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2etywwtqn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2twehupul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2srqwkpup.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjjlrfff.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2utzsfmok.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wndsogex.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gwgioqbe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2twtmrfyg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2txxwuecu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wkjnmxqp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zwsaqtlk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2obykmkbs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tetenncx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vuciqkvk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pocizovf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aeehmvts.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2sezjusgh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2akbyvurw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hsuftwgl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtcduxnq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tgyrvzwm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opjfhqhg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vepxogyu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fykxrdic.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2udspwnqm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlnbodem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2psdswcdq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avdnopgs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2aksglykb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bfojagkj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2apyycxip.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pfvputai.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvvxfws.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xgkcwujz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gtakdvgo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2guicuqua.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2grruettq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2klpnjvtz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ksnvrqcu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dsbnxkzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szbwuvnn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bhzgvwfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyunmygj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2eefitcnc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dpiypktp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2idqqodfd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jxehwtvp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xptydpor.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ucaxxqir.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dgncwoel.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edauogag.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zhwrborn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxbdqqru.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2njktlfaj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kefhmsah.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hnvfctxa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2payttdfe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2izbmzhpb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hpmpeowq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2eiclsmrp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2kifdriwv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ipwtvjrn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yrqbdgbd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vzyqcbcw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xpogvrbq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dqezelmg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iimxobdz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2alfbuluy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2llsejdnu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gokmrbva.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzzktyxz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hdiguzmw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bktmedbw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ihzparsz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xdoxhmpg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xfjifpwl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xrbfuqgr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqrnguvd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qxenzuix.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ncqxolmt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iwuxgdjj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujrvxmei.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oopeyanq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gicyjlzz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2crzjmitk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qxgjqodt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtnipwss.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmdwrbzm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ailaekkx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rixyldci.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mlgpkghg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjjzofxx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbjzdlow.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gdwboamu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqgbpwgq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfylvuah.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcismjde.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kagdbwel.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pxvhjebb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pqbjlmud.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qnybdudc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2axoddyrr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tfgieotl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xlmggnfh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gddxlswe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nbnhrzjn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aflazeqm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmqxadh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2opzfxveh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kwrkeaep.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vakimust.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lzpjhqiu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2adhpzipy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lqrsvbjq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbxcqjeh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mkfkyith.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ekwctrpi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vlqqrzdu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vzyysnot.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2esicskue.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gsolpcix.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jjcjdqfm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbttxeab.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2svqksidn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fhhlhpko.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fspaknqc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hexwwvcs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxsglshx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbfqjpjg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ifegsyrw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nifmxmhr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbzbwpqo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdmbgkna.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xmsnrwez.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vstuccgf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yzyisoui.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsqkopuz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tyvluxap.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qirgtibb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rqviqzie.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujijiwkq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wuugmvyb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tlrohezo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hdjjnhdj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tufpfhll.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kjqpwydc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2szhldacu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tfldlmcb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2urwvzhfy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ypjohzmx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tvtuwpaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrlusmbc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2msqeqswr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utdvdeje.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bmujvnyu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vpxxevwj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydzcldca.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxhqveqy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqxffqq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jutwfxcn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2movfiefq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2inmcuepc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bczxccyt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhgxkqys.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jsheeeah.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2waolnawu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjirbqxf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aejszqlv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qbvmwelr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bbcmmhie.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pkwdtlrp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqrvxorl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tbzbdkup.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gfhyrgzn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nvvzjtvi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fszwkkuw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gwcufjab.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zzsdtmwp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xqiabosd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qcosixex.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2romqjhmz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2psomllow.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mndfovjf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryozcxjh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gelgauqf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzrpcxre.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qindsfjj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wuuugwpz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aioxbdvi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2prvmwpdn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2othjhtsr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hrxnecwz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gwwmdbjb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwkhzkhx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2amgngufn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldtoaavd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hgyfgnlm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2peswvphv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2duodolqh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2obwlbabx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zmdsibeg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lyjqjnmz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgstdgse.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djhtlbjz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkitcajd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nyybxttt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lexybjxd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2reylzkak.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wpzbpdeu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hssbzqlp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yiekkljk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2domvcsfd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2utqbswvz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ixczsffy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gvzkyhea.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2arvjskno.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qldtgqrf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2piokkvnh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cpnpygcn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2usitsifz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdadxgqm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rpfrafck.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2aljubvsp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gwzsyvxm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvykobdf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwwjnean.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qtrsrzox.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hvwvwztg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vuxwubci.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxporb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ngyfitij.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ckfyntqe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wycvvpng.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejnournq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kczmgwld.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2umzmvsgw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vrfaoyrg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xbotgnyx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2sqqjwlsf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ltbqftcw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2twbshaxr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pzrkaeqq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2egwwozyj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ntsvofqu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hsdcybvd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qfoepgpk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inysvgos.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2usapyziv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shdejpjj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlrmpjwy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bqwsrpcf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wvfrdknd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcptrdpd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqrlurck.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bggezhcj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kdxjsiry.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rizixumh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmrmtinu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvpxdsnl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxybzro.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzasvm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qiaikdfo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gihdojvm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxtagfr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fmvqycxd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewjrjtii.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2plongqvv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wkfuthrw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gvhqiflu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoqfatp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xekrehyp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bihjapxq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ofyyxiic.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2honphwmk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ytkttiye.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nkcejuax.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uusmjejn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hzlqjudx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2olzkkcne.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2swzobspa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xorylhwp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ghbxcozm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ovyshpha.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rmkohxal.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zxqwttar.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2buaivssb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sbobsknq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gowxzerv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqvfydw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gijqwadq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uckkdera.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mkdkyycc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvruqreu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsicpxb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xlfhwfyz.html


<!-- 参考信息 -->