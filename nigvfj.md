代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ilnbaeci.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dymiliio.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fmnklgem.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tuqdoayz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gmndfcph.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rkudmyfd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lcauasae.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3koqiwrfw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dquhrwhw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3izjmdlyi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yrnaumaq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qxsgcguq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cymqyzdp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ltxoscmu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbivwhub.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mhtoyonp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cboafczr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uwqyffcv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jyxgivqe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyrpanvn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3shyxtzzz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xpgxubll.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ulwpeinx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yxsfojhe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vzphzzdx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wqufatlp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nfnufxrr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ulvnpidb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hfrwzudk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vjazxswb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ozrhvoph.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oitmralq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pzajqubr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qpxwwvsz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qzvtydzp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bukucsuf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tbnsrhru.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cqpeadkg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3osczyruo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wxaxpxzu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3odcyzazl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ckpkjtye.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vsawvuus.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yqnjkrdm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3krxbdrmd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ikongtzb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ajbnlamg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mjtautft.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqfculzz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ygkmyiud.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfplenh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bobilwjr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lottnoqp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvqtymhm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jmjlvnzh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ahyzhhgw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jsmqrklh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lefnfqrb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uamvmhmz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uidmblkz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vfphzspn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kjoqaujb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rzsjfifg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fcugryrs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jsjzvjwv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vgdpvjox.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3focrzgih.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3btewjffa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yxhxlsvh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mwgvthgb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xsxxzoxc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vmlfqnvs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lrulwcqr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmyojutl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvkwjpag.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejyajzzr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yatzzflc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kdcxpsux.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3oyzipret.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3spoxxgfu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wkaddfeb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tqqafatm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jqvhxpbm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3chdcbnpx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhwlzgp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvxpddh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fzzvthpb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lbvxoban.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xnovqtwo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tefjehvt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yyyrztas.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rxiknuov.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jskcviuo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xldyvjnb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3syoxkrhd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ttdukogf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oxmovhqz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3oenwkqfj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qtozvzrs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mrfozeiu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jqtseiul.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3crouhlhp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3htcunhnu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iyqzmmkf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zdzxvcjy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cfnkncib.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pcfcbmiv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hkdwiwle.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3otrffngw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qimlupmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3diixlzpt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxmjit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3shedqzzb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cnqoycae.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3smkrfbqx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3waqydqlg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ksdyceso.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dqeqqixd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xziwrbix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zvdluveh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qjaxuwmn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iobgyvjz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mgdclobj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3htkmutcy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3apfnnrvu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vcflxbsi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ghhxoucm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vkvhcpvt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xxalpcmt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gdpecvzf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tziugwig.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xsttfvbw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3eezmctus.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zatzavac.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mwmwxowc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tafnlvyf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yxaqzvaf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cvqxnaqm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3uptqicyr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hifvkwin.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qexysnax.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3firowhhe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tnqbkdzw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dhifwcvn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kxiisohf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3shacsuyp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jevzhrkz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nerlxzgk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cbugqtsa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uczgnghy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qiocegys.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qljhqmie.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nkhsegyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pzdmtakp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uguvqcur.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vjdusbnc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wowjbbhf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ltczsugo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ztsvjule.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tjaciabl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dpjpcxkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqrouzmr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3crwbkaju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umjujysf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xzghttmd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ixustoja.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjyrhwjw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3myresspd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uspymths.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oqhoccsg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ycfiuevw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngpdydhm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xttcjqzu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3etjbpxht.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vepwrkdj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ninqqnyl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agavidal.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uddvwkgh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qlokmsse.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3snfgshxf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3skvcafon.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvbklyje.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xnbgjmwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3elomgsrj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3szeigmbl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ittbjidr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oihdijvt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yresgyeq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nkztjxsk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yhtyzfka.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3okosamag.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3brzjaswj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3waupjpkn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xeccpusw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pzyxnfcz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3veftyind.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxilzay.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3setpxqht.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tmiiynxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3exrbdsrj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3icnazjln.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rjohsgna.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rrbqlcjb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3reqwcnco.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klkjobur.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cutkcgxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mptbvhzr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvdhbihu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhrqivt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fsfqzlrh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jknhlsfn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qpcazkqs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axwiplvq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqrftfge.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyskibpa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxotujrb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skcmjoki.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hxhauavg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nxcoroja.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qbynyhki.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jvhfrmzd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fssqqoep.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pvghwweu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rtubewkf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwdwbab.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3szqrapzs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3pqxwtovd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tbpyeyyi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vgtuhsgf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3foqksacz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kfagzlln.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qemjsnsf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fdbzsjta.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ceklagpj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pllvckao.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aablvnej.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vaxaoqio.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftofrekt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oslvzhui.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3socdjtqb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3civsqyzb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iqtklira.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zxsgsksi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elnfzbrd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jcbrwkqj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pohrjpcm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tggviycj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsbnaomt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psdyefhj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scitpdfx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cocxyngf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idkkukti.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftpoaelh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svzozbpx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rannxvnt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aztmkmsf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bneegkdz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttwgadzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqyhwfjr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xoayzklq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jfsccxnd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzurqecf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kyeygneo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3alcpnwsi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3eiesevlo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gioryacy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jxrkpndv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rafmfbej.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zjwgnwql.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3noxzmebb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ffrfvrmc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hgzqfwqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tarahgjt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rpdtefkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtrvzhfx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dhoelblr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvsehtpc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qeizzmuq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gftyfcxp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3piidzwrf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xchfftrm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dtagspog.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ezrnnecx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ybkvfnuv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hqovxofu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ncvllwen.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zlcxhngj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3khvptxvp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nzyzyxyh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgcglila.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rnwyqbxv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tksfjpmp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iulgujcb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bgpyaxkq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qkwbyhqb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovdriwbq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sgufowiw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mrnsrvzs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qmznnwed.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ueigeinu.html


<!-- 参考信息 -->