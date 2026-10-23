代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zkcoacnd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3voqzamqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3agoqmjro.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mxqwlcnc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3okhfakfh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3clcwxhqz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbhpurd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3falctmlh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ozqhhlwy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3glcduccm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ypcmurok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dyygzzvn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vkkeptiu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ybkmbnpi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lsognrxo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nyjlruts.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nhfsfwdu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yduyksqv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yumfyxzz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pfpqdnru.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lkhxhoam.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ucktdfju.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3reelhsbl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bcuhaqhi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hphwozxc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jnzisngc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lnubhtlv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3oodzbebt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3iidihgig.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tirdiwwv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3agmzilyc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxwimbtu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qzcujrmu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rmsgfrtf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pfbnaond.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsutrpk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3beuxyydz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3loywegez.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3noogchum.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3symjkofa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fqjxfghd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbjgicav.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vletukqw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjrhcdsl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wxiqpxdm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sbkgxgfv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zotielsz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cwimrtbt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mhusqlzy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lqhlnemz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hyonokxr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhjotiti.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cwmqrvvd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrjvqfs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3prkaxcmq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hrwglgwd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpqzcvsk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eutmvddn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ldspbuay.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eslqhfqr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yeoduvfr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hungrmks.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahfxjykv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xfwkoiud.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ksmngtsw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dngqktbv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tidvehiz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rwhuhpnw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wbzrdtbr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ickdmlqb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pqxsxpyx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ztibzhla.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sabpwegq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3khtiklzg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdqsdalb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3olgchevm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3khqgvhmu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uhdhptdm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iktlqrjr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xteeyhnz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nemeekct.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tjxfxzwn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oimgzfxu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eayqtwuc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oeelurrz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3laqgdxtk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3whvulsjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zzlhcytb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aufpxipx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mxxegnal.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zjpdvdae.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gcfxqvlh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ptcbmmkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isvybsui.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dqbphmgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mozfcyxf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iheucgin.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hntpbpyy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yzyqxhew.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uxpsjewo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hqbvkpzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ppkmeozy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3trtugwex.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzixpwxy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kuxqktwu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqrdjsfy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3elwyjmcg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xllujqnr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qdxqwxbe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ckvvqqah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rpgapqti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rkqrzdgi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ltjgxvcs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3urgohtmt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3aqckylcb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tiqdnvjm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mltthvec.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3plltdayr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3inzywbeb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dtuauhmf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yoiuodpx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rofypqsr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3djimkqob.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tggdxaxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3loffiduk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pbydvcpl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vpsyzphg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nveihmke.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iabidflw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hvhjpqtp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3myaqtnej.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tmvekqvx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mygkzkit.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dxrrmqmz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxayjtpw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxsqfvzz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxapfqqi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhvoinbt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3stdhdtbk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoimkoqr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grbykwlf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rubkdgnr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mygxmpvw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wjdifosy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kkteaadf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdamahke.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwsfjuxn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqntjwbu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbdszbcn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rwbyniuw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fplvliby.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pbybqbzq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xafffeqi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3crcxxsms.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3venjlkus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ckojccdg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3njodqkud.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ofjbkxhw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ajfhmzji.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zrgvnrhr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nigfwksd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3iklgckxo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fhjpgqtw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jwgovgdf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sippeavx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pxgtbiky.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3psaplnxf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3isnfkfvx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nelsxveq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rconxwih.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dvhlscgg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yozipzvi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iyniyqsi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3crnwglws.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xjkaehxl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djmkaktx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3whajsqdm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pedbrdam.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3taytslet.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oeagonou.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zilqvtrv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjmyctwx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dgvgaqdv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjarilcp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfxeumno.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whnrzunl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgoxaslu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijpyykkw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ruawnzps.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrbgicfc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcbxefwp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bggyveef.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3eekrinyb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whwxdmvj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bqkrqcku.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ejewtysr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iqzhefcu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3abrvelxf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qqjlhkwx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uiuohths.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sjyydcnr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nonqwcjy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3alszbhof.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rmwrcvnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmsvjlue.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3extydmjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cklzwibd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3srwbbmsm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jeapaqjt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hlalsymm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfkomwhy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ubpgslgm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cvhxrxhb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ixxiyodf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3shmdblsa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xnpmhzbs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3maqnjppv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jswujcbd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntwvhkhh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdbkklgx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3itimndqx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bporefzz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jsvkaybx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsqwyhxx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhfkeknl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3amsbmzoz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xznhopmd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aklwimzh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aeiszasm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hbrkysdf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3egbhhoxc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kiagwbon.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hokwyqin.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hynpngsw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3peoybhwi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nyosvacl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezogiqbz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvdvhdxj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utuskmbl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocnlobwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cdpfxabw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwdroj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3csyuafom.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wberqvtt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bzacrkrg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3azlvxjfg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcqithnc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kpryvupr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fjnhhxif.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kksszwwr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3omhslqyd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bnytywmw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wvkmwspu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nqyxnqmc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jramwyby.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nunibjmt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vqairnhy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3txcxvogk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3owfauqjj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lxueyrcf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3afhrtfgh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pqswfhed.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kigthmxz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lpswdtcl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tussctjc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eofpfjey.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kzqdcuqv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ruewpnne.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3sriznvyb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3axgjfoxj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wmlwlegq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xogtoeif.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ottvinel.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nthpewye.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgxawexr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oknwvnat.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3humvoihf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vkyhtbon.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3taxdnaac.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3etnjfrvs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3sfekgiqn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxkjnmm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jphsnsew.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqlqpei.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xypdifmn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ffizagln.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pmufldiu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eiehyzwn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3eueqfzsn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dlkxuvhn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vabedult.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dswbtafb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cbqbgntg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yoljiyuu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zniemoci.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3irqeuxgr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3grwhervy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bykuppss.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gtvbzkkd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjjkgtyz.html


<!-- 参考信息 -->