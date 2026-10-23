代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gbxezjdf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yygezwih.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eqxkbpqj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sxxnmgji.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ewqqgzxt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzccnor.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vmkmgxwe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3arykytna.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hkilfooh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fupdffze.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3usoyxmap.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txbeaopg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cgwkaasz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yrnwavbs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gyxtwswt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kubqeaxz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mnyfmifn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fxywpsoh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zgydqkpj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tvqrmevk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zkalmeij.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sedvrbcl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3irdcvfvb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wqnnpajp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nkomrlub.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3doycntad.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bctojzpo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmahbnen.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dxnsftiu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dyzvumfm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3upejfgwu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ewdbbazh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3apullvkr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qnqvifbr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qigpoton.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hxmfkpix.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vfctqnpq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3obtrohkk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmcmnaob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wueemwss.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uklmamui.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yveltwki.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3epmddoml.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bclpozdm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3irrxwjiy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3evrcwohe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pwbtggqp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxpdwmwc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxaqgklt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3feuktzdl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tmmvxxld.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3symjghss.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wjqwbrdx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wyikwfzf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mxibrhcb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzjcxsl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thaudxwa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tnzqokzq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3oqcfnzcw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pzxekibh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sjgcvsgs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ufeqlgag.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upginftg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ppceklgv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mikhqjvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eofbvtxh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bwyvwgtk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmchmzdy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtfhqgyr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smessnyd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fdhxveey.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nqqcwqqv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cmerucao.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3prgqpbtg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tyzehjaa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwtjdil.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dkmmbica.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lzwqlohl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mqmvnxvt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uglkqyff.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cpjvbomb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3abwgzxyk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlksieov.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kguqmrej.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrurqcak.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bklwyths.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xiyzqaxz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dwznazkd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3flaulmat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3moacecfe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ygrwoifw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ohukqons.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eejvhnhv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dzwqldxz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyrigqfg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yjdwoubr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wonrcwsv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ibrzoixt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dkqfhnrz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3caiohooh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pqywakpg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3slmbokql.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kjsbcrwv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3glqapcmr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jokstfgm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nwdeemao.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nzqmhnwz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tpqspivr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ghhgftxm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fhjaitlu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3szozueey.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bmjrgngp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kplrpwpr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3onznwrzo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvqwfrbk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gplzntfr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zlocjrkj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rfelkdpt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3asrzwndu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3issccwvh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vemliyqh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rtvzzsdx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kakkhvcx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ffsqhaxv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qtykncgt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vlrhephv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3illckkqt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hrbyxxsl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xoqssybs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3haekggpn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qaiktzgk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ilfzjcfy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yvrcqrfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3petbhfdk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pnzabmzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktjeuapc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pqtpszvh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3eyisxvqj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gonpmasy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3abrrnyij.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3unkgykjk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vmufebui.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zlhrqekl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wizozpov.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qnwkfdzz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwdbbpgp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wpkhhvhq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xgqtcyyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoghwska.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lpxjqhbk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfuzzpi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3coucpadl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xlcnlium.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3iajrngdx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oewcoicj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ygpprgrc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iemytyec.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yfzixwiz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3frvzypba.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jibwskfy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzfdtys.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hosctmrq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hovzpbvg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bbnbazxu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xiwhazzy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3cnhxqxlm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3oggarpgh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3drapziim.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jepafemj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wmypfgwy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwlzadg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fuymfguj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ruvppclh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dyqrplsz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxnitpqg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sajrprmj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfnipvts.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ytnrhaul.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mukhforf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjwyjkwc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtowocmk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3netzdyin.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvrwicqz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xtekkztq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3luhvoocx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbghxkkp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3smuxaxvt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pehvvwjb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhvlsfya.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tlktinlb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jkirjmhs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yzsebync.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hzhuuugx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xatskdej.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wsziqjds.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yrndyhjq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3efmrxkwo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rkgagndb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qxqirmsy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zdzdfggm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vfbkfqni.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jplnrnpk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yckzvova.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3snsjnpfu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xxiyeggk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3utwjozbh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbkdqniw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kzghxbhg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ptlyjtzv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpgcfsxc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vcxjlhvu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yzzoswit.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gbbbuvuk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nbsaiixt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hraawyex.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ispwwfge.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3thneuuyf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lqcfvxuh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipvhxebm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3elexyvmc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tewurceq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhncvhkf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3htwoloou.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsxdzwlk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwwalvee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quliioek.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tihwgwae.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdvbjhol.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjoqwwnz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlpjegvd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbbyqpjd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ghaytkgr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3djkdduup.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uxioawqd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oftrfwwj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ikuajrbr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cuijqbwi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mpnnuptg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jvyvwiyu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ppyfhtzo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cpdlbftq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wwzidgbj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ygmeypht.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gcfqquqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjqeopgz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kfryqbnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrsbdhva.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3svlevtad.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mxzjutha.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3guamhglx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmrbqdbo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrnhidc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgnwjsyo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hairiwur.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fwqxssxy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkfgytpx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3scwmafqv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cyjfmtli.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3desxyoxl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qrshawoc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3abredqci.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zddizelh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gojwfrdj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3evvwhigp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ewgnpvzz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lqqbgaor.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3necngbjh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kpxzajfv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cujtlrwo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3alarudlg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cxanjmht.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wjmhhnqk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3scjizvtz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3plzdcyto.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vvblkrrh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jwnaoirj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jxyjxvqp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfuladdl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkxqlzhi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqfxmucy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3itrpvcjn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfmqfsxp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dfvxqklc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nwayrsmp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lxvbkoki.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgndtqye.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlzzjaur.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xsrwfgwf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ymhtnriv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3miajeuod.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3oukmzzcx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmnkuoro.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3flelxwdo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zpowvapl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfiyokfd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vdrhgkei.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mbghkvrk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3egehlkzn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3keowsqsv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fsxnlryb.html


<!-- 参考信息 -->