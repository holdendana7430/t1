代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3yicdenxw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3odvfnrtk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wfpemwuq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3imlbavaw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hkgqyjbu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xmslerai.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfqycxm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3waqarflc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kcthsxef.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3holrqdkx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ikpejyxc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3epbtubjx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzweuse.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bynyzoyx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3umeouwje.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3idonamhr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qqsfvxmm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dwmifayu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdmmybn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3efnhdurq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ckokzqmg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3etlmhrsj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dopdahxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnurpyrl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rdnbclur.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kyxvkitd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ngzgnvun.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jmslygis.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3lawpewht.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pblnfgxp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xymflctk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bundyanu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fzcgpdhy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tafswnpy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jcdltcwb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pxipobpk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3xhslnkeo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jlreltat.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osovhnem.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vnpdcwzf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zwnmdmmx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bfpfsnyv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wrfegcpy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mqohqpbk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3heueeamb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3znbffvxd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gisdscjv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iviuvasu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qfszoydt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yivwwrxm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3awexnive.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ahgnwadi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3veeyqfrw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xthrbusn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yckmyfqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bbnjmshc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ullwbpoo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqinlcw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zwmwxvsk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3updrgabc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pgjzobuf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sxutkbpy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qwyynwtr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uzvyltuo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zytdmlon.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xtmtgmxp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sffmyuuf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bggncamw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lzpklqoj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3anjzmpru.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3secgvxpv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gpzbtldg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wmqrdmqy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yxohustd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eozdbrxw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zudlfxuh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jvjsmitb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gkrkggxz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iojioggk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ikcjadxk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vwzaioln.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fxktjvfz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3afqnjifn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ftrwsfis.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fgtpugfo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oztxcyod.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ydingkns.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yyahvzwg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ehgfnyfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymmuudie.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mhcjnqfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afglllnt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3crnwzzpr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gtdvdqnh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fyygqszd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wwcumyyl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bgltmysd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xehyitww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3secvdhoa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acyadkee.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlmmjmep.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocjlmqms.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ecoxkmbr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvualkis.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lzyxwnfk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ddpfzhpb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xxnjnknt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kxmdavwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dqjdiwsg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukyxdsyd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3eqmxkbzn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nyszpbms.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uhcbeqwt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pizuoake.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gltgmmvb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xlevuuvs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3txcdbzwz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kaszqstl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nfbzllci.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdrdwjqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3puicnujf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3trhihqgz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3swompgvw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kjgdthms.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jauccmxk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjtwmsai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqsokzgg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lxwomdwz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iobpfozw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gjlsvfup.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cekzglod.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdqvorsd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uccsgpja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mgrklzjv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ndvfsfwo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpcuhltk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibqpikfk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cfwffatv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cesxektr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3obqapnyr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddnbihou.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aautwvch.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vrcghoxz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sncvehcv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxeskwzv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ibmfjzyd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cltrogaa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ejzojjgo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xorndtgv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hskhdegn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qmzdetbe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lprgcqcq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxgwsoj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vuiiipem.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gqzzuvbj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xaewuquz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cxolnuvq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3geedaorp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ozooobgj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wmgecmsn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dciveivc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dcrkwewa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kysuqrhg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ealilffd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dtpnoqgk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afekbtmj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nzdmuhsb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xvfizwfe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ucomcnme.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gcxzanfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ybulhzba.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svoohghx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qhfquwih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pnmxxarl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugocpiyw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bmrmelgm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxvtwras.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlepmyft.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ieenycjn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huqczzrz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iipanjyo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkarbgdw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qflsitri.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sewojkfy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kxwhwppf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ecbsnzgt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oygleoib.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkmeetf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3grpwjgdq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwdqghbf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yyufargh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bvbsnijq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtrzjky.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xlpytxte.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pahcffle.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zvykckar.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ctwfbkcq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lilcpkbw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vzneseur.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ktzadkmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqvnmc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zafulcet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsrciqor.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rmjzuqvo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3oipfnxmz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xqtnnifq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ftfukoaj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uytkadxa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3knmbzckr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vdbtuefi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mckumxpg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3owmdwutc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rlmhejhx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kmckogvl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3joimuupz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yxdjylhm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lleqjecz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hpeztvnx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wzccqutv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3euazrsxu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdicwybm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ktvtlwhl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qutmcpuh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3daozcbih.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oiszsvdi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lvrpunzd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fnusnvsn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sscjvjxk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hsshncma.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ansfcdyu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hbfkwxje.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dtnqfmkv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmpxmjhg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbvmpioo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jnbvytlv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ekkdawai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yzoptftn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcdxhbpo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gthpoqvs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3utaercjz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3slitpskq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiyhivyw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3paeqdktw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wvddeouk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwkcwvhb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dcjdcokz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pcvuovtp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikiqzcal.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bqgfisiv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jddcobsd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fbreyuci.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmjvsumn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiihpojx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkgughy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ejvfmhdr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ckrtxoem.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bkpxaklo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pyqatvyn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hrktmvkm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pfrcgdsb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dpczcfrl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tteqgnup.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ixgvtcch.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kynebdpl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bwpwqvky.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3scajpdra.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3axtpfncs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zcczlarz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ukpxbhot.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3oafzewlz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mujphuwr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqbmddgn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pgaceojq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pqspltrr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dahjsjpz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zblvpwul.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pgudulpk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmgzazzl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3akqeqznk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3norszupu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3izprpwsd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rgfsdolt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kuybqnbo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3sjlsydbf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rtzctxda.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3upbuprov.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lbrbvqws.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ttfiqhve.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qppfctsj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uhomkelm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yqlyqbxc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pfablaap.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nnnqtckc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3suwpkvfv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gdlvuepy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jxwkhonq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwoerdw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iahhkjnz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvmyenxr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lnifbmuj.html


<!-- 参考信息 -->