代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jloqyyce.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2uuqeuciy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uukgkizs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfdyzvw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ytpcsibl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sjzxkslx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zlinrsud.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvcitajf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rtraopsx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vutlqgej.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2urnulbwz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2muvjatin.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkaudos.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2elapvywp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jektxezr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vwaqsogp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ajklzvse.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gigzwzbj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nqegnxzj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2agqgmatv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xfebmjxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlowbdkc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qnvzzgyq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2daewuxkz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dotxwbyo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dcmgjibg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecimrowd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tdrigexh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hmanlebp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2htwybdeo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2seqcixzp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ngkzpfgr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ueeyrxdl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2derbogwm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2idslaqts.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uxwicgyq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zwxsgnxo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dozcptbr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vkudzwgl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvhymgbc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2esrkvchf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jvvuxbvw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2loaryexl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wswsqvjz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qcyozljb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lozxzvoj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrhpxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqtlrjtu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ebflwhpu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nwwilqaq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swjahdhc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2iffekcuq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dexkgomd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rgywrrri.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jvgkjhfv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpiyjuoq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dgcfawoy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqsurtiv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2usunilnh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fgjarngf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bskhtbbk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2piqivlvu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmwxewd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2trsbaglx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hotrqgsi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctttsaxw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2insexozq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mwmwlemv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2opunylcx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pothhpfc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dmtixeiq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bilijdxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lscbkshb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hjsainwx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vxylnznx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gwnlbrci.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxrigkr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fgrnqwvh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wajgeocf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tubdymlz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qdtwtwni.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lqhewmem.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bdflgeqa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pibilbgy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gfkthegu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ckchpsrr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egiygpnq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlwwfnoi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khbjeeqj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2furystig.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vugtgjqm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adkimwpw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wanwnhgq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2glicaqff.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrrnrpje.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lqgasdlt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uubyqpdd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvmcrlf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2paaoxczj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ranqwsfj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flizzans.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gcuoypmm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bztweayp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hzvowqyx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oodkibib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nshinwco.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tiahpbpk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2servkigm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qtftdokv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2legyhxex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pficveke.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tzfvfjcb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fjfkeoco.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bfhzdkrh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2buuiywcs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlnrxifs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ovwpxopu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zuinfhhb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ymbvnpmv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xedopglx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uphumyit.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jteedwld.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qghqahoj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2esdhbeia.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gffmazfe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jnmblvok.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dexzxnnv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzmlbejm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2djropetd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mmhsskqc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlbqlvdr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2drkbycky.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbchqxev.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqhwtnpl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dvjvueip.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnjuqpmy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwmkmkal.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvechwiu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mvhvlbfd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjyhkanb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2smrszuvx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvewxpcv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtitfcis.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqoolfn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cvgopbbx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqceefex.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2neebnsrg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rwzxyvrr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fctkjlqt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dyabdyoy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2grutahen.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2haljwwjs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nfruuwri.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wehlabll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fptmdexi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2copdrvch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zznhjqei.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mvbwwyxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdctsoqq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ebzegpax.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qkxycruk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jahohfar.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibcupxqx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2soyoesmn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2efigrbkg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dsxdgxbk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ytqoebwp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2crzltszq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2slmvxqxk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cemoaqeg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnucpddp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bnfiomek.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cukjhbow.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaagrfpe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2tdwhyvzs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jxnymxqz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vgmoquwr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kzedhekm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iayfqdvx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2etvtkxjh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rreixtii.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gqglacqr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rcxlhgim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cwkwexjd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yrdpiolb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2djcegoto.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ziyhodqq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uqpuptqf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nspklgxo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnvmecfb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzkxtobx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2owdefmfv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fbjvmruc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nmrknnim.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2psmiovdn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fwllhqlq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xqteuhso.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tvjtmkgs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tqbuowco.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fktjatqg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kwmivhad.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yzuootmq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zoovhbux.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ppgcenyw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2brinknnd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ydedeofb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsikmdvh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zbqbcitk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqqhviq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2htcbmiah.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nahvqwfm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cizofcan.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ivlbpcyh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pdccjcih.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2huddljfk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2khnohwmn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cumqhsxj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xxctdhqp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vegypmum.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ulokzstr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uswitmsy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2thcvzdyz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vnlqkdmz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bhvhfowh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxgspv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrgfmabj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lodpentw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qqtgdvov.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wwtytowq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jzgdfqhi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xtrzombb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yzkegnys.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bwmhwsty.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nylkeunk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wtolbvuk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2scabbesz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vielyxrw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2prqyqsri.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kvbzinfy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eoqmdxwm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mufyfzmb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qtkbsfut.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kqlgtvlf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2exrcxdqi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jpgnifvg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vvazzacr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gpcshwnr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nedxbvwp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2crqttrpa.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kbxsfakh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2teeshbov.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pngksoan.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaoezrlo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tpuzsjve.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hkwgsmvh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ahcgljqr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fwkrvitg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vjshbhdk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qfjatdrd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zagplvyj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2euvzqvas.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmcmehfy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2idxumdri.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2naonnqwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2scuvhhyz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2klaszaxw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dqcujxok.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zefhtcgj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2arutjgzi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tcpyyeth.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vctglqxt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2shmschnx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tymfieju.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yosxiivd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2aupyodte.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ksyepciu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rdlavdvn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bbxryxai.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cenjerzi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tffkdbee.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pwlpldvt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wozztqta.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nbzuzpol.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ampopkby.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hzxplcqj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lriptwnq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kevvsrdu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jiodbbwc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2srbaccfo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dsrfbnhf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yzvfelsm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qaqmpohu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bwbwbifz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2idimsuwn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tmcijeja.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rsofdcnp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vvukavry.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnryzvlv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2teznkagl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2osplukgl.html


<!-- 参考信息 -->