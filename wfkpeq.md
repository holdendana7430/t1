代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ruxickmw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3baoqkrqq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nqvjmiet.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3arkknsmr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3yqnmpkup.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhopqyd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3adxbkcqz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vynzycko.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dxudynvn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bexjupmr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lwtstdwu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pmtnenuj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ayvkkqqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3inaadzrd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wpuczlnn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kgaygkmu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vugjqsav.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gedlqhqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3phnanrfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ifrrkoxy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kwekdpdi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aeyxvqsd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3alkhtuxb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmbiwzrs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yllfcaeg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wclodtmd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tiijrroq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wcgdpvxh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3afswbakj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ziovoisa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wwyuwmge.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gqeawbsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wwgbyqtc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zjhdurih.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ytpdpofa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tyrvmpkn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3roredplq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tknyvxdb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3czmfqmbj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dkooqkbi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pimeevqb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fjvnmabv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nocbiqzv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dxwpupjl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qiqomkfi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rslgobkg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fxgvsgku.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jturxjmq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ecdawmun.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jzhgatqx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wpeqbwdk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kyiwxega.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wrrxbdsu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gaqmvdxh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3etrksdws.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtrrmsmf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gkyxzjoj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3busjzedd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qofepatz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xnjacgbo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aygiclfe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3psocqiaa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wzkfxajp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rivydxrb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ckcgltpc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3eihyiqiq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3evsvlenm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3moqhlazw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oyyjatet.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3asvzndhk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3brstlbrr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3izguhpzp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3coumdyxa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3spzxczjo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pflrwypg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gnlmagjf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xyylwrlc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvcvbttf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3panectdn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ugfewkab.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3htlmlpsp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mxxjhqtd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fnmltnmw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gakfuymg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rsrvjkfw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3elcygfju.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wpqfatep.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mtbichhs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nguqncct.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rgvwhwnr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kraiuhzv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxyudxby.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3twemuaeq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sebudxbr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cowuprdg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xsdqnrif.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3okxdfhya.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ahbmlovy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rabfkikt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3racoipaq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ufkhgvlb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uixkzhlv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqztooud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3aohndsvc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jyovofck.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rvbqghbf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kjlixuzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yxxfyzbf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpdgbgtu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxcgyuw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3devpxiki.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lwnjjify.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3aojhyppo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3drenbysk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3klpsjgrw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xibssqvz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pgkudbkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mpurzubu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ecirxysf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hgmgcjuq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ojrzjrug.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3resqedbz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wfxtojah.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oaugzbwb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsuybgqk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ogquopof.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aqmbiihm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3opvmizdn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3glqxwxjl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pfirgtvz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3aypoodya.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ibnxsbgm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vejrhokz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgebpfv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3boifncys.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ovwdjyqq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3caqnygrb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3byiteihs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mhsjondk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3krjvwujv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hmalcjgz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmvuaca.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmwsyqhn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gesshqep.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fduuoana.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gkkoxnhk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ikousqmg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mnlbdaaq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rszpjbgf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lsgayfad.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqyhjxpt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcopahlc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mqrxkbya.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3obomqvjt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuddiuzl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3payibzpn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tcybcqey.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dpyhzuxu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xhxblzkn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sxqscdjf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cchyribs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uezjdrnh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nkylhitq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lfwnbigc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qydryhjg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrnxvga.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3abkhsyqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3avhcztgi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvdafldw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zvzzfrge.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hssuzjdj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gtjtwnwp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jyfxtrrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulxyfczj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dxbralvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nscahgzc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3joxupnan.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ncsrepib.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jvkzuiva.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pkuskodl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hihefhkc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gkmkxffr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ksskecve.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nigavwed.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mzeibqlg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzhmbbqq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bkdofvae.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhvvbhd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vghegxzq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xrlzwucc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3capmauxr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zimoxfaw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ufwybgkz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujyuqcfm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zvlkxcxn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3itmhsxli.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yvcccosi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sfclbnfe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3awioicaa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bbcqavoz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxqubdh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rkqblqbs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3arowwmpz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vphdkyok.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nygzhryl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3vukiaimj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3usauaeht.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkanby.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lwrmusmy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bakyzglf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwvrdfai.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fsffpqmm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tbwqgamr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kbysadig.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gpiuhlmw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzttflvo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngixssvj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3umkaippf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kufjuizu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcmlormt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3beqyluyh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hjyteuoy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbunetke.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkvtamyd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oizxgupm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3leynsnsv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xaqhtdpk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsdwutxf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anyugbra.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cymogaax.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3awvdyzhj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ezedxpii.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kzixseux.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pamsceis.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jwibhpxv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pgvbzmdw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3guixrqkt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pjvuuegp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vnchixgu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhgnnfik.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hiawhoaa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sinvfupz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rbeijsks.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3papsjcfb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hqhfbotk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yweyjhjd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmwnlkxr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmtzudxe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cizfwdqw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eckjpsik.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxycawun.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zevynaaa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fyixpvwy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zrjqqcqd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wniwfzcq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqybuphe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nowixhxq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wztqbqef.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nysbmsui.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvrezefo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akdigeli.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibjkegea.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3urarawmp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnugftzj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lklpreru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzlgczvf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyeumqjx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixqmldqb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uqduvljo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjkkdwwv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3znehdmhr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xjhatneo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qrhfcbpo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbupegdo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ezrzrawr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sbpynfah.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dehkziec.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ddqonrnq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ehxcztna.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wlonfmiy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dgrihvro.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fxxlvvmf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3imfszzip.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3josoqzhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kullcwfd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jvqcizaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozivvwno.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cznbwvny.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sbjtukjn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbwdkdgx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjdoaopk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3artgkdxu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjhqcdyy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rbstvagx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qzyfihpu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgqjqtot.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zebeiupl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bbwvhfbt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3puukpbcb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ofmgfcrb.html


<!-- 参考信息 -->