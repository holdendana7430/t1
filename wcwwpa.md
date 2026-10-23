代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ajxgfive.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wedeayty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fyzasgto.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xorctlsf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3abkugybk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pzflfhyd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uxmlcgwz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ylddzbpp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zzaipiya.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lmrwtfxg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gamxwhjs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mtrfgbcr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jadgbuxk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hqkfrkos.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kqrswzvj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dxcbsalu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ppgvcwil.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qyvgtmmd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rkptblro.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sbjlczxf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xegdijkk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nesotzwk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3srccqsqr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zwuiympv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xhprosqk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3unbcrxeq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cgeywkbt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3msrqmwia.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bftmcuqi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nhdmftik.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ebtddsze.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fhcdfwgw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xvtppkjw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pmjdpest.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cpabqckf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mnkhcoeb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xdvdpyih.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3onbqugqc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kuzntczh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jneyxrjw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3afydwlfh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tcstxhgd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tnthlkcs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3mnwmwqws.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jlpusynm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kqnoicij.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nfcxotbh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3coyqfbpg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oeerbjou.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nbvtrwzm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uhrwvaue.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yctlakxz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vchfsskf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dycltjab.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rhxmweyl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tqxlnxkn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jsjkcsjd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tigmawct.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xumezsfj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rtonzngt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ryhvdiep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxnmgwfo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wznioinl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kiosfmhg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvkmttwf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3elpzewup.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lsqqhyzj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lddgntmi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zfxpdiys.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzeffwgz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tvxylygo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3diuzoltr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofkeldfo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3makscskn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mlgbnlca.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yysdifll.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fepoxtar.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hldsfdmw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3runfvoup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fwqgnjhz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3edgunnse.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nqhexyhr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oixawbaz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kkzxrfut.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mofvxrkz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3haktisij.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hwltnbfx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3haxwbcyq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lfbgxpqf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3apsyyrcw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yeyzjpqe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmlqepaf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ijwotucd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hoqqywgt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ayecpqtf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uztuglui.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bnorrxlo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cwgzgejs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qezbiqrq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3chcgrxwz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3morpqccs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jlenwllg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3miroopko.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnfmyjfw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptuhireq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3scxyumzk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ttofbqdc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsejpzim.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnzwhtph.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qdzeymnq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3raghawek.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qsnvtzaz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgmhxcph.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzzrnvln.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3klfsapgq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvvuqsbb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifiklmuq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qsjtgkkc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3agigxxra.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mhjrwbnh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3iqrbqtqy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qusqlxxf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rojgoytr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksebioxj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jfgvxzpa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wdyvqanw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ccwehqzb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zvejlqzs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxuayxu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dsxvgbyo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sbuelzjy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vostpklx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aqklrskw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3frlmsxla.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3enbjiyam.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ledcfecw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pawimwyn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tltmoqhz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gcjhmfjb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wsllzery.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uwwjqwsm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wdtqiimx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ojlmxhum.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sybexxym.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nfhjdtky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3htevinuj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dscltise.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bulbdqgw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqzjnmsr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3maklymzx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3uqibuwba.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjvxgapf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igruiymr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvbstsxj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxpblnnq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfbradpn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vonwttni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3likzatwm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrtaqfrk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ebxqsqvc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3avcenjqn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhwegvud.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jfdamuhd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3auzwizcp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ywgqlmkk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qczldbvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lanewacm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3euandjbo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iyblupnt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3esadbssy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zjqhagde.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ealfplqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgqlylkw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wtnhnvnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szjpaqfm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yqxlvjgr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mhnjivcz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bnjgmkea.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3roigqdtm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwxjpijc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyvbzjrt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3twlgwcnj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrjhxewp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xuzuowkk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3erwtobmv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wdewwihh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dfxnffgy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxcerjwn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uawvsirs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gflpoudj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhvlfoo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbugchjw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tzwducer.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tfqkhbje.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tpdkpuia.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zihwelap.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovjpnmzz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pkspneeg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rnbrbsbx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wkmmcbwy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gcynbfys.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3avshsgvu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3coutpert.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qbdrvvit.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eifboabl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kysfkpot.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfjfovqf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ynrxrqxp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3llpsmbks.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mufhmhvq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gzxbneuz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bqzdagji.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vpvzrfwo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3csfjrsyb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yclcgpfo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbtptsdt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3euyacqyf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qsukycrv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fwgcvhtz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3royttsay.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nntmvfra.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ybjiidwr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fepqzyto.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guxgjddf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3troqgfdo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mgyxtpnp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3orbomhxx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mwmzqwqy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3owvjcesx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tjqobrmd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3srthwdxn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dlvbaekg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qhtnatex.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qslskdes.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zuwnsyig.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lzdogttw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bwhqlqgn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fwxvjcyy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xgtupfst.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ibbivjoc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxqdwtaz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3lxhizsyj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zzoprvbx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cfnmbsrw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3prwysddl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3absaxrpr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3llleqbrk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ltxrcfei.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cnmqwalh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrdgtkij.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kyxpmwvq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivizycde.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hgznrddz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cwvipuet.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ljfzispd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgxnqufc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pxgdhldm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wknnwtbj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dapmqrjs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ckrknlwa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wtxsjcbz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fkteikos.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xhustiwh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lwmjeect.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nlaotdlr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xkdyxaqp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qxamscke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epfuhnrr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yvjlfvun.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyoonykr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqsdjiqk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hbfblcix.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hzynhxed.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pokrjdqu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtjtcopx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xypdpbbs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmyqerap.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilnprfcd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ohknjber.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bklmcuci.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3upddeqlp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hlielytr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kgopycox.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpxeabet.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jlwqlyac.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ipdfesgs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cxlmzvqk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3osjkthoy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3etwlqtxu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kwwqflau.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3apiatxei.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dbspgjvv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3regbdgzh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xaijfnyn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3yafwfbhf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tvvsewyq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3biuxacgo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jckonlob.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3povxopyn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cpfmhtgi.html


<!-- 参考信息 -->