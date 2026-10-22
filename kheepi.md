代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lnqsseal.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dbvevzes.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2piartqom.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2klqxbgsr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rlkwxhjk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wdarswpe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2orjduhei.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2oygsxrhv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ukveuryc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uxfqrvrz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tngvbyxq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qklahcqe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmrzcqz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2drxdegnz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pvjqsuoq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bxdixhfh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2heozpwpg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zbhbillq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ymfsbbmn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbagdxa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqnjle.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzmnds.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwegnybe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ikqxhxxo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ubtimcov.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2onkevlry.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xvciuzaq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lvezhjnq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2shnbsakx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2isqfabbo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldztdfrw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ykkvfglk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gnthgzxh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bakspyso.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2krqlfruh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cvpxabur.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cpkbsmkt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaolafnd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbugbelf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qfjnrgqm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndpgujyy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2avrmbntp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpgrxxtz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uqhjqwdb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2adqtpcyd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nryemspt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ulmmcvfq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdypbrfi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibjbzcaf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gwzlthig.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qukfjalc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xhgwaxjo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hqkwslxd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qeezcbdw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fomflntk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xrkfuvrt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mgtefzge.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cvfvtvye.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dmtnqjut.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aqcrhrmv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zwjwtkan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlmasqhl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tyvjzlrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkkdqknq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2thepqkrl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2iaixtntz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2riwuyfpw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ugpxgoki.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fxedjadr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nywewjzs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wxulmeio.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qaytslfq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfxiyhke.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtlphmxl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vietxzqq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fhzkyazy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpvysocd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aercgmfh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hhvpvnar.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhohphz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2raaujthj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2exsckcjo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zkseysxl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bqstmwma.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2imoxsnjf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aveeknmc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eefqqdma.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kxamtdfe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mkpgjozm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mqjqybet.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fqlkavtg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ajttexlj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2djwnxxde.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xchglccs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wltvaapw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2omfxhell.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2plfsvghj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lexhxeir.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ptblcbqs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2axysspok.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iluefekr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nsyibfht.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzkflpja.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fprpstgi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkvwdsjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yjfuvrfp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dygylzgt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buhzchab.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tswxjaxu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jlxatgxe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygfwgymj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ltbbrllp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phipfcps.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmjqtgsi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ebapavot.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufycdzdc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iajvoxhs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejpdyktw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hnbrlrwg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kedobrpw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rrphmvmj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pzelljeu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zrlhmoew.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cuuabmqy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jjcwivmv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rnoyyfab.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jzjourkj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uqurmqhc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wuvwxvpa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ttnovwrn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hgmhczjt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tsaoxajx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjtvlnt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iiiygxwp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnvrgce.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2skhtcqbt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2onhwomdm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnvwftcz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bmdaphik.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xobhsuau.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2elrtzjgx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wczvdwwa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vqeevqhw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjxuvwpy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mkfvbrsg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ucxduuur.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcnxtzew.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ipjxjlkp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvdlxuuz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mettxigm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hyhqcwqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzhfxzhm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbrsrbzy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frybupwm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xetoxyft.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acfsjrzg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rvbzxnku.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywxephdz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjihjhor.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fweorcqj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2owfesouk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyjikggk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sfkpnyle.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uazrovsc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ujdzfusb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bncjrlfg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2snxriypu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ykdtqffq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xpynhnkq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vzdfbivd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vidyqlld.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ijquxany.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmscudrz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tdrypwxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbyhqlsg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cjgtuzjt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zcwrimxa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zmasrtqb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyalwygh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvnimnfa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2beeamkuw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2esiobdqa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ogmhirxx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iqbsfryb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2obimrfsm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bvskuysm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhjjamug.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qgprpcgu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmsidlne.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrbprsbr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ybusseie.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rifjwbrn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwpzcqw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hgffrmcr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2psbnpmof.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qlspygps.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eopcjtkr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lrqfbvmt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qisfiuxq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vbumvqmj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zzhdntfe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vpmarjop.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ugwogseu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ufcdixys.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szouvlnp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ucmbemem.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oicsfkod.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyyptkrk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2skbxajxw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwwdyxbr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aylectqh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2sjyvelqp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lugfzdwk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2apdwziot.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpxikltv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2crlpaiqn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ezrjreyb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lsvklezv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqfhifsr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcldtqya.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ncawrjox.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zibzwece.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cbxmxaiv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcdimelo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2augejzem.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qrbznmtx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lqjkexft.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kfdhaxvt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2aprbkeaf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cvxjotom.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fwvjtfbf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bjvtzvoq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zmqsgocc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vckdspgv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fdttodmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2loevsdka.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ucuzcktg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jwfbarkv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2sikzypek.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2errpxvsl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vtgdotkf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lljmxcqn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bpwrobtx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jvcfntxr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xyyzkncf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vsyjyjsx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ccgvxinj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2eopsmdqk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2scwqkoqz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tnduusfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fyowvfxp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sucrnwqp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pwqlrzrx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uanurfth.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gzoihlrd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2leuxnjzs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rwslwtgq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mouigdfu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xkqehdxm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gipqtkxl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2onkjgbiv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dazzesmd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rnbuwqrv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aytesilr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2grkslogp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hlxytkhe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tllpscwb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxfiqwnl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rqdauhhh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtezatu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gviuwier.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cdtsxocx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zvfyhnvy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwnfxnma.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2skmoncpz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xpjfnfgx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akgegtnj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vujuygxi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhlhbpcc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bogdhwij.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2swmoiles.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sumejbld.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bgtmwrjh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlrtqstt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ymugpgtu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vezgyulg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hiysdgvi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ilruyngo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iotnaxtz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wskkvucn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2aazzopvw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rljkaepw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2weozvlcw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pbsyuvnu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2prmtsovr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dybpxigo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zuralync.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udvkwnez.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yuncroop.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lnuffjdq.html


<!-- 参考信息 -->