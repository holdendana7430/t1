代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpjjnpt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qndzfipu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fvibdbfw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oykbhvbl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nykiewlf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cykysosd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2chqdhrsm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dutvgzag.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tuuxeurw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2isqpjfiv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2geqyndgu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ibgxbssi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qftrytbt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gixjkfef.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pcqvsbki.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tqjydokf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fzuqikcs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tozbzhby.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cikmxbft.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zltluwtj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bimwtvjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ktfosezk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zrixitwq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2doujrmkd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tpsqtodn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lhtrjait.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzcrbi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxtzaxk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2exagsnkp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hitbiuhl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fsgmkvbz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xmcjcsex.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cypnzhyx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ntxjlyyb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qbfbeiyi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fbcljsxg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2suweegwb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2itiqutqb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eonpapoq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2omeduyah.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mkxvpnml.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2egqjcjxy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gyrurqsf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tjsnmedy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kujsgtzu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2eznsfflj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2iztncflp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2faalrnqx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjmdecff.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wapkpnho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykltzwjp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2norvmrwy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lzfwlxnu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vooumexo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hufvljvg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2faajefes.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zygedrbi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lggwohzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2exxihtdz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kutsqrnn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2geetecdv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xsbyojlx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2omitgefx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gajpyqft.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jozpphho.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nxlhlfcp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2brcbxduk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vtxgjujt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mdzrynbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvzteuur.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ywoyweft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbbipzmo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bawwrfde.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2quqvwpaf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jkncedpn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pehndoeg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cadqzluj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkgkkzls.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rpbstegv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqbkdwcz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwyxyhdz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ucurjngx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zypxbnfy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2udzepngu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aicmasiv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrulhnha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nxawsrys.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwrakew.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zomlkaed.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bsaxbkni.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2eazttjig.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2njiutnmr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jqbxuuuy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iipukjhi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tzmaluqd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rnodjeiw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2akyluijw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nqvfvdfl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2leueutad.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ncsziemp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uzoycvui.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jcbimitc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fzaaalgs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hetcrwzj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ebevmncs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xcgjmbkg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wsgmqppt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nfapndee.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mbvnqnlb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lwirdyfd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmnpfadm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ednywydu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydjivlwp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezjyomfa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zytahzpn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdkmcgji.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frgbxghv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnqhzssd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhtjtqjg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxaghljf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdongtoc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bchjzzyt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ydtgqvdw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjmbamhw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckffylut.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xdzqukjc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2huvwhytl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mzmqyscx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hcmfwbla.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2srwhlmpg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jrdjuvip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2btschodg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2casmdpvy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gtizdvqd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ptmnwlzv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ncujvgca.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nreadowo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2soupkdqk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xqanpdwz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xkdzrabw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2imsgdqhm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mwmgsfxe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uzfikoon.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gcxappol.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kemlhanu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkrmottn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ryfbvokk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qipqgnpd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2btqagdqg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bgklfnec.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uykwrcik.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqkeflzn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zcjzntbs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pisqitth.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcukjmbm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rztuafep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzjolxra.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojekjhjj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uizxpteo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lecnqxhq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyneoqub.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqynwasc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfembrck.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvxbtphg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wtosaisx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewrcpfuu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyhooxtc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvupkwt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ssujcxwo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmrcefom.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fewzcjof.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2eqkduzcg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxojchz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mftctcpg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rolrywbe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aajbfvjk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2iocgxrmw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uuuksehp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2avfgnsfj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fzbrhyri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxggdqfp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oroogrpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdywhmrd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2okxwnjhz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pozruiea.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dinhuzxa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jgmljrat.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqelidpo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2swuwsdmb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mrddijev.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qeeybkmw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rwixfwqt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lndmlven.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hamlmtfi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fuqwhsom.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msnmevah.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2leukdvre.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ytmhiptr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqdyus.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlpqhlat.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfunuuk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yzxfepld.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oughjqok.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yrmbaani.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ozxprrtr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dubfmqus.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2enqemkfq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2atxuaogo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2utboxnew.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ogkujcld.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2opiriygy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xqjqbkjm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtpskati.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ozcixkie.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jioaggpk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxryplap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vughozef.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wjjudfga.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jhptdmli.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ydslsyfw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gtoesmpa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmxbobhr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2auewrqha.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bvppikqz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gidaggzv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2trjkzhvw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ladxuyve.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cylhlyik.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2czycwmrh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vxvuygnq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhpxczue.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eixvzhfg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nrsednte.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aimvoqhg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jrfcbmdo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlxdevwb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oqthwnaz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lezvcqpu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2slzgvafo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hvilamrz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hsgejtzg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xyqninuv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jkwleszg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xwqiafkg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gcrqqatg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kgydgnnw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iobiluzy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vhjjifnf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nektizsi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dhmphbxi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qywjkplz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtdwuzsb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mntlbfdo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2daukijzh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkizrfdz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ptlkcmye.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2housgdlw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mltdclkx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lremkkrh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvrulqtm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swhrtyad.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mvmmkpev.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zmcmcrvb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lpbudifu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tyjwavcw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2inhjnozw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2prvwikva.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2eaqlgmfo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mlnqvfyp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tiydyaso.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hljgwgns.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kvczgmjj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hvpdbhif.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qboveteo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ngirqzei.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouatryqv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kxwqvofi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jlgfwwbr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgkvcdru.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tujlengo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qhidtjqs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jiylsevp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gdhhnjdk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yymfnffz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dmtagwnb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zwijthza.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbytfgtc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msahupfv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qscepybt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wdgimdlg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2odzavpyk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxzcnduw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wxidlqni.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pucdlkwu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2anxvwjmi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uapboexu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wctozqbs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2efqtzess.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bwmcphgv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yhgbgngv.html


<!-- 参考信息 -->