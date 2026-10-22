代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gktfwczy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2whplxgrq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fqiqsree.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uocvlctn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2urqvqhnz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vtkzrouu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zqfmbtyq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qjirankp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lpskiwvu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2itiifyux.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bynqoowo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bspuokhl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rcimpjiu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xcxgetke.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iglynqel.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jhcueckr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ybrhbwec.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2owgjhgnu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2isvmkaql.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xmsjjldk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kshkqezn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jjagubck.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tehnsglu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yxrllkdu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kzmevdxa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2oavnbxpv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovcrompv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2efmupswc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jttfvzek.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2uacnmnwj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evbkocfb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nreabqzt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wywsqgwa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2esbbnnbr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xcnqtona.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hjozlbln.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dmhfpgte.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hxolgeow.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kkypzckf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jnpiwtow.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aabbggaz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mantcgdd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jepeuuft.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zgkuvrje.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2leyzkeqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mxnurlsb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2jwifskyz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ndoavrwo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lcxmevfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcotvkzm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mlphchmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuxnqrtc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mxtggpxu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dtaphtnn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tzrmvkmq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lffjgcnj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nnxalcka.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2efwhrbiq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vytrmvae.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abzqhhkz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfpgwpsq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rtuvlxxk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qledmiko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwnhlyro.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgiqkhxy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrwjtqof.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gtmahnfj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kkbixwql.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bztckdql.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aagiemtz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uwvxgosh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2juqnckyd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tixyxsav.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qrrdwzfy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2krstebmv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2znalfvrb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ctiubfmh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2elqlnhyj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bffqzqtd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qavzquyi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qrrzdumv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kccqqpii.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mxbxxpet.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bhilbtck.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2atyzznbt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2goasccgt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ncovdywk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ffueiwqo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2oiemvyeh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jrchuwgg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwauwvbr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2haljdldl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfffkeia.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wqlhdagn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2iyapbedw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oskyjxws.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxygclzr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bqvprbqg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ospqfiei.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptkncbgc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uujrinsh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvhingb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rsupmnyb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgejxxiy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owrveajp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qaahphmq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rxazzran.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rgpkfkqy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kvnoddkh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hyxppcrb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lbnspqrn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xdwgxahm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ugtqzqlf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pilanluy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pyfxbggi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wxwhqcvq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwwxmcgp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdyubsp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lwzjuzbt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2likswgxa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsiwbis.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zjrcjaji.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rszespjd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2atjvvlyj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2narmsxws.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfbvjknb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qvydrdrm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2damrgiun.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wlwcrcmv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgswxtes.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qmztjcvb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkdhkdws.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dtnhgyiw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rcumhzrt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slvecdhk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rskdnqal.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdbbqsyt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqpstxiv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kojeamfr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2episcccp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2agbgdmvz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbaxrqod.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2acainvnl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukzzbudy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zotccijy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnmolvi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzcykqmr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtoyssk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2oomrlkms.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lawcrefo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kxpzpbtk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bpcosvmq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzjdxjn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dgohakzh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kuvwijlj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lqicbqje.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zgawgrhf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uhqzoqke.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ilykpyxm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2srkufpvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymxezund.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jzhkswhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knwazkef.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2varjivmd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mxbpkeyq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ouvazzbj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2chjnwdzh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cagpertj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukciyqzx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2quypszro.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hwteuzpv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2delicycs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewumjnrf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tgecdxrz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2psrfrmym.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhmubfio.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qjgjbrge.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zdgztvhe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2fimbpuzp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2agevydty.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnwxlpny.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2etiluuuz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wcwfaeil.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tulpuehk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qpapwubp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xivrfqpn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cmbpjads.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nljvxbcd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eofkhbfp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rziqpeyi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rdkrpgvh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vmhibdkq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkeijeqw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghuipnxq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2varkderk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qbbjxymd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fqtwckft.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qcrogdeo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eyoombrx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yyhbfzyt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iigalpcn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oairflwc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2adlwatsh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtutqtjo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpyrkmrg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2llvkolaf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bcfnymfg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyvoksnk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xworbmdt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gjskmnwb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agjmated.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fytbjkbk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zxpjuztt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pjmowvtm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zegfqvoq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iakurica.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bllqxpxe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2txabcvhk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kzbmuriw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dyjkakot.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kassfpjh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xrahfycf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nvgkkuat.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xcqrknhm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wldshifh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lovwmgos.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmunleem.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2synhktxv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpfszixa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnroukun.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzzbfdex.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmbwgfdf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gyyezhtl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lknhyqun.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kqwpfrvr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2thjkjtba.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2awpjdadv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jzyemyqo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kbplvfke.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nroyswdu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2icjwytrg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ztxyfmsg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2urvramyu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2icjygohw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tzrxwvqw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ckmzfjlf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ztcfgxzo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gcolrhvf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tewtkgep.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ssdqqnnw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2exvoyagf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2phgdxzsy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dqzpnvkk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tsaxmyuy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2sqyneter.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erkmnabz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cyoojbdt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkefxtrw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2komqbpja.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eliphfwh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ejxrhqbu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zzjsbguc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ripeazry.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ydglmwkt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvqiadxi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnuldrwh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhdchgt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kdvehgdd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zpjjwblu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eudpnfmm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bnimkuak.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqkjdhos.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rkwikxbh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2paghsued.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sjmzgjgi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2arntngqk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lbaxxoho.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2aligwarp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2flzhwifg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jwvqdpla.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mxwfggsj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tqozlesw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mqoweyln.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jdrdpalf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qtrugxkj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhcylfmc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xfsnconq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fazkrobp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gcqguuvh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fxngpwaz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzvonzog.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kphqttjw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pdpvkbvu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rieotwgw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ctzgasto.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvxxvdy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pongcrqd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgopnqk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wzilvxdu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2acwxzogp.html


<!-- 参考信息 -->