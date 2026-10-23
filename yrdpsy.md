代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ovqwzqug.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cpyvkpvt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdkegy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hppssfuv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wjxvtojf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pxfwrvzf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ksfudjkp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3spjcmard.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xoldbdrs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ktuvqggg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wfgbdset.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3knoeuidg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3sfrdxneq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mquvexyq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vcqvkkzp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3cqubiewh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rklfmntc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kxixdnph.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lnzspcvl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pqumemeg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwltozxe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nigwnnuh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zgtavolb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lnhnpvyw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yyksntgy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvcpusno.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kqogsdra.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ntrawbym.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vnaqydso.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nvvfwmgj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsyqgev.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqsnnyhp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pomihxas.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ulsvdurm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jumktokn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ovcypmsx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3orlwcmly.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ywketsxl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pfqajtsq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlyxzhgw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qjivjjtr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ahqrtmxt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bxiqmvpm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3okpcrzob.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zfyjxopb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cubawain.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3znnuvdyu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rirsksfn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jgenpetn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cykdebvo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iagwucvd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dxpjyouv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3frelgzfb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rwsuxhsw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bewvyozy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gccqdxjc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3achwxlla.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fwpizimy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3akrfhfnu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yeovjbzq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qkhlsgpr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ahtmaomk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wrhwbzim.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wtqwszhh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3izckyiqn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pldettll.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3avtndncy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gwantqpp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jypfwvhh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xcjrhira.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3falkkqpc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eurdxzuh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bhfymztr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fmkehunq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ehyzctjj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ahsyvvon.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zhwtntyu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cgycphnf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wguaweqp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lsezqkyj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jicdoyvr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kzqmohyh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mxnlowgy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gwzmisgn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3oahazbwt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xfvwfylg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nmxrmwnt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rrcvlmrd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dhflqvmi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ttmwlqmg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsmavyzq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cabughvn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3abkutjub.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vsezaeda.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mtimexae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdejoyaa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hyswuugd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ywhombxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjpsfkra.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3injmabql.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3opjwkjvc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3onqvoshl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ugtodjog.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xricqfed.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xtoltyfi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xfknzijv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zcyfkmds.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oquadwaq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ahdfluwj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kbocxfsk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nrealgpc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzujdwjb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pzkdklpw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hmnakshk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oyulwoxg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3stilniyi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3anofcvkc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sjuocenq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nqsotqag.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pbseyubr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3iwuwhdwo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fxogvbps.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qivmqxqu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ilczzyts.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3stipndpz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgjoxvvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xevduqms.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgwcpvmp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tiegzhpa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jlmhajmw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dynaxhuv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dtcmochh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pknnhijp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vnmirdlc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qkrhvxmy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nsrwahrq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jdrnyghz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oigaxofz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gvvddjaj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qfdzavjl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kivyvqcm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3exvqoxty.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zcteccfh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3otnwoydn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qozggcqw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ancedqki.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ijwlylmm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xpyamrbo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3egqqeswq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3afgaduog.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ropdascz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bljyqutc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gttwtqke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edqbsict.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuhwxcmy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mbsvrpiu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3oukodeuo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sjltqzbn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zqeucwml.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3syuhxxkt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jqlrilbj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jahjogqp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3spkqflbp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mvvwerwq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3toopqhdd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zvltnrrs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gjtjxsdh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lnlunzpy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgyfegew.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozshsitu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vuorelje.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lxmecsze.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fcmkiuua.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ymxwnwrx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qcibzlof.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sydkjevk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pffetzxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywrinzmh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nhrkhimy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efsmtxix.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3shycpntk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hevepwwj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3alunjnyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jlwetagm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fobsgxvf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yereiveo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tfryhbcs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjuwffdw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejqinwae.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctmqtypc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3badmxvud.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tizrevnq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpelwqbr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqfatlfa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fywljogj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qfoccavk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3blafzile.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tsllstum.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pkqjivhj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3euvienyz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qerjoslj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eglkfinn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rpsukrny.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mhzvegnu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3phgoslbo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yknxchjv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hmygypza.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3uykfeguc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3odgjjxyu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fnglcfli.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bmmzlfkn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sccmuqpd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xvwfvhbk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zuhqjohy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtmfcdd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jcbxqdek.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gjdiwfat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3npcdxmlt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jvnojhhe.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipgqnevp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvqwhzvu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ssdqhbet.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjncxnf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mplzosee.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpmbwxc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3btwslqqi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcnbvopu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ykfyicfo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybutzpch.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njelhjxd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gobrhmue.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yiwsftxj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ryygnqqo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oawpiqaa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xvhjdlvu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nfbcrvgs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3juyvqqbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lklwubux.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zmeenidn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dlltnbwx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrmloji.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dkljpysy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3obvvxzpq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qtmaixdv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nkqeiljm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3anihendy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gkohphub.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvgeeum.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nglnrqcc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nyucqmsg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3faqtjzze.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bdgcbxcg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hvdfcufk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvwqwvrq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ogxymeot.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ngwzokgd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pcozilds.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zumlzpng.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gcxjptfc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjjyeavq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rvfmuhau.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qzuytsdt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmnpenab.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kdysruiy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3foxolchy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmmleypi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3arjynidz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijuitgpc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvjpgqyy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nisqtjsc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqwrnvqc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsranvjp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hyefcioe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxgkdman.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpkewrsq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrjjvja.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nrqqdbhu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqpodsqh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bqkflnqe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3axzktxjq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwqwjzv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hynkeqqv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wpcivoie.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lgogzocj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fxlnymxi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bertbaqd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3apbjqfcl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jrfycfts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqgdqgwm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yqiqicec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsiddysk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wuzfhbrn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3edtmkeil.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ujxqhjps.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bajvksnw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pguvssne.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtogyqfi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lhephhmb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zzkxwtkh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3opdgpear.html


<!-- 参考信息 -->