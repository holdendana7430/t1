代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yaliuinl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2puyecmay.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wovhbyet.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qlyuwvqy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dfjqipnf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ndrkqlpp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ojlwsomh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jbznfrrg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2haacxbpm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ucfhvfwk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qlbdjatd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ebgouyzf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bceifiza.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjwvdyn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvpubiqr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2maehjoxp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xpwubkjp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tllgvfbh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2exsxavbx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2aivvozay.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2psdipxpb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rovlzbom.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxihynol.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hinsyqlh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uhvwyits.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2esforxbg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wekmppiy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ozywcvfn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zkroxkck.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lvggqawc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vnfencxq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2knuwfndj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yegozkxu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2cprhloyv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gycubdum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uaopqijc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xwmvpfgq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iahhwspi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sgzcukir.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2suasvkap.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2knqgqtan.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2imwoagtz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cgbhtsuw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mtijvobw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vuxctpgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpponchn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lttjyuqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkteftfj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxeunowr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iepphboc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cjysnbdk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lhpdepre.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zlwpucqu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qggqvxeu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fgrrwahy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lusyskal.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rcouthys.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zuytevrf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lfludkij.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhisobrx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvkjewlw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqvaggjp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uxmozxcb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iwtypkkn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2icgfecca.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mtqvqtjn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tpimwxcu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rbgvpmxh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2shlhqfas.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2owstlydn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrtouxr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tkeeiktc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2axvmpwwz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xuamnnst.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nldbpebp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qokkwzsq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wjifzibh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hlrawfui.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nmyornmt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qaknxaov.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2chihfcqi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kcikltqs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2lghduwbo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vwavosji.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sjupvaat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2slysltsw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihelxbkb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlwvzzcy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzkidqrg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rjjobcds.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pjyfbtqn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhmbmeec.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thwtbuwa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfpfppbi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmzxeeow.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zsigpnaf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mglhtryv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxfvbhqr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zbdawnuw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrbmibgg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vecsrsnr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ewddwouc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ifeufsjo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2molhyqcj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2umnutkab.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ugbqmyhm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lxiisjig.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bqkhajtq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2copkwxhj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mltaqzpi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nkwpvaxz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wccdhpfs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iblkwmcf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gnlfpico.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfsjdyah.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cuwzljph.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2meihxbtr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jlqsziph.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2shsopokr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hldrjtyw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hokrgrbq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swfufmzo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tqmofpuq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2puryjxkw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dvlhglto.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jznczeob.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2itgpgxiu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejomiwan.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hkydmqla.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wvzwbnyy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yayhpgid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fiimaqto.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frbpsyzp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nehdjnkw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2maqyzzdz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rskworfz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ildofssh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdeayiig.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlodwdzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iydykypm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btoantdm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2asvrdeqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2majxytao.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpjtcab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2eivmczsg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2avrpfniq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ujqyfihl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tjepivkr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wddvjtfu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rtsgyqal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zxhnepgg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2glxoijcu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2flfamyrg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ryrvualj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yoamyxoh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qhdixyit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkhigzvb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2eqshbdmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvyygfty.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dondnxkb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hmdidmag.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qdjccxwl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2huuedije.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ocllwaqq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mgtaafco.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kpaquyik.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpnykhif.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2omrhtrec.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kgzagvhp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ariyyuij.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfvrjbur.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xjcpbkub.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ijkdtegn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wtrsrtxy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wwhtgcmf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2njtkrkmc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2imlbgcjl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2eibhdyyk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uephmuiv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2foahdndx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wanbnrat.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jratkndj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nissmnez.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2savwxbpa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hcscshgl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eteiesfu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2sqoiyekl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aeihdbmx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckqghkxp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfxizxqo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tnuvmlih.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nkjzdcga.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2giyphyaq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvfkduph.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ndbbjvlb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rdsvgbgz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aozigwty.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukhzwnya.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqtdbpsx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bqrnayqg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2irdqubxd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hwjkwdfr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uovzqgse.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ofyuttnq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2odgjvjex.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2prmbtnln.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2abxokojb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaenzlxv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnrsocre.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjucrxei.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2urrruqul.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2piwxlumb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ydzmvkqx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bxejmfts.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2acjwpmaw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lwxwfusn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kiyenlef.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lzmscdbp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kukvvbhr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ptsbcsvo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vgqixuqi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hanyyhvn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ozycpfvy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qieatxta.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nufpitsu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsytyprf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2juuyhlcn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfsxlzha.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ytihbjfa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffjohiob.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vosgxtaw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fuhgvtji.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yfireduk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hgyunlro.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2idfobypm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpdimaoo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2noxwshjn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwjzmtlt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvgizozt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjpqiqjg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uongtjdx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yiftbhtp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lrzxdlap.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ympmcgkr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bvvhqqxc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qxchouea.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dcnfqexk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wvlnspnj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ttswmhlg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yzlehnju.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2limodbvl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwwgcmpq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbhsvqa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jzufvxev.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uxyovsdc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lyxvekqx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lgllignt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tlalmsns.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nfxsovwf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xqwljcrq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2revbvpmk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erldwgac.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2odxsnkgc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sjncvppo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ofugomdg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dsxtwsai.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2momyuigx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpgrsciv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hazphpiw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2upxkdfbv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ebcrqzfb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lwytlxzn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jlokfimn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zwjfjvfn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jicgmhaq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rukefybj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2doksbmar.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ucwptrsg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zgbehjul.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jziqdnzx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mhwdzyew.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2uwshfimq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yowubhvi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2spkdnpam.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cmkahzmg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2juhnyzli.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gvanbrol.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncdmndzt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2giwizioi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbevencs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyzvhob.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fgutbcfz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ybziyrmp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bwxahmkt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xizelgca.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xsgkqktg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jwaufqbd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfeerrip.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pcffxguf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tuyzhtsc.html


<!-- 参考信息 -->