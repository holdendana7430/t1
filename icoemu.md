代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aogmloeu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zanrxcrd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3klaxzjmi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jorwbypz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmgmywq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kpnapakv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zqbshqyz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mqtfcwzs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3crnofnmu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yyasxkmx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pdapgiui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pekwywdr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lxhaqgnz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wvnnxoxd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vaobmlvn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yecjgioa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rjdfymjy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rmvyxudx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ofsphffu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqieaiwv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jnrojzzj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3prucbsjj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ggemaqyc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yntwqzjx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3goktjocl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fhetxybh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gpfyepny.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qmdwixho.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qytoyuka.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cbeomkud.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ckfritke.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmfssmjk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lqnhejww.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gonpzwxe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xudbdaje.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3neujrdth.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lifkojyy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iduabebp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcicksss.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3abjljqmr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mpabucpm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zntykipp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zlllgryk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mqcslptq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3pydcrgmm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3edeqzuls.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwhevgod.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3avucrcdk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmeyehum.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3htnffwga.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3heikluya.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pmtrxxeo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3piucxxum.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xpvolfub.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lcujbgjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vicjzcss.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3psuzuoxi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tdexvyxs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tswbrqre.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sawctrnr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jbfdaasb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hoygvwlv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fhfwnpju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vutrdufb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ojnayour.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ihlqdkrg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qpwlnljk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qmcxjyvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3edbitxjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lympefud.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mfkeiamg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzkvfhva.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3acqjxbke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3iekvhcfu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qkewujsx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xbfqczog.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xbfkynyn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tsnpsmkm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pmxqdwsb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkcrbiug.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wqtdtnys.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uecuslgn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3udarkdrw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3oczvizqu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3alvbvrxn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kakxahcy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tvgxncmb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jjbxkaoz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3banosbuw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3azrtlfid.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3aolgikrw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dsfyjwmm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yjyqntbo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kgymlwyg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yaodjddh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cgcthygk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qhujzsyl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hwqqfmaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tsgdfjfe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kdhpvkiz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eqoezyhb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rkaviuzu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhybuiod.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vitkachj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lmmyjbnw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3igaykrgg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fceuvlie.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ucmugxqt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3njludffv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3niqiwaai.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3syyehqnh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wltrvhke.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igrljrza.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ubqjtbjg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wgyrdxzu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cafafqhx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3disfdmed.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyvmnkmx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byzubzdd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hnvlysbe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixckddjg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhczplcy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3whunccog.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uknpxqxe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qysubfaf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tvfrmwnn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3utytgxos.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wexeryfl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mzmsqkff.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nxmzrwuw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ybrmajjq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qjvcxwkt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nkudgrxe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ehtwmbog.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3abvfgxyt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3fwibfkyn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dvopjtyz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3otblimcr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxkpruh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ogbcgrvo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhkzhhx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3suacnkea.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qzfupbqi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kvpdouge.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3acwsxrhu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrwsjmwn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mzqhvmvh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pwqrmnrt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wqpcxcbz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cfsgyrdw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lyvqklxu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksgyttrc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3utisfjnj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qsdeqefw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dchkwdeh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3piynvazz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbmzznnk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xripbxim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wkdeyqik.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waarbilx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkpcyuwx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azylomzh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nrhfvgoc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3msevxstx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djwqrelk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgpmpmrt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ittfrzbe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sdseizxs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cmrhdutw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3awdbsntd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3txfimpdx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uxlvjzlv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qtvydarw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pfldykow.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jzvlcmsg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ltivljzq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3thoowckv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ujgcnkzh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ynvaszka.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ogqrgxdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caqgufpn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3nwdujlhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfczwoup.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wszdgndn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwsulg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnivkfti.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aycysvvb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehcxlwhn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wegelsum.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ssmularj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3thqbuklk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3flundftj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3funhkwtk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cnfrssni.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zybxqyym.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgnwcxup.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3swjrfcjy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiierumm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ansqwytf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zofpqizw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sqndeqwc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hatvxxvq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sdhwiudm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cglqigdc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3svsjessw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nsqnipme.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vqsaklas.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fiubruoy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iskrplrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zvmsjeuk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pbkjisdw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oxjnlhhx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abmkxbyi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gtyuutre.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igghouwl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zqwcetav.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3snadoknm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocfsfzla.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wakbnurk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ixokcaly.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jilnpemo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhxwnupx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kynygdhu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3joqfsgrp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dafqjbll.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pjuuguuv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbkvlijt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3decdjmrf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3smtearwq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cuvggzrt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkzgfxi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jksjhjpt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uiusdzby.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qqyrptfh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ukyhbpci.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3udcbtffh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qakgzvqm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mlphohkw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qtwcvnoi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wfaknszd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qyfaqhiy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ojscietm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xoyhehle.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kxemuwwo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lqzajrpg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kubwltfx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ltfopfdb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qrlmgcvr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqmfdfvg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3szpdqrpq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhwwfmbl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3svnjbbbj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3leevnbzq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggvejyds.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3klvrutmp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uwmxspng.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qeatfzhk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3feuluhjh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qctoxvaq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrcowtoj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pxrczodp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nhnvagep.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zuzkutxw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cykmuhxc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3epzwguaj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wdwosqla.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rdmonhtp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cjrkoarw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ufpcjcne.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ztssfycx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pkutmowz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3trbzvuek.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mnxtepfu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zdpomkme.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bjyqgucz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umrdygka.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ecgqbeup.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svbgvalt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfzjuqrj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rqaagmix.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hvhnweey.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ifiuqzfc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kuxutpdw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3godsvmpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcjqdybk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thymurzm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqcotvxk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3igmiaath.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wzwxpqah.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nydvjexq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jsmikxfv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ejonfnzs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lbwpcxax.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nziikmxs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kqsshysx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bmohitya.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jniqhdie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ilvqekyt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lojfuogn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3seobzcpy.html


<!-- 参考信息 -->