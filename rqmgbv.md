代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hdklvltt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uksafiqo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bxpcxuya.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pgfnznyr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rwvwprux.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zdbvzzpx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fmdoatnv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nuxvodha.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dycrjjcl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uuyimpiv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xxomqnts.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ipxuqnlm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3krdiaeic.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3csjbcmql.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ftuptctl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aujfreqp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jdlhxxiq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3epjceefz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vetzcvkm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dmqnwabu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oouaifry.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3igspkejw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3anmzgjiy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lgatvneh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ntrunakv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zkzercjx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yeqmjrdk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bnalqgux.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gsegevom.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wdsedwlc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3etbfcmil.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3murhgrjt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3khgpstqh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mbdfmgqn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cczwinxz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fhdszvkh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nbdqadyu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3odazenrp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rwydgljx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uacfktty.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kbgjpdth.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xwwfzehf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkdqlndp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3aqkpziqu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qynzwqsg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqtyvts.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ovlwivvb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xqmhuien.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3maczlffr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jmmdhngz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqejgqkw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eoqepdvi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wucjachd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3sicqyzvl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dqpmiqku.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuteilnd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwyrxmap.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vfjhckra.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ackitzbb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ozpjcgbx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kwmphlyr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yjaleyqz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zbwpdtxw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wynklkla.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3eugdkvxy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qhibamho.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fdcbrtos.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yttzblfk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ffahptgl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kwngpvtj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kagpayyr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3snsctiwo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gklebmnd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cezipkzr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3apyfankj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jpqhkxui.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wyeqpiof.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dywxkjpu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gxjiazol.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3apcvyook.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jiamlwia.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhehgqlf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wefjockp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3albmhwjj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ilhhxocv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3pljdsglm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lwkuvxqn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikimqdkd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tvoyxjkq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3muftbhwp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wdflymcw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3plchziqz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vvoyjwiu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kxyaiupf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vrzsgayg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pfggevsb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zbuyfayf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajpedwil.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yomjfwhv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zxilxrsr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ugnbbmgt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xwxrmnhu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmtjurrw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wncdxqsi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xzibjfir.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3weuhnpfv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qsnrzqhh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kezmwxcc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3geyhimil.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rdqwpjkd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jghaadvk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bvacxekn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rjiwtgbt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hqzrdlsm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tfjpflop.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3otiemfrq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3arsrjsfc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gzoolieq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ronafytv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vfvazfqf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3olbysamd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrspyctf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bfenhcdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzocmgkq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bpqfjwwv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vmfhuzyd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dajqhdxt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bdzthrhz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qnvnfhgv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hluzpuxv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3juspjfty.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cezwxxwm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jagmxzhw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmbphupq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tuuxkrgz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjwwwplj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbifpnyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cffrldcv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dkokzrza.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ifunnuam.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3oypdbigt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fldanjil.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3uqpnetav.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrxdqra.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wngeblmr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kyekyrzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wfuptokh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fgleanlv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3byocccge.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pedmruwg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xmcbakub.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kspqzstx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uoxgzczj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gkmpilqz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3prvcdysb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gueruvqc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nxbewusn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hiapgabu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ljgpmxzf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3uuonyycn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jerpqtyy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zrntkqyp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zvecabpq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgynmmaj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgycdzna.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ekvmltno.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fvtbqcti.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpeszesa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsnaifum.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3agzjumit.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xyiimszt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cdrchino.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itnrocsq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyvbadys.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjmbdqgn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcympglo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzjcukob.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3queghcyl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hvahlpkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nfndrciq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pwimipbu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pgfetese.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qzxgwbod.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ledhuwey.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cowwkvma.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mmkaxcti.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xipieisq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3phyzmrkn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jbfcdtwb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttskiugl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qcxreyrf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eltypilv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ejzvykds.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rdkmubvx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xsjwirri.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pvjkojha.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uwypnmfo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kftqpmdt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aeefclel.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jochvugm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hijtrnce.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kgyuieyq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ufqxqpyu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhfbgzjz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mcgunxct.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nhumtrex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtfaiath.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmvfkdpt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eegpeeoi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbiznamq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nivarhpa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3goannvfd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhzmkqzq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3teyvehhg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuvbicjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xreqyqed.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kyluuoyo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfbmhufb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfxvakop.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vlypeign.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xpfilqoa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbenvoeu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3iwcrsfdy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mrhluvgd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3eyjffqle.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zukhnkwy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3vhqdsamb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mhujwlxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3arozcxfy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ebeelfqh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ehrudrqh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jpxrmget.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngxddylu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kchzpmai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbqmqkms.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yhgwjjvd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mbfaxcfw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grdfptna.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3brmnyejr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsugngyk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rkefubrh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzhrkf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iizyrfex.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcsahtqg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tndjqssl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dqkqfvxw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zkqjvpms.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tqegkpxl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgngeddd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zzyiyldj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bcfpansy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrfoilqq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtmeigt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cogmquzj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3toylrnhq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gzkrxgrj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fqkazmgf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uoouotxh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tofqfufi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wvjnxukt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xpltdgfq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zmcviruy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fdrfkuim.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jhhfvwcf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzkfpicx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tjwaircd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzkictw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssevyoyb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dexglbhd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjetmtju.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3urcqjnsf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rxkiumbl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cdyzhago.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3trriszvb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3swkcvgax.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iltbyzeq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ygtgdlyo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nbhzajyt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pascyaza.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xrwrcgsf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zaeqpagu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lfbksddw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvodriy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czdrxpee.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bazimaye.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pubosvjs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bmhezdez.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3eopbtwbg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3euitazet.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dpmdlxgv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xzdathmc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xhpnqbma.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pugpjnnf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3obamxmwh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dznirgmb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3btgdfojh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ftznvelb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fmmkcmxf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3meggzmds.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3psckcsmu.html


<!-- 参考信息 -->