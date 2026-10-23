代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3itsqdpxu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3duqasnbz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3agmgqkyw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bzxodknw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dbsnwkfj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmjtgsm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3urayeajr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcxsugs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfavpwq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3grpvurgu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3trvbyial.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kaosazpo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbtxatip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3phwqjypg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wmosjgkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3clpazmox.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bobmfuao.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ubxwhlys.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gnfivjxv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3equiayzv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ebmpnphr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yjpopejp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fiyschvy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cgqjosvj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yadvhtaw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ofmchezw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dhdknxpz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ilhvhcbb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jaxcmnbx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zvzforzj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eyhpwbag.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3eyiypqxb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rtewgsco.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ywijlzcl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nltlpiuk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwajpioa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3spbxawqa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yejopqol.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eebirjuh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rdpjjmey.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mkaicfbs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xfguedvn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ucofvesk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3owkqedoz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ezwtwhfm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tuendsig.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qamufclg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hjkdsfki.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3izwchddy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eygdxwii.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jzjbqsdm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmwskszs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eklrnvfy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yrrxymps.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xrqjuhfz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nsnvnqwu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3riwqmomv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dousjjzw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fssxjhgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jabywtcj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3atmbtqzn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qnemkrtz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mlgfmdtd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3imsgrwpg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ezbvnsuh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hzsoxmry.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fvdntsax.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngvbcxcx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygrtzsuz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3lrsenude.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bbqxjdnw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fadmfhmy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ibmlxyqi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjtgtggp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3waxjhvmv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bxfxwira.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kwhraeym.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifetzhew.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kpuoonfh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3weosxtmi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bmgikugp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bwcmiolq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fvjwtvap.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ntuctzxg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rotrrfop.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rivjjuqb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yotkdjsw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3melzmfrv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lejtdwmr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wcruvsac.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ohkwzxlz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3opbcsile.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mkifpszt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bcbbxbkh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yjwfbsxd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3amnthfac.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hsvydvix.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gjfkrmbo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pkcxdcgz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xittrsul.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpwyurem.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ctpoxvye.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3todolcdh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sotykdky.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtdijmsh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnhrmnan.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvohrfkr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dxtsftex.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbvrzdqw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhdnrksr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uycsvpjp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sesfctvj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtplkpks.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihjxwuia.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3igjmzfyz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mhxvdjpd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3okxyguka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3urcefxge.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bcquphnv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dyhkadjy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3epqtonao.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jbtqexel.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3aojllokn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3oeqhpcub.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bhcdnkzj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3sydznrig.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xxvzdyqd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bslemuln.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bhnfykvs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3meikdhyg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpgowsr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3yngaszfp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cdsokhkz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fyxxojoz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znkmwbki.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kuguwmlm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jvtyxhnx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3caudxerm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3muybrukr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxmsqjad.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qutygiai.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3douioowz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhlcfjw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ckhxqofl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkquemyl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smmmoizq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hcvyvyza.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydsqrxvu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khysaozb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gigxsgjq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfeytyho.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjjvqzda.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkdhodst.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3javbfacs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfmrucan.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hzsbwhrv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vcgkhvrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pycseucx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3toufeqll.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3psqnidyi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qknzznzm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zzxsomwj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hfwbtzxv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mjqbgpvv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hwmansjf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xqoxudek.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3cimggwto.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cdtmnnog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkhaqgvz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3deqkjfpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swzvvoer.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tjmxjyzu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3yfluqqhc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3uhzirrzj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaycqzbs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ladubqxg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3isxpegqp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sqweqrqp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xhqxcxic.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ithsmtqi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcuoqjmb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qptzszcj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqntbaju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3psechuby.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yezlwhhx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqdrsebf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yuhiobvr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3awawiqck.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rydpskcw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xpuaztxq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iadmiejj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evpkinxd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uqmwnjiu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eqnfogkw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tmvzorrz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qexjjbhy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ptthnkis.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uthdxbhh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3uwwenyhx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fqvmexuc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwhzarzy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3redgwoxe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkmgvahl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjmrdse.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fjeaqwpg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ykobqeyr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xdeahtgp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qlchifoe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3psssiyas.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwirubbv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wldvfrhs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqqphwli.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oayrfswg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dhjawexo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nrudqmtq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ajxvibjz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mflloixe.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bjennccg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pggocwvp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssongawp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kpbdejvr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oweyljht.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pngiyygr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jeoimewx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wxcvoajn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kfpdsmbm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wotllwao.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pjlfvzko.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lteuvruj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fyueuyku.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mojlqdxd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3alkeipwd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3gayutirx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdvhwzno.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zrwqcllw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vpnhemlv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjrwuygh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahockncm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rotleijm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3trjmxknk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3btmrieao.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kivqyoun.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3epkhdpvv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yubusrbp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tyrwfzdr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zuzxoyoy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jrsyfzuo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlgatafi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkjtfjxl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3davlvuho.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3udjwhvre.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kcfrgaxu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yvprkecc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3excmhqgb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mndbsanj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kmizdenb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xmjwpufr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yvsnkdjv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3emqjzert.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lfxpqprr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wvrmsckj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3arwpzpnu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zcjyqeks.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3reetgjxw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pduvksxu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3unkxtbpo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrppgbup.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mtyjpvhl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3urwbaexg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kezbmdua.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mxbeqrck.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lrhsqkak.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pptcmzay.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzndsprj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwdrbaki.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgychbcl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eudygbok.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3azwhbpkq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wdismwqy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3waniceuj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lscmbthe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bgajcnck.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yhbljekd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wcnhsnsg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fwtrxbxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3srxnwtbq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdrmsef.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3roipfwcj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kpmouykl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cltbddbb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qzlyjjnc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nghocmld.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vxfcrspd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bithzkad.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jnddfmeu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yjsbvsla.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jntrcnbq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ixvgqkfy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vsedbaeu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yayyprjv.html


<!-- 参考信息 -->