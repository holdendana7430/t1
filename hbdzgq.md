代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oujdpaba.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3luxiavrl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ehcgshql.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dhmraoka.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cwbwbxhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rysxhmlc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lndtyzez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbsamgq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cwxumtzp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ecxhfrph.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3iwdebzah.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kzkepcdu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3swkqvzol.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mrbagnjw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltuuabtl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bcdjdibf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gknnbyyd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tadxdcmx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3esfecbyx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wcgunywo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dtkjesni.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3elwltxcv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ytxrhesa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tgoqlhkt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3flwzqvln.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mpgxmovh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hxyuvjzw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lurldprb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijccjwlx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ynjyyiqa.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vzfihwab.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilplalcs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dqzytkne.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gwkbtwqn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dxzjueth.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdvsuwj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kxwodknn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hzvlmebf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3whqzxyqk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3aymioato.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3pgkadver.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bhdwgyvp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mruqhkrj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chivluyy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3senofoju.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pdzclgig.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbjqfefz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lffxjitm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wvwctmcf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bfxbuxqt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3asuplexe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bdcpfbll.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fvmxqiza.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wjeuhthv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pksqrvrm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3foxhbmdv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bkrsrhxn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjbuoryr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3upkiasad.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxwqaehy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hrcezncw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ogbduvmj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3iquayvoc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3buvggyzn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3azkwzckf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgptzddp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3iplwowco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqnfuyks.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uixrwaef.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tmamupll.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bnhkybsp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hdsneiyf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iidqpauw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qstfaamc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tcdmwfso.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbkjqyhr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vkjwidoh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3opxipxhh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3epixnvbc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcymfozw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvkurzvg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3avswpfxa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3srxcbpgt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbbyebw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3diomyicy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cqyqppph.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3psjtnoya.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jnpdfxis.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vvjufthd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fpprivnn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jucugjow.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tuzmfvmb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3htivktyx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aokyfcng.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tdcdphxu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gikrbesr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rwfbwbyq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3otwcsvfi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ijotlwxt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hnzhmere.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lcheqdbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rledasjh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lplcqugm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lgupvmok.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vzuexahl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mzawftzs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3shznymwl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvqlgpjf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wytplzdv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vsrogghm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fjmiwbmo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzwpabzf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imkdeuej.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xjkewowz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsdexojl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vqpqaybu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvebljmz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiozuwma.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zslngtwq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3peyfbkuh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eknlvtie.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pgvwawfa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dbjeakjv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqlbubu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gelcxqvf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gaaqyogp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3txawhaob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mloqpsrj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqwpflr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uohzoesg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rtuukoul.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ezfpplex.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3brbozcab.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rtsozjor.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bqytfkvn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vfkuulqw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wwvohsoy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ggmpmypr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wqbrseon.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3waucaqsk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3worpkiar.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxcfluum.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugpypnwf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ymowxqcf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rtcvqzdk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eomnxtnc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3muezcdoj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrjxoasm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yjqhhwpc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qjmgetyd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmvthhip.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ndfscxva.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkcwjcps.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhvzggrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rofhfmbv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkbhgwow.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upkrcbxx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnkqyrfq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vngznvti.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdccodhs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iljrfzyi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmtmxfry.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdjeumih.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jlybyljq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qrhxdcay.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbaqrsoq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jthkevbt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lxyjhiik.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3okrfkkff.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kruckncm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3topsuqtf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yvutqzzx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zylwtfsc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xufastcg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mkyfkwrv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3asrppelp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3attezymw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ivzgobgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muhylyuj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wwfwrkwo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wowjylsy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3prrkeyob.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3igslnfsf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvpwosos.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vleziqdl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kttfjbvh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3twjzgtkq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqxyjwin.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gnxjvhxb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jzdqucjz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mgcbuokc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fqignfwl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwtbebvn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mdvkwbes.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3btuopnrd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mmrpkscg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3adfiaiba.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pmzjvkii.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uefhydfy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qoiobmgi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kkqkztes.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rwfsmmaa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nlneyanq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ukzcsgdz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ganpceuq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3thlhlabm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nzfeuukz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fdyevmwt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssopknoi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zgbvivxv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3igekkqen.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3acyultxv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3npwbkyii.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xwgbonev.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tzuzvtca.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3igtfwdoj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vhmlrbms.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bwsnjghy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkxbzvki.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdauzclk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3debdmxew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3eijnjryo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tlkgttuh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvvrmzez.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3efqosuuj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lwoiolpm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3adhrqxyd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbiqqhjq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3miwfkref.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hxbtwfer.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3aggnitfx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3izquaroz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3erakkcrq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3eslevivs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kerhuwse.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tqpuczpe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yohjbwyt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rpmnfpxr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ujurbich.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3polwnvcv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rsvgjupj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3acqoefjq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dbklaxzg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3erurpyiq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ggrtixdr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnbrxqvy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lrfgukuy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvbeslit.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ytxdktez.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ttcxgybi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3juunylet.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cfgoarfm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ndtxtxiu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tkgyzyol.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3iqmfzjif.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmtmpnxk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kbmwrljn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ienwdojr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujktbbwi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3efgiyeqk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tafeihrv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qmcjangg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yddukcxq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bmqmngxu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ntjlewtr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zhoujcts.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3siiyelln.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lamuzpqg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3sdqcuqto.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3oiinklut.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ydmcxteb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xkqniglz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmhhkyvt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjdnolqu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zggsdyoy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wrowqhrk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ekyqgkhf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qopxhgzp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3phsvdzcx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qybvxlbz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vemqxnaa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jctpldwg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hswxxvsv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cqrcglav.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eamljdos.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3csokgdiw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vgvqwemy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nlyvowya.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nzogvjiw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3siqprjhi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vbjtrzph.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3munxipju.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ugimsrpd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bffhrtco.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lrntpqah.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dpnpsgdq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3riudlvzy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nslgmgfb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nirtqgrl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ffshzbnm.html


<!-- 参考信息 -->