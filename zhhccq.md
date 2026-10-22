代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wqglpehj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jpmctjug.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vagzfqdv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zpeqkbjo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fioikzsl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhdbhul.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mklfgstg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sklkvebv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iemjbnem.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pgipujjn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sdpslneg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dzlgwbvc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2idyiwmdt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ycsfgwyb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2asqlsjps.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nbllkdbc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rmdpapue.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xldulzyg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ypkasago.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2misjzygt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2csbotrmv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odtvxorb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ttwcjqpd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cizsunad.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sqpyzvro.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2petcrqfp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdzreqmq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vnfoykie.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dcweftbb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ootocemq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sdiedhlh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oiajyghu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cclzoarx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mvwmtaqa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlsvsges.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tajnoven.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2eyvzctbv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uyapafxd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hinrpylc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tpeewnnh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sudxjsti.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eopvgjpx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2socraijm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2udnrkqly.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kzebxeor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crirhjmw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rvaafxpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skxkbpjz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sikukfhx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2stuyfcfk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2grtfljqi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2haoidguh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jjiaetuh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xjpbngpx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kevkboyx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avuhhepo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2frpdhqdb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tbdgppcq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yaiflgcx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dsmawlhz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltjccxpt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qchncizt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfmxhfh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fadctufb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ptpsiatw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2atcairrv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2itkisdmm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zpozbifp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2agtriqtd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2brtufnzo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dfcsqmlz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ubfttsag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2vfikpdjc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vyhtfgor.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2laiygnmx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2swatprdy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bbcameof.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mkvmajqk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uyotarcx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fmniyqgb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjhnlue.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ipxecdxv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wphkfmld.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wjogcylc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2keafcgwj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xeitgbwt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hehndaja.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htfpkgmp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqectdzs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kcpzqfib.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2aboplhtd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxvsoqmn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ernqcfhb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkvvoojz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kucycphl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkonamzl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzpboakx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wevyqyuo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kjgjydyn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsriohgo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxsfuhvv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ujvsvtym.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lnmowube.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtexbgb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mevamusq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2atvhaxuv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pnujmjis.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xidbmumb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2frdcqlko.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wauxdvqx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qyenhmub.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pijeqsae.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qckkqgpt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixyuijyh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uyxcddcx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vzsfqiao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fwjdgeht.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xtfxqhpi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zlamrsov.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2orrmqpvk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2giftgazb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkivoduf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iyxmbrqi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wzdtqcxy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pfmhephk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwgxtvej.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vievmafg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfweamvh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wlkrfdsx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kvkjvxss.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pulrvocc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aymomcco.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czscdmct.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idtxekca.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ybxzoxgx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obkvqliv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hncphwfx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqajtvvn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tzasonpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpyujmcy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ggojhnqh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2grupufef.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aodewqkn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lpggynjz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2aqumbskz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcftqsku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hxelgehj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qcrbndfh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pzfzrpbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2srwqxnne.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cggbpkei.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hxmeiuyt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yrazffgq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2chlrqvcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2otbgtqow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2loyjhcgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aicutqvn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ovtxbfme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhnrdrnj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wcduveqs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mwutxhqs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gpjgpelb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmztcieq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rnwphuxk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vkdqemwf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wfxxuwtn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iuxthrsc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkwlmhql.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jhzuplmt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ujuogygd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vtlahdja.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugncblvk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cmqqvdmb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzcbnyiq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ywjvdlha.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tbzoxfnf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iwcscylp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xsildatb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xgzrymyz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2esnjnhls.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wdmzvjat.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gvzacnoh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2atyjquoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kowlwopm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rskjherp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nmymeimo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2igggains.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vihzvraa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xadaenvy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdrctkgm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eapaujua.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrgtngtv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kwjqecqp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jtiydcmm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ylwgwyum.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pfnqwjtq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bjbltjpu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2futjhafb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rigafnlf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jdhgirko.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eimkxnnc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2nmszpylm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dvfjvpna.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnkbhvcj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ldjipjzz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uhhzfqdu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ycbwqbsx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2medymbvo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hwtkvvyu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaokomwe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bevouemz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gcpupdxo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2afobgmzj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bjklbwgr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xadlpnql.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lgybxxig.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bvwcebxu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ahhoabjw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bnyouref.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lnrysbnm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yldyyygf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gfpurplj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pbawtnpq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rnggunfy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zmxikzxs.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2atahnjbf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wefjuybj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xocunrjf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jrymzkbf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2irsmjwaj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmehkvrd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zoveuhzm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2syzjgzpk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2eyflyqrx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yfuspqak.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2slzqspap.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqqsvtvt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hwvmwozv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2stmxlzlo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tlpouzuv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ufcyurhn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jqkljzka.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uegeqqoh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ukslwyvt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zushklfm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cnyxmvtw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2estndxti.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cowuvoto.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2myjcundj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vxnpouxt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wfakcexf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amcfaeud.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pjaosimv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pzkecgbu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmaikqkh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rgfbzcgg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ctsnebwl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rllntppg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2eewjohba.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hrexmymn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zlrsbuii.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mmvlexau.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2byjmpbmt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yxiowtwr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gjdlcyoo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2odbtabuj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uyotawiy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ararlyli.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dvdlipnn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2antvhgkn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rvywtylr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wgwbozpq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2crxrrcxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hxywfjon.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dzaibwdb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lcdpkhxh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ewdhaigt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2chwtywzx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hdaimrrv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rpzutdoh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qdqgeamk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mspppnce.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nhtwljgv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cxnzsnhq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwwcohz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ecstcffb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qpxacpwc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hwgrbiny.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pkuwwwjf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vdkvxasp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tgssltch.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ggawdkve.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dhtgfvtw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xyjpdjsp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2heylaoxz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dximpafd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2svfgtapd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqnloyer.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ipiqqvqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rgompsvl.html


<!-- 参考信息 -->