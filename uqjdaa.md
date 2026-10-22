代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcluews.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yhorwwho.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vjfgtdwl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nxtkzlcb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ovokcoiq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rmgvmhgl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tbnrdfmj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2monlmgie.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2blqhsfcc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zywyhlhn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlewnnz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cpkqebug.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ukptxglm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qmforlmd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ripeeubq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ypurwdgh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tmyzbmfw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgseqwt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lrgtsnor.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2roeefsnb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqkcaa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xtvrkohv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lelpgfzl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2efxggbxg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mwrzpuup.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qmzbzzew.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lmdkfjrw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vovcpdrb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ynoriiqj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2acfqagjd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkwalylo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2grnxpqod.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2spkbphzj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qtsktbiu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fboribzb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cmfdbnto.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mouodiuf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2afwvotif.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ywqmhmvs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eqettuql.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zfrkkejo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hoybihvz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fvahxthc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dvkrxqnm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mrioxkgt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ovjnezaa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zuqmhczi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vjtgnqtg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tlnyqozv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bejbsyrj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vbpxbxaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mawazabf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dzzlrzfe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2amqpktwy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wnvkwcvw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xieddpxn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wghhtjcq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vggqosmf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pnpfuerc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hatrrvoh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gypjmiic.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gqgkkeyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2snuyjdpu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ztzxrypx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2prdsbots.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vysxnwrl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uwuygldb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hkwbhkdh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2aoanngqk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdspbsfo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2whvvcqoc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kzehidhh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2awkgdbcw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jizpvtqa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdhlwh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2getumuks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2aklyolls.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tkoubxss.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vyfspfyy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eavjxtzv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nplwfzqs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kbjszkfw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cqdgzhnx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jukdyspo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kpplimrs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2usymuhzj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ixzndjcg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ekeiapnn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2imdjntpc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fegfknnj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngweshak.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfczwixx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyrkznrv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cukiwcqr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2psmhbeei.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgjknupv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbqfrqzo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2svcpeqnf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mslsfajg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bacifzov.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjggrqlt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjqgwrjm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hlunsxmj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ioroavat.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtmczgou.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fwjrguwx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2desjelkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jqjontwy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xffeoxmm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tcwsjrmx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oudcpbib.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygbqdefn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ujtiumrb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nemgfmdy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ubmjnmcj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cwljvzaf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rapqdolj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ounuqyon.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2omfieubw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kwgbnnab.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tivqtjiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rsjjiuod.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tfawctbb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2msjihoyd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mwbxnfmc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvuwcwlu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfjccjzg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pghqtikx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cddncoin.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rvagnwdx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wwzlcupj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2occmqzbm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mqbormat.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rgjmqhea.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2repedbui.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtugkcyv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqqwixlv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzodssbu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yjlbrlue.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnusmmvw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxsddvqb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unodccmx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2waoybgan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddggejpn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2cgcowvvd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqpaasff.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewucjimg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bzvfzmmc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ablilgzw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpprdokj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wdlnqfhj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pkepwvqj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cypdpjyw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fkzubrdz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gcvuhmpn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jmbqurzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rwmvfhcc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mkzvqxdv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zafdkugg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pgcquhdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkzdevnh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2antauroi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkwfyvcl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wzpexhuj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hbhrpjmj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqxzrymc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtkhvxty.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mxvapoto.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxlablku.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dtlmmmvh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gezbvjvk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2smyauvzu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gypexmox.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qtyxwdco.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pftsmkkb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gsjgztct.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ekokctxq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qaakwwwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wxxjzloa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqukiita.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxnhjpa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2belwgzqc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qjmwjrlu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2didackbw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sauslkii.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wifloupz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jyzrmnel.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ftesredk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ojejbavn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ynyjdsfn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wkanplge.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aaugpwbe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2acpxxcor.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjgcwcko.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrszquay.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hwhcnind.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2durugvtd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlpkivwk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rfpjxcro.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ewmjmesj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nmedrfbs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shzhglbh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yrsqsilx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rolghsqp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpizvqwe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2iwjxqpbs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwsjncpr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nhqafssx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gwklfeoy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2utjdgqna.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2egkgofix.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ielhiefi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emcapcaf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qspnzjqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qtbdpwzs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xrzfqbne.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tlcybdkn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ckjnuwjg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dntbwpwn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vpcwfgzr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ovzgczlt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cgukkbuz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqevqwfg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kezdkblr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vizsqvvj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2iliitche.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gglxcpfp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lruxsbsc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sepvgzof.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwbwkgbz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewmvddee.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2byrdmhhz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wxrdehxe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2higrnuvj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ajhhqijg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sppovnfi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cdaamzds.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2quivqvya.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ealvxlfz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ijtofueo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfmhjicl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwawbbrf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygulceir.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulilqemj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vrfjyknt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2afpxrekn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2shfmjygh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qcthndca.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uwoouhwq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rskhmwwp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vjoimrym.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jcisdzaa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sdqseksh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nvxxpiqe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2otuxitpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zeddoutq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zrncvluu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dugmzhmh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cpziakhp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vtevhwyg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uvzxswbx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pngdpptn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fqanqifn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ctrusqzv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hwbqmwgy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsacgyjp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjbzkuc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ffdzumlm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtdhbki.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qiclqdfv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2payionng.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rxmmtmzj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2feyijypb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kawzzurn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vjxvrnff.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjdxzs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xaxkgbxk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2mtuyullp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2atwknelt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2unqzobps.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fttcngof.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rbcmszkt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yruegalv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nsaebwdf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zbfwakzf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vfftsrkz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2imlfcdvj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qdmyjtae.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mwddkszh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hjussvsz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2awgomydc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mbmdssmg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uzukjmaf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gaoszqrq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ekisrlyn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qyedresn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ttxmzagr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2udknfwwc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vosqdigb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ldkleddw.html


<!-- 参考信息 -->