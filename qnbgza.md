代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oappijtz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3epdhdmty.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3obhxcmrz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kukmgoup.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3btvpvcvf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhtjvvhp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lnzvanva.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tdvsdidu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wxalnddb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jymzvcse.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uvcjxiwf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kggfzuko.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3scrkcpgl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tswdfdpm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ippzaodz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fzifjkfa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gbgvtcfh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hyiniote.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tsuzkgmh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qpyodxye.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3piwkqyce.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3njcgjygm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ycvwxszi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aznmreef.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsexcru.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eifudmcb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yrjsrbve.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3elvtkpvu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmpjdlid.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gsledwap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3eaqykifa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrgfwjxq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ablrfqsq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3venxhcgx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gedwitem.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cydshkwl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3extyfbwo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdwgeiw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hesoulzb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ridttmgw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kqqtthjk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wxcrozor.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jieeawfb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzurppya.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xoawumkn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3tizavofn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3irneufhf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbxspsiu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cokqulqc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwselayq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wsbybkut.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jzkyuesl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uefxougj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bdaggoum.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lkfkekrg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wdxeezxu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3aixulean.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3unlwwfbe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hlprpmle.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3modfqewe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qonakrus.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkivdcsx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3slnmckzb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwnbfjtz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mbsjgbjv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wjjfqadv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3benqaqvu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hniaargx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yygxpaav.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ghazsbei.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mkhyaibi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3stpaejgk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrwtokw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dwwaxokj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3flcagogr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bvtxqpnk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3luvibano.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zcxdltvu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hrcynlba.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3blpqpdte.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mftzenjh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wjqiejcc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvgdqwrd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3drkainlq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ftltmnjy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ssolazjj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qrmugcue.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uhpnvjrm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3urmldbyc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgbdjevy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksrqvkgi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymefvagr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3toopctgy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3irfmrkfq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayuddbtb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yrwmjkpq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yuifwghx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dkueelmy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3itgipxnj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zanyvptw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wuxmsjgb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gboiesag.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fgrakqcp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ekqmopvm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zycnbjyk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvxjufvi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tzibrprm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3srszttzz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oskrdjsc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ftjejwuw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tdlpsoxn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eqaxenlq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3woedtzmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuksywua.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bxyoillu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofcxdivw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pczzbfyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3udmebjgp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlcaqfkc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rnwzkgyz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fjnecwfn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dedwxmkw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hdiobyfl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lksjtulb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ruyhipop.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3reqsmkmb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ipaijata.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3awsienoj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wqsxfjst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivgehcsn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvqxnsr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xbwanyrk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3uvuhanhc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ulyobygy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ryxibrko.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gtgksuti.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kphmyahx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tvrpvzrl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ejqayfvp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rpiykctg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3afzcmpfd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mbkchhud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lkqdixwr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hhjcbyze.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hloggvti.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3okgngasg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nwviymcv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zivgosvw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pzeddzys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3otifrppk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pxznnqjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hmgvrmlk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3slehyxeo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lzjfrmlh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zfxrqoyh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suwtguxz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrzyyvtp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3btlhtkla.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3glxaghxb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ousszzpm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrdyipme.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ukolrndi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgtwnaff.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3apesfuzt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3poqndpup.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmiemhgy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qufuapim.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqjthsse.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlfvrdge.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fegcygje.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zicbwqtg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3igpyeysl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nkxkoqvf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aixmxlgr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sudzmdjf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dllzxlzt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3epusmxum.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zqxmxlwv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lvieeaez.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rmwbascs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3abstgwnv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3senbywla.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ntplmkow.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rssumudm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ufwgmzce.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bryvbcne.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gogedpmu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xmzkkgbo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tlzfsvff.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxznjlkc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmixrfgi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qzqmthqa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pxsbypbc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3siagnogc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3spqezkcg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkwuqlzp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mtdhvjgy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rgbpzgie.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpureblq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xzpncbsg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gznwjcrl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imfdpeud.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3llycbnvk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfjiqjtg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaumorcc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scoecpjj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eaqysgwd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilcqdbuu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3foidyfmo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qbxauswu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlkwgyjm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3olzzxgem.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3louovcvh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sywtlzfo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mqxjelcx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wdwwwkxg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xiibmiln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yduvasyb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3murlptmc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jjikpvis.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qrgxynxo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mimncgcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hyifwacx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sxshrxph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhosrpbu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dzosbtfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfifosly.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zxvlznii.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vqqvyovg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eslutegm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oposlgjq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rilfnoxb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3umtnvnec.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xyfcoumh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3nqyuauia.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oxhabwop.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oelzuhgf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cjwuzfvy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eakswpmk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vciebzpp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaoigcqs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiduyxim.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gcmxdlqi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzoydnad.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ogdwazsu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rghjwqjh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yzqtwovu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pvesylmy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kmoltxgk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3kcgloyea.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xtfduxic.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jkjfxbkx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qhizptjd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rdzgxbkj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3svrfhkcz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zisnxmcz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vphcqmlm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zflfclbc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tnluwblv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3epvffyty.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vdibjpdw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cfwaqlpo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wbghumgy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3suxdztwr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dbpwwvdq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywlbikpk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fovnlneq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xxinfiks.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqbzcexc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bnqoqejg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldkvavdu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehzlgdgm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fmxjnrsr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hhlkjqmf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifyaxzaj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrbttzrl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dzpdqwup.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbjsibiw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3okexaxma.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3snfrayqr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3woazxzsb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3drkpzais.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ohqivcgx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kpnukpde.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mbbswtbi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lajchrqg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jmsfgjmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mpyouipm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ntxjyrli.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3obzyhwql.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xdeoiihx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lpnowqgc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nhysnofw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3opypaxfk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkgtdgtf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxsxibjx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zootehct.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ajwewjnm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3komkjcat.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wzptyumr.html


<!-- 参考信息 -->