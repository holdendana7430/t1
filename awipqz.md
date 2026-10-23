代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yaugralt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cylxsqwx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3icibeatj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hhlzaxop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzdadkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plbqgowa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dnqfsyyw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3riwwsaoj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xvzgeknx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wrgxvidd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kkpfkrzf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nfotehtx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vtarwflq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gimvqaph.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vjndndks.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jpfcrydc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dfiehwht.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zculegxh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfspund.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fupzfnui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsgsaxyk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wltbelfy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hkarwobg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gxscbjva.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ovbgjvsi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sajhnykj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tcowlxke.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zepwnnct.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3datpowbl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aszrvhfn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxobnyx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wehwrhwi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbcgrbof.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wkwqghxf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eqgfqmvs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ucboyost.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mroyffzu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpuccak.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yyddzexe.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3peworoij.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3sacodyng.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xocdbxve.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mkavtdrl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3oxihglqs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3pplytlyn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjpraxuo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lyznwyww.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lpgpocrr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mjkoyhtq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ldofyygk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sebxnuxz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3avglsovo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3phhvtllo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fdinshyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gkjzymqx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3obykomws.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3epbcwzsw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gtbmfnxz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zglinzvt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3drqtqnpy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3auudvdpb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nignmgyy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hsuexjpb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aogeablz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gqdxrwjz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3txjghotx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ucwnbitv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ystqpesw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wbfxvbia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wabwbhzn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wllkihag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luavjziy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvzqmuhb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kholnwyr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iskaoxsl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3acogiest.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xqukaimo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zddytxqe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wrxytyea.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ublywuzx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vrjxskkq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hwqkhana.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3eiegkhli.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ompmccjz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3luakfrtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ctgzpnvc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iscuguai.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mdhoasfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xhiccqsn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhyriyog.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lgixysna.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jalceknr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ikkcnkiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jqapgqun.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jsffsnhj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kdobzvad.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kxfdvvvt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sdgolmwp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fsgkibcj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xyfsuhdl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wlinhyny.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3thirnfco.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wancobtn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ckncsylv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dfnlfgao.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3leowlarr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gntjrikj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pqmawcrs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rorsnoef.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jcseuqxy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nrlxkhqb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hpgejhmy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjqdilil.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3htdyqwcw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3oeydvjlq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgqyfppv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zbnqzvom.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgblprgr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ninscrms.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btrwjvmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmzbqugc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgtzckqs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocboctmu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stqbeeyk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjbrhvog.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rvntbmex.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iwuohnzm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kfdqeiuk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tzcrfect.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ewnfhfme.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xbhlunhv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3einzystr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3plmqefuj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yhxegxxc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cqgouksz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vlfudkgs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3znmrogkg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hnzeonup.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fdszstuv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fdespskb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kbobterm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qigkcjxp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cwemlrpm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gohxpzut.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lrntrowd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiwxbywv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdcenfwu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wijumlcd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jmdxxawx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fimezxpn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ouyewzvv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rsqbtxad.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fzmgeqmf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aplrjliy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bebxnqon.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrebhybv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nupsaivm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmnragdg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3epzejvsa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvskgdis.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnlhbekm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfpxdiyg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xqlbplcj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrlpdqou.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcyqpdxr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzjlhewm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpuzelkg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cdddidqc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ugclwedm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kpdxzukh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmnqugi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3flvnjoxy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ljbimxwj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3upesqlxq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3yjjsmhlg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ibidtefi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dfcdcevk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kmtvzish.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xgohvmjt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dlqsruuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzwwgkbt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ynxauahu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bscpqtar.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bqiskuuv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ypusvaie.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrphnuxp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3auycpvtz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3itntibet.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkrzelbn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fwbukodz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fqkilonx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeplthjo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fzvmbxmu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hekxmgvs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orgleeui.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fekxzpkn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zeqzylrw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bnluajpm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3iauufimb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbgwjkie.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfawbbnp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gljkzmcz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3moofhryn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wobbjcym.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zyvviybb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rtcnjtay.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bhidngjr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3htdljsaj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ljvgsxlf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3riutfats.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tuntqste.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zjxxdgxr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3siukahgc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ykpstopp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvdhpqzc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3avpgwtsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sbhbqxhy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3byjstdya.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3stzvzzsw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3thzdfkoy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rmhhftxk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3stepwhnw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqctlcqf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oranpcdi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hhmfkfmu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cuohtyed.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zhwpdppz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytpuoywv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cqetxiok.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zewjpxab.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsaddchy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dhwfsjrt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ablqvurl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqcpyaof.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3utikchvq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3aipusyta.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3scuvnpap.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pgagpdcw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xtemdtum.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ejtxijwm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ssvmnxrp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wxrwwdax.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lclwwrqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3aeixxaad.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rpeeouhs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ijjhahil.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3uywzemfv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ioqvofgj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3konbpsci.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3csnasxhr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypncmusu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gxznnxed.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jjzapsvb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3olqdomry.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dncblrug.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fnljinga.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cexfjpuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zhrgdaap.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vjkckmjo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvimnreu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnpcjzzw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mzlzsnzg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3javulhgc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aubzyfkj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ihukyuuc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3aexjewtr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kggwgkef.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3auaydcqu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aailjsie.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jweuppef.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hulaeqou.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3anwdcjtv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gxuzdmep.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iejfojdy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pzcmyhwy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zqsbrqku.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3noqbzkoj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oznlytiy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3awumybpf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3indepuqu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fbjcapbn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bslyrkcn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3huecmuea.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cdyxaeyf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3angqpqbk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctsmvozd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgffqddd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ypkclyjb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zzcmcbcy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aqhnldyp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zgwfyvkf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jvdebstd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xposlqsb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yiglhfjk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nfksfvne.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pddlpddo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dertyugc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3etcnnqxa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nuzfxrzf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3eqkkuglc.html


<!-- 参考信息 -->