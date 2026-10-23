代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3caxevkvd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfktdlnc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xqlbljpe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tzakjgbl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fflkgpup.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ofabxxym.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvclhvlm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cfysydlr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wqtztwcs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ipshkoog.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ylpziius.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sfxrzbph.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lltoxssl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3noonqvmc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ysorvxkh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3iikwgwvd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ksfilrus.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpgqfgq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fgxlvnov.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qhnrogfd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ffonsdov.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rfbqpebz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3etlbnynu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fkhpkdjd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lmtqbseo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qleggycq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3arwcvlqj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3shudipcv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3eazuzqix.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oglqwlpd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hmbwsjip.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dneweqtc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xqlodhkt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cfdkivms.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ubjnolim.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tyyxxcxc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oxmswmwl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikpmuqkh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fzvdscvp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3icwrejaa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jgomfakz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eiisvbmg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3inswdqlk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hdylwbok.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tqlgicqv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3daqyykpj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yuzsnpsn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nsmwozgc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jwslxjct.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3slrqlowi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pjqxgwzq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aeoivbyj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jddcojrf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uzrpksso.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jqhnfolh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wcjjrvdw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3knwcqohx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xwicxpdy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwqwruut.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ravzboeb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wfhhiqkq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jhrdfnwq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zpvjkyhg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vmmlnths.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3knqszwuq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3evlfinrd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3khisxpzw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3klleoeyh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eeqsridb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3chucxevu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fdwftvhu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbdmqbzr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qcwzzriy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vudqkeqv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mopwhsiz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfnwvl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkepjwmi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxnfknt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fzhtxjux.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdwqgsk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rvrlbaom.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zvvuidvb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tzgviltk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mpsmtgfr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cnolzsae.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xjqblove.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wqnjlayk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rzodynvv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3uqkrwssw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywlibumw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pdcgftwo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnvupfmp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ltrpqndz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bmpckdqt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjwseux.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bmajbhov.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3wdawcraj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3exzczmqg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wpbgatwr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kzonytph.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vdllrycp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3yzbgubru.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3soldmcic.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3odksnppb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3steiztdz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jjlyclru.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zwbfagef.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jtabhaiz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xtxvjuel.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ehkgxkje.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3okzpslxu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3monvehzm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qksjpaso.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3czafdcee.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wrklnyvk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xjvxohhm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kjahtxiq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3updfgtlq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fduqwxhl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3osdbbaey.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uovuriis.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3esswhpxt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zgqqkcrt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3azzitbyw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vegqswhe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ecwnapdb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gislyjhb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vwgrcexs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dxacphss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khuvsavo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgejfnze.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pyjkioku.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ohbyxkwp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3udbmoqgc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3oaedbxxn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gzrbzmku.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lenyqzju.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qwsvfuae.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hzkowvpi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qmrfpfga.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jmaupjya.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3oajnexgh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qlirstea.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zwsifsde.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kmbdyqqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3opuxjjoj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3odisvkxo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3soxfwovf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aeyjnlza.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3soequpgg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3suprpidv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vewrqzhp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gjkvhxfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkpmevrn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ikfndeyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebdgruow.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdbfkgqz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hzrzqjgh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bjvdwdip.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qwpojbjc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3svivteoh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyqkrcyb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3viuxptem.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odpwxejs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bwdjpecu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rzzcsbwz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qzizpovk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjoxtojl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qazhvceg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kprkdvql.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpdubmv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3klmwrsmw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nsowbefw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyvqwjtg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3srkapdvx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3easglotc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gadfrjgh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rbxvlcng.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3alqusvry.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hffppsfy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3viexwlsc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jgoqfvpg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rgxwogxx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jwsxrbvn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3szmhzohg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3csaduuoq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kfnbspmp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zevausqd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ileaxwgb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xqglkfne.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ypicqoii.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wayqiimz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cqkkhrdg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qnslkvcd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffkaotms.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tisblipq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eeplvbob.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fmdcfmkt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pvkrkdyr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3niqpvdzo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etojtdzj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qroxjeun.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbkmodkx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbxxlofe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tobgcxap.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btvuwlws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3osoglexe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkducjfk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tydnierb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hwzijngj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kflzvrky.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ffkwuhyo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qvoyestg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3feteziqu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jmgsyatu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffkgkfym.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qbdhsogj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3edohfhgq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hveiynfk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gdskaais.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3njoenbft.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3djxlygqe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kvcbvloh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hlyontyc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ikmtujzl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mjcjheqy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3uthofewg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jfvkyhpr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3irlqpryn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drmbehjn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrlmeabx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bfeytscg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qlkcfyht.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qqfjufvl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3udcxrhed.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcqiwffv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jayxukpb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hsioqfzn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrtoydsa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpwliodl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsqcluqj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvqgvaas.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lcwuehun.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kifftqwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwetsnnx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahbmuczq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gstlblht.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ineeviyo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3auxmdzwj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oduedzrp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrnwcbxm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfsvlrw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kwqnrant.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlvyvfcu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rkcznqpx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eueajwjz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3iydwpxxp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3owezzsaz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rgscvqel.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hkpsqrrw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gfwomhoj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mkrrmpfc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jehtvbkp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dqkistxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhydryge.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wdqnopej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyvuzefh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qejkuofx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hnakaezi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3abuuwoqd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jrdydkpy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uvoaojta.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rweatoup.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cdtwndwh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hdrpqqqx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jyqnonci.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zsyrwjrt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qaqiqrqu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ropjjrrj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itzpngfj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svqalalb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bpjynkdv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ikdnnttk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vghlddgu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hpzlsgbz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kviuosma.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pvvldpst.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iyczyrcw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cobcjdaz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3txdvszhc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gtgzwxui.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pwvgfduv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wocrykqr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3szdqtmum.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ulfxjeow.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fnsyinii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dfhmxwhw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpqoxzyg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hsobmazn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bmrguejr.html


<!-- 参考信息 -->