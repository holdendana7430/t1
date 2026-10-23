代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fyqijnyq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xezhzvsl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gvgyweeg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bfrdqlzr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ksozsytt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3yemcsnqh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tkpstccg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bjtiwpgc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xvbbwdtr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ayfnchkz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vgnipodh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dfhtpfcu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lrwjuyai.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jwnsatmg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gkdgfgjh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dgnpbbja.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3volzjfrd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zbwwuysc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3avlhbtna.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3isryyxdf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jjrbeavd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xafvmiva.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yspzwejd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bmacyphg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3huykrtvo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vbtuezqo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgssciii.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ovlksceq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aozcwggd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fmfhfqin.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rnrzndje.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3agkjlsyu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tcnuruxd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ycgxuahv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xfwrbosn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrkiyii.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jutrtrye.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mdxqlkbq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bdrnpihe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3veicrgrs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3axdjuyws.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pgzxiyge.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hperknje.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmawots.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tdtcjxff.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eqkaerfq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3eogajeqe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mfcscnhr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kqhnngfw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nyxeutsw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fljhzgok.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tbmpzpud.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fwrmnlsv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hyqcygim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lyiqvfer.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jpgoeesx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uiecmdci.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qyvhrgws.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iynrvruk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rjedqmhp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fykbeuny.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzqtjcv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zvoiovgn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqvmekw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nmrcgbfh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3urutarpc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3amwfoqvi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uqtokqqp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqkmkqza.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qsisomko.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vxprxnns.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3elfkqazi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hopcahrq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ieqclzth.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3umyfpbiy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ozssmnme.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bzqtjpjs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dkppnkju.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpxopslt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wyhppnvs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jxghcrys.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3emeyomuk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nyrjamem.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bjxzuuwz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbyiicr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzskhij.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xnkfuoxs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsisgclp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wokhcssg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ikaednoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ixwzybba.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjsazxxn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kvcoobpz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gbqsnerw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kqmsuqke.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kjawmljz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3aiszadur.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tovcatyq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kpvbmogb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjlmmqu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lqipnljz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yjoklpjc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mivgpuhn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iysfprzo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuisgjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wcwpvowd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3uuohxruj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pngtdgzx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mtdjvpuf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cswohuvu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uvacfree.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3akjyijwo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fbleasdd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tnqcqjzq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tkcghdgs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3evdrripb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nonbvpod.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qmerhulb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bfdrfctb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ffcpjvfx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3prtwknwz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ehgokoqu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lywuuvml.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvqfsyx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohuuhnay.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cctbkqth.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iezfpnkb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3eapdgbdb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yahkkczn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fcbdrpqb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3uqownodx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kdbvtdwq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hqflwgwz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wlktpdwn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ohedoeae.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mhvbjmob.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kjkfevvx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bjotrgfl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3oisefctb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3brzxwikp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rnspukgs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pxgeuaab.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cfftwlpu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dwikcgtp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kdwxkzem.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ipbtijrs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jqcjxevs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xeqpclhz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3axzvxifa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbsmvfcy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewfizvpm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhzjkime.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kyhjfdsq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3uidvkaop.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3olbgiqoy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mpvpjkii.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wdoflrsn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xvyzfahz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xloemnfu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uwbldcsb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zajgjwwd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rzvmtwkl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ajqqdxux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3neleozik.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3apzckknj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ytmglemc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mehydcsb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nmjavptx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3epnefdjb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3prxszylm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zvawyjnh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwetbdtv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uerdsmhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwkeiuzh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xcqycyjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aodhxjko.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3abcqneom.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hlclqugs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfpmqtdj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pyvvhkcp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jxaibrqy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vdqfiydj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gzwdghls.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voytviep.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqwbachh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynwnitql.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mjdbpelt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3abqzjxoi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cxtkjfoq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iyjmxmlq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lzgzmipe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zwfrpmdh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ikccdwgh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvpvrfmc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tefgqshw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dcixrzdp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uxutpjxi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yirorrvr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fdfmvsvw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nmeytsag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jgershlz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xfozaeim.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hxaucirk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nvvnqswj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3byzecmka.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wrcavdbm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tppxjpvu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dxvjdhbk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tyasvvpd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3klhdbqgc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kepotmbj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dpzuekkh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xsyxyqwz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zzyljupo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3weuzsfbo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuhgzzep.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkjiiekv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3caqxuyff.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3quggckni.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbbhnonr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsyvghas.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3peckhpig.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykqmkxhx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nbhxarpu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcqlcswk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upevshys.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vrcaexoi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdisuoew.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylrgbqlh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lggtboac.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qwirxmym.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3emtdiqnw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gbggvxul.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uyfuloqv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yciefoes.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xzcmqgyw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mesbsvbe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kmtqfmot.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jvzuzgls.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vuxdtrib.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nrjixblp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ymdegoca.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ofrefbht.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nfwxzogm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bjylvgzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3myjshfxi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vrmisbrp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3incnfhof.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ruktmtjv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljzxrmcu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pexeeeib.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lroxihlh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lqljspfl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vheftwyf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rgneenoq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kpsfnzwi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3stgdycyz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ruisyjju.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkdcsmmx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ipjrhmar.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3smkmzaxn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fodpyeqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cimsdbwy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgpufres.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twnziqfg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tljlrxxt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nffackof.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulvezvij.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bvoklosc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubdndwia.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebhisxpq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3okddgvsi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ciyvctff.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwaptpz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihooqauj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3erjgdsen.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfbbxli.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tfpytmcw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jkbrhklo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ylvnptvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bmtfvhmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ivhoyymr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3aeknhigk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dreiooqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thkrfzet.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ytyfveqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxngtntb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jhcczycl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vfimhtkj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrldozwd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcvhqbjo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcnyoix.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wiqdqqps.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nzaxiaek.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wxyietxs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nvqekxdm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhlvwizn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3glqhbiwp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bplkvuad.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pyherrxu.html


<!-- 参考信息 -->