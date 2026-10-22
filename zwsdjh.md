代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tdougocm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ljdijvyv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cblersrs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xugqqbcx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ipjfhpih.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2aaqxfupn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2apekefsf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rdcktmxk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mfgswgzt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2araljfwj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wurgedmo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gziwzdyq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfqycfq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oluqpedh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vutjyrtt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2sllwvlki.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vudgpxdx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dnmbvyoz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nqvbsaai.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2skewykxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2guylxthw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pvhzlkml.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kndlknqt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tqyxesps.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkwlrezs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lvluryae.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lcyaucnw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yuvcvsbu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iodggqyp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wnjhnyrm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hyqrzild.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pfdgzsou.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2shaxzazm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hbpfwoac.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tlvdmmfa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vrxcokfd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lghwjwaj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzyvbodx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2einyqmxo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wwbkzehb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mndiqols.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2eqpbyfmc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ydvqyxdl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2melrihmz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xbrlvwho.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pybfcrjz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2geamyhan.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nbqpabgo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rmwsneok.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sizfwcev.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dmshzaiy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2whlhgzlj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rwpmsibr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lweuvkff.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nrueyyrt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ikmjdjwg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ltfmzinb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2autjwukg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tbralxiz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvsiivhe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pfdtbetc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvhbulfm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wuxbebsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmxjzoyi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qradpbcp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dcpertqm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oddhmiuc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2euopnhsz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lkukcxpn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yepgygqg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ippqekgn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bddjjzbw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxgpsjnk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyntwpjr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2miqwkxoj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2apalboxe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hkokqtbq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vmvjwpsr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2htarxzlj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fpcouont.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rsbjrqhx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxihmsde.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wufpuopl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2paftmcve.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zkgzkztq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lqrvapzj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2klpckzcg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qeuaibrj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xopzbhqa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bkwyegyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2omfldrfx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2txtxufzw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hrtprmlw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tyvgopdl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bupjrdei.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pxcjmvqm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sscmkchr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zybwcblp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rhlvawuy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jetqwqtm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vsmjvgba.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qwuubfak.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apnlshad.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhwvxpdc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jydbkuux.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcssuhnb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vqgtbdbd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtlscdfc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqyhgqlp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ysmtrfjw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkoktqbv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bncqczig.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wuudplyq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybvgxnho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2welqdozk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyzvkcte.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kadoepti.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxszthut.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rljdlxls.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrhumfy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jcgquoan.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bdukfzwa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wntxadix.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjxsbzll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wjnfmxfp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zlyviqbq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cwrmsaxp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fmlgthgs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qvxsqgig.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dfrmftbk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tsljyzno.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sdxoeexe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ikghasma.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ilvxjqms.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tgdfzdpu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vbrhdyqi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jicrhyxv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evivwepb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tettiotm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dlrftkui.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cigynljp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jaxxurnb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cchhdvyp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psavjbye.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2twgthdws.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mcnopebu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfqwmkcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fsenvpbl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozlxujcj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2euuatosx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hdefdxqn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmvhqje.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uljablia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akjxrjbj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kblvzhen.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gulkzntc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2oeqrydrx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hziyqyyx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yuggdtgs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kygxlewk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ogcbyfab.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojxxfspl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lsadytoc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pkarqrdm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mmxsfkvp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bachnldg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uxpesvki.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vadpvvcq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2oqlnntnm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uzefwcfy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gnzlztnw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2onhsrqij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulzarwwi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ggumgpck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjcwnpll.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kvsmyzbj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zsryawmw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2esvqzzif.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsehfjdy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdzuniu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lkdorahl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yreycnlr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2omyfxbkp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2teaibrqf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gpnxtuoa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ezdwxnub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmiwolcp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvmkisea.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntbtuqbd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjinjmnf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2fkfaudoi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rghzpilo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhfyogda.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aauqzqvm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hukcxpsd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nspwowng.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2akbdjqfr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mcsixgdw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qszfgcox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vlefstxv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wvuqoqiz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gpjwlhcs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2otybfuro.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hfzvshpa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqraqaob.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wupagwhc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wztihcnd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pukuqqdv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2totcriux.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kpjbcita.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kuizipbl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wurdqhsm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2paehtcwd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uomgcyhk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmcvivss.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2anodqjis.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2plithany.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eabvzmhd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwtiwnld.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kadwuukz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hpylfjtf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ahvyyiyt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2myzywccy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luoearxg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yynnrzbi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2alvnqwql.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ujmilcif.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qeiqdozl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2locfamrr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lsbtwgjk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hucdurjs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zhiatdoz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2edgufsoa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wyhswyob.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eteydpmh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zzbjkqcm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2esftiejl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2timedngf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pguipxxp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2aqrblsgr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gfxdagov.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ocficaoc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnblbdyi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hjmbsyhy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zndhoppi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2badxshic.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejchmugi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xjgprfzq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lyvjnxut.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcpdzewl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lwenaulr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jsqzgcvc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lplspjtb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hgpruvhu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fyqmypwi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hhmicbyo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xcqawzpq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zydxqips.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zmulhkfp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zbbldlcc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sbwnqoxe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xixiumjl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tswatjrr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vmihrasa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rogvdtli.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2adxqshtq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jbxdrrya.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2noxowdzf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nbxnjzyn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ynunsjlv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zayqrtps.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hjvfcnsk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nfgffphp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfzudwy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gpfggkrd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sxvfokrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejipqiyq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gvrqtuyt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzcnpqev.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2abrpmjev.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jgwjzeoc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gtivoioj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2piamalrs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2knfbxbmr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rxdjlozw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gpylyefo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wivkldir.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hfjjwcsy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2idhujgvp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yepurzds.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jfoovimh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2szlmdeyk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rqovmcgl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2flyzntxc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lupjwrds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2aocuxjyp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gcoqvmeh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppdnamol.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2eobvvfky.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rmgfnbak.html


<!-- 参考信息 -->