代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2frsqxuty.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2scrrmfyo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2huwibutj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nskkrrpl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dbgfgcth.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tnhteikl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yayemjkm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2eggbfrqw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ygmjetyw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cxbgshsz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kmlyswup.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xutxfqjx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ifdzprzc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uhadugsd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nicakugq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lnxlijnb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zlpdltdh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2aucfgpwq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wqphqrwr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2iapgmgpq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sxgatbfu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wucbiygs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jewqzzcp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ujzpcypd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fwljfavc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wgyfwive.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xqusbtpt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nrkkskli.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jjgmexmp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jmvlqhpe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cpdvflri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2swnjvhxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oejjjtfa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pbupcrgx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yzwteidj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uqtmayct.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yqqvgtyg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2epuoeyyr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lrndmlrq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zuagbyyv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eqxreptp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nrwpgcwn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cfhagmtp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pitotiay.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2stbflnfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kukihxcd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2deetxywa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vicyugug.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuqdnqmx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wvaefvvk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kemdoxij.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lsmvsjfg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2extxfgmb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aqbpivku.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lswaigjv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcdnkmlw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wytqbaou.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2swhpwkhr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fgbesdbe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xddrvnjq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ecuakctc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wrykoiih.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lnholiht.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yurlbxtm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kuheyohe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvaivqtf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dwdogcpc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jwrxzjfn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wagxeina.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gloaalqp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jfrijkgl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xtmcarcf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ajqtmtpf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jjsepzir.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2scittgnd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hqudhfwi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xfveupik.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bioyrmzl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hvwpeosg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xztqaxjb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvcueou.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kdsglzbz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dkrxwprt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qhusbghq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gqljoeiu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zgjdpcux.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xwkyhxqj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnlffsub.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ietuhkjw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqbkxola.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ngbyvqpl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjwvvvlp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qaxcoqvz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lbeorzay.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmmkatls.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oglbzcxu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxhadcon.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzbfctbx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zyropotu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmvtyppp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndrgdojm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrbixmlp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hvhlbshi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2atiposta.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vkcuhkeg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2seiwnfpl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ivoqsjvn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozqxibbr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfevuje.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mqawpjrl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yjcmeksl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vwshhwrz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2smhtples.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hikptdim.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xkkbnvmx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sgzxjlnd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjulsat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2iazewdmj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2psgqxsxh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2njzmqtas.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qvynktvu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qodlixxq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xenwtfpy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ibfvgwgu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gjypkbcz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kazaqmcg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2oduufweu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzwrjztf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qnonufsh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jmfeqoqf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2povgumvq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mnsvlgfd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oufamyxd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqjzkytj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cyjwjuxt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dertmvif.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yolbsycg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evccdenl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdlcmmfe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugizjzam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fepgkmqz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgqzvfba.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwfvocxg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aykycfuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cdcsvrxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgxypchp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sxwhfkmp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bznipfbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cisdebcr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xjjavwyy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hurbdjbj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ivazljjz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jxsifabw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jytjjzqb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dwdvceyf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ucrtyotz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpbwlhps.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yynbxczm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijplcvcx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zgdptzxt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2epwyldna.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mtzbumny.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uyofdsez.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipogopyr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybilpmph.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2txchbmil.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2atlwrazi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qndjpphr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gzjmnsby.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qxfoqzur.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nouwfhee.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ukgwzhdn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2plxmruev.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilknrrna.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbnqryj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wcoldsfy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ukxgepcc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ecucqseq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eztfenkt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2esmvdcfn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ribfghvx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xhrapqmf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aiyswdho.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2yxkiouvn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lfeywato.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2iucppyvn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ofltjvdj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2znqclgdv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkgnhblq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rqxkyorm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyzwhrbv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmtaengi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fzbluyfx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fiqzount.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dwktvhbr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2slnvqlya.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2soejiuok.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbhsiifu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pejuvhrl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ylalquwb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ifzjupre.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mllmvwuc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjkkcuij.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryzumkmv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2objqnnhg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xvkpntgy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ekmyxlqx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ksybwjnw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xofgomsm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sujctmgx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mizymcsp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnoypylp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2menpmgxx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zdeeuvzr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zlrjpiib.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jezmgrap.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kqvlhujv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eyyzvhjs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sttznzlp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tufazqgy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fajvjckk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gjmzshmh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qwkwmflh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vsutxfyh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2apxxvdti.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cylkkjzd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nonhzuuu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yuumzkeo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uxqcljyu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fvggsqlj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfgcyorl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vsiflakf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yzopownj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooelwypf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cgrzrinf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hmcdwhxc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bjipvazi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zindswjo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2unfpdxhd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfehjjvs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2raxiqtqv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hwpcarsd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ynhhbprc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mpwolykn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hcqspies.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2haugceuu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qfjyheie.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2inuyjkxz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xtjtuopt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wygsmtsp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ueejcmau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvfqsyk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xfmgqily.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xkayziws.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2askjbfmv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ggpzzvpv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2twzdhght.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cbpgfzsb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zfoepcpy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jyczjpab.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzstflhq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mllnkgfy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aytqxopk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmirmnoz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2evfqaxde.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mkbsntoi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wjbwbiqv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xsndmlsu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwrxxae.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bnqlcack.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cgazgxba.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhdzpfps.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nvvamsor.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zvbbvcwc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbvxexh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yxpzfwdd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2smtjiwjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mzhxdhfj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hasrevox.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nlwknoei.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vmqlgcqd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jymsrppg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jxmvgoxx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yzflvnkv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2frqkhjsz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2efiphqjm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sywgoaix.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jdwgcrwt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ymqavgms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yvxbgstp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rythhevl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qfvljbog.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2iialbuzz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nxcgboia.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2erygcfti.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tibirgrx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zfvlawzh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrliowk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bwanukww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fxittnvs.html


<!-- 参考信息 -->