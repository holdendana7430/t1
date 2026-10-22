代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2snreenfh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oznkedsk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jfhiqpjt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2npmkckmz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jaqijnme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ttnmaeqi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlezqkae.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cyciqodx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsededhy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2efcfrfof.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aaxlkhoj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2youiwypv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pvqgiolw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dxestrob.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhegevq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqlzyqv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lfxhlooz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2apshnzfe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vwjfchvj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2txuuavmv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxuaynba.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lvtqjzro.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xycbaysk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fqhmekvl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptaodrbl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fqbmsyog.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwwykqtw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gdzhmxuo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fbkxrpwy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2mimpeoey.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jrnrjdbu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wnigrqyg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xmnfjgjq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2focmpuny.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxyvwcpk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqtjzbvj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hbmrkegi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2egntmiam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wddlhkia.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hryovedg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kpewwdnk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mrzdepdp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jupeihrt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eidbnjqn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wcjdeksw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kqealspv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmuyygwt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hcvafbur.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tkkfkuyd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nayhmubf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ydnlvxzv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wnejwgzr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dkreutiq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2faywplqj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pwyixdln.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rpghwlfs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bboyudoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kazvqufx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qmusyktw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrmziidv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvqlshbf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ebapxazr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lyzwbmjz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2luuzawtf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kjqnozmj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2twioqjii.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lhkjtlwb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfaditqt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yudnhbdu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vaotirfa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2oahdqmsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdtzftbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muinopbw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdcsmnce.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kfioxbsp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cjnvdqiq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nwphrida.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjoswltq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nqhwmwjh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vhohefgt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vkgzgwwy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ritzdcss.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ynubltsb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rlzcdkzp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nplwhgxy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tbliyitz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hfdcbzct.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vspcgcga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cklyjsys.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2agesdbwi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jsxmkchd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xmgnwdcp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mdtnbtwv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iwibllqq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mnhpumgo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bamowgmg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2sqbpcrry.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tqgqngbi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tdvahgsp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuilyfrk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwcyvdlh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mvtsnxva.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wkepyvrd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blokrbyi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abuevkqc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfhhxzli.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwlmltox.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yijwnpsw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrpwufmn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbybetey.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2furqizfs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebsidhbm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rewoksdm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgcdakme.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wmsqvmgq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zwdqmitl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qimdjltg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fldjvltp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yuwafope.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gnivvdsg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2biggqpkw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2suuapehn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hnivrpag.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tccfwede.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fpnwwfvg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbrwiuts.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pkqqyifw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ajifhiok.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cvssmqut.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zqctoxig.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fszqmqmw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2chhmloho.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vrbndphh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eigmqdja.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qgdtemkk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nqlgffji.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qnsqzsjp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jmkviwes.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lqbstsqj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gptnjtme.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jdkiuxqv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ezkgrldk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofoctzrt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwkvdhhr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaeofupv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iezcbcrl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oqwzwtbb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfiguthf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqiomukj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2immucime.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkjffpas.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evxclgey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2skbimoeq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrowrecn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfjfdpbc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yquzuoyw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tksmqzmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gggalxbd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gvmqgmdz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bpmpljkc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xnnnvfws.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tnhmwwyq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dmnxhoxk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ismhffjn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hfomjwmb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lqctyavz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vyxlipzj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bdlmcsqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skdkwxrp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qbphxlhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmrhlhuu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lptuzczr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wfdtgjgm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysunawpa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfotivcw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ttnnwywc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2izxhygvz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjuzyjr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsphmnes.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dmnkxhzg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qjtyuztq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rduersxl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olefwxdx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jexeithw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hwqeilyw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhxhhkwd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2okalsfpi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xwuiikxz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqrqgwyk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hyeglmyb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lbgodtog.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xjqosdug.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hypdveom.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dxdocpqr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jguwbbrw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yhbrpndy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqplhx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gpemafpj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2liznnsbi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ygfnuxgx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdklhbej.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wpddwjrw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2luwjeutc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcrynudn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tvvprmuy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cabittoe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2osmdmfbj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kbgeplap.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mcgryhem.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xihvbkav.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2phvwnruq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2luxzwyqb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oneobyvl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2txgakxma.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ywriiyly.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghqefoif.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2uodfmdsc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wqreiiyr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vfutbtdv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjugenbd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxrpedeo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zrafkfkg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ufdzzarr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdddpolk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ajadniqr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2biliomlk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xxbifopz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bpbrzfmh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2clvyatft.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kubyskfk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nsjsshzw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2amtreyxb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ajxegfuv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yjueibzi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zvsuehat.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cfnhqzxg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uhvisfld.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aexsuwaz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xvswxbms.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmveqddp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ktrdrihg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2epfjsohd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2netmpwtk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2eyfthfgt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cemcbarr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jtkrvzkq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2scffvglp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nkbmquzp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vbipqqvq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hryqzakn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dklispud.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vwiicrrp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hvujencd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zmhpnjjo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bgykmfqm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ixgvjysw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rncfgwza.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sarlysgg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hpkwanhw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ojblvxto.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nuatetmj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vydgrvfi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rnqznfah.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nrkiuohv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beyrqwqh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jwwzlrnj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umsndiws.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vvcqndhr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2phywndhk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vomrmbes.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jpshprrb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jlcacwqa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vauuyglb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2prskmzra.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqfngaoj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpgjoogn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xyzutfcx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uxjqdmlq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjndljba.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kaknxkqp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ycsrlqrg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vzuplexn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jcoabctv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bgosupxg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ypnsupyu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2llznjzrz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tggwzglk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yfosdblg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jwspqxss.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uebmmmin.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hqbffteg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wrlsthsw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2utmldtrp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kcoblycn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2koiuxbxt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ktcrhcyv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pmwkvuoc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ulizoxgv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ivuuqdjz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrimtnh.html


<!-- 参考信息 -->