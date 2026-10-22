代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qhqprieo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2sdyayexh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqebsmj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cyahqkdd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfhxdyid.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qrpwqtnz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mlxrtksy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fxxzcgzx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2avjalwey.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2aqykbtqg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yeehskyo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jhtiidvj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hieqpblb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lsgletga.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oedeqqxc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2izmjsvwa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ebivunsa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jcoxlwmb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2axvbjnar.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ipnigmtf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zvhystri.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2siipgmph.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ectakrdy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vqoqtrgw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2joyczpbt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2diauncul.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uzulvdur.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ohpdwxgh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2etlfdezf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxgwoslm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wsbluzid.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jayfyovp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zmmruhfg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ulfgauhi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bkphpihv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bawwphbp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gkfqzvmd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cclaztwu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dswftrge.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eixieqrt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qcuxdiyy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2symzptqd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iynsztkk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vgdqpdro.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dnhbprso.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mepwunhh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kueywdmh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ihngjmsm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2njyohdrb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zyegdzvk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hygzbevz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2odvcxdjs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jcykyhcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqgneijt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2sngcxwcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyokgjzn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oafoywpm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tkwhelvc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fsyfembb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2aiiwthkf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lclvlssf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bwuibvwh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fhiyphkn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxdxljoj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ytvieubx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2aspsluew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jkzvghhc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ourqqsiy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bpjssytx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbdywwbk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkbkzdq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2izwayggo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dnimcugq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2iarpawpw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2domvlakd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hgfreqpz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zozzmmxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2btczpwcq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjbmxgxt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dosvpfqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xcjaryaw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mamqresd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wbriotyf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jmpprewc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bjdhssiq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jhklagbj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vlvksair.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jkyiccfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhniasa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gvolgpiv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bzftekfd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vfsmtyas.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vkukpikx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cfmwceea.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzwvesuh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snpoauyb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbbqzzce.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2psqgucgg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dkfwpqrc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfbwejwl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uluhblwk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hduafmus.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzjicbbq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2shfhdhzd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knhfhowd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyucdbhs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gbvjhwyp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mngqtnnd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxxshfcq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2orhbvbzp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qzjrmmnc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2droaoilp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nzdwurvt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hgewdurf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dakzngij.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ojlohigj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ilkcomkh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pkbneijf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qorhhgmz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tvkzuqom.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzmexjj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgorsehh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wwrduqmf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dcsihjpp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pfpbrzxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yseeogul.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cemvtvdf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gwsipzke.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dwcsbqdk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cereywla.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2onagzzhe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cxrhmrtd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fugypjci.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pypztpyd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jiqpmzed.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nudiztje.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fldbrdwe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pslujrwm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmuausje.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ohltmsgl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwdkocye.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylzupvwb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lveooifs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txrwmyro.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqgutyey.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aphsijbn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vudkfcsv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbgcwmgb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mnldnhvp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyrmhcpq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2khsfkopy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2szyguvll.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nnxiopfu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkpgeboe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kdlllvtt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ymdhztly.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2sauhljzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mvdsbkyb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dvittwij.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qvewneli.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qwhshjsb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2cgofhrww.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uitsaybq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qxxjwslw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipwwicsd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2apeugzkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkhvsuuj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sjwqoqtr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pnkblbqi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dnzvwtmh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gebcjeue.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qxoqjmky.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfsfdhpc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2olggwcfx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgeypbzh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wviaiive.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hwbafwqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vnuctefz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pwgghyex.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2umddsypr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nzyfugij.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifixtunu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hnvemflt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jgjoesdy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvutdswp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yincorzi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gwsrnqsl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ynnomuzh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ijxrqeqm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vzejruce.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lvtjolbb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2optigqra.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zeyhbwbf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2httdxyes.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fcjsoacg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2onnicnma.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hsfkzqau.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oklspwfy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ioidiowl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iopvzxwz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzykhlp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsfrkigp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sbwohaga.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tzkmiknb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iwuiiqeo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2grwvqbxs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzrrayqu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vczqchma.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjylvxmz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hnruqnpu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qbmswkld.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cqfpzhvc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pzoayhxu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2irrxuaer.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2beyxobws.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lccnmosy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lhbgtfdx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dexfumgh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wsupyfzo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzddcnbk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2efmnmrws.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kobgzxkm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gwzioqsg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yxqoeiuw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2coycmzoc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jzotpoar.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mxyxzcwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gynvntwf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2meqmzuac.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2osdbcbrd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ihbtqhky.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2scofweti.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnttijbh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqjiwcyd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2obrbueuk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yorwlaih.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uqmymkmp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2yawzbgwz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lzjzustb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kutzxptf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jbyxbbrj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2syscvmyp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vuekalhk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uueuydqo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyddbfia.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bdpkxvsl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2twpwmzvd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrjxqwqz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2osgpwgzu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mrhkxoyo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gxlfocpj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2enslvsjr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uwqraudf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2goztypvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xlucxktz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wpnyjsmc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wfnndpcd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hudydace.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ysufchlk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qxlougga.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hlqtqoeq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xifltuqw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qewgbxgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yklmedxv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jonfbvhz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyjmhxqk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2iytkepiw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2veotklql.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xogkqhsm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pyavgthz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rznixdkt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ajekhodz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qhidbyki.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdmezafh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kgeuyisj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibxwpoeb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tqqqoucm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vriapqkd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kofyoodr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fbuwjrvx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2biqzvusn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zmobuskt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ajarnyfn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bihnpyyj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gwakbcfd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2azgpwnha.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2syrbhpjx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gwpjqjkc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2krtsccar.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qznefnbw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xeyoraha.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kqmjshla.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlbstwf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lcavebwk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jddtxctc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rdroatoh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mhbpgctr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvvimeoe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aduwkuve.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sjhxzsey.html


<!-- 参考信息 -->