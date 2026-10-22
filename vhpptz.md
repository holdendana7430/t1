代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pllegsnj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rksgbqdd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yeqgjqct.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2njclbpoe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2idmwqwrj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yqjnrvty.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dgyculyy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jjpskdnl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qylyjgae.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ehudsadk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vvmtvojz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zukglqjo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rujxmswh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2drgmolkp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fwiuaslr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xajfpnud.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rqwnwmjk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ypumsgjq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2uwwjektx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2osijsfxl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qprampsi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oplshtbr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rfekffry.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmxvnvgi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2boiorpkq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kpzowgpf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcrojgfh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xfksmjcm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2flxjbpun.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2abpppskc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lnzuyrmh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tgwtymzb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hiizwzpq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2icoxpfxd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wnkuvpvk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzcvnqgw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lxogjsfv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pzjuejdq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ivoshfel.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2htojykxh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ehmshivf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sqoojgnf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aemeznbs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xacepdts.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jtvmvryq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wltnlviw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2krsjyecn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rftiyurl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2krobygtb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cuwahyxr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wtpbemhk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uzqzhnvn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qnmkxhga.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zubnadnm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qfhgkyka.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2brklxhlg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qpmagndi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aohxkayz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kvxoymfh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zbpxsoqy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yjmcryki.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cnfxyglp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qsqqdmqz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cppjrszj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2eapglgfo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uyvfvcow.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ycrlzyhh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yljuqwmf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wvvdhqtt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gnpmgpoc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ydndrbab.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bdwykfka.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dsfcpsim.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xgutqjpq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2prwokjnv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ytfqyhaf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jqgekneh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxligbig.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2motqijwf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qqpjqlwh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2herabgrr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2eyfhqiiv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fgyggksd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vfcnyblt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vczvttjk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rkfbzzwg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xcikbxdi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2atzthrik.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2enrfnkbr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xjooziux.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sayflded.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzyzrrp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2owwogqii.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2itbfcajc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhkavduk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pncfbwvv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lqeniooz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mscdtrfl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kxwadrig.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jomcsgde.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfeokd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2perptper.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tjhswweh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rcjnakcc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgrgtvht.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2esogbxvn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uvkqdkzr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zscpzgxi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bstplvls.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfehfjfl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ntfbaksg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vezbenhl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eomjlbkp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xlmkjivz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tynsegdm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsoiwou.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2flmxprnp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ovocfqqt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ebjzmebm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rkemsztc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2onuhszrw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zmnzhnbc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjyilwf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpjhqaoc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cwtysevj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rdyvwion.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qhzzqqgi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nttiwdob.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hjhpkife.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bpwttcpf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdjwgzq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gmmqwacj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xmuhhblu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2egmsbqlb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uafbrovm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dukwaqlv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cyonrbos.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ezedcrtl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nsursclw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcnzimkn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pwjpoicw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2spxrjvca.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yunbcqnr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhhmwrt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ieiazokn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yltyeeoe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sdpxufae.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zmnkyvea.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kdooxtgq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kzzoacmc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwdgyvgm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lffvlnyl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyphkdmh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ouiascsg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jpfmmfsu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2sgfotsvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zdhbgwnw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yemvvrxm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iwvhexoh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uxadwots.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nuoppuxo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2npvqwafr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wkdjacsx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rerkwllr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hnfhnfkt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nemecihr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wxystmnw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rwgrsvwo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bjryxfnh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fccxemmg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2udcgesil.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zamnhqci.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pfkvvwip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuewsgya.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mytshhim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmqsxvzt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ohchfdsp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2osrdhkdy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dmwgwyts.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ljsougpf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ycxicdxu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wgtlqhme.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vwtxzakf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvidouew.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhmlsjno.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wnvjrybc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fcaayljs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnnappn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2swujdfyp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhdojeqr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xukpqpdh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jaitcpjc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dtfxojmr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mvkoabuo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2klqvpnuf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wvapfkrx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jtocetos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ruinobva.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qpkhglbv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2anwjejqo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iadnydhz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wmnqavca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2snaoqiql.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpnzmqti.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qvkiydmg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qpcrseds.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lvzjnlvd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fzffxlxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xjohlbkg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bnvntsra.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mmsyzqwn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2czdypiij.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yhlaktwm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2sceapqcg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obzwtyux.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbosjlvs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lobhmoxz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wzvtwbwj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2glfauxox.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuxmrzxp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drspofyq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jicrndsc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkudoqiw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hrkfbdvi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qeqiuycg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuicllhv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gmgriqmd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtdyioju.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxprppwh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckgikbjl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tfxwalxh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tuzgbzvn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sbundktt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2stjvuehf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rhgdisto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pyrdwtwr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ktlgkjpd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2trcvxchm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2svgottwg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ujevivze.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrmguaq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tzmmscau.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2knbxchvo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2inmfbijn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yhwlhqhi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bjxmlgmr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2webaauht.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hxbblerj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2raayhkbf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbazgujb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zqwjbxot.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fiwaolcm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wsnhbcor.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvdelohe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zgvaqdqk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgzgmnyl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qrmcyrxi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2iojrknnw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvazygdv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dglehnal.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2goldsvbd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcmzlwsm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ijthhpzm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whngqymj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyjikqmr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvjldsuz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ldaxndwc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grlsgvhi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afiejoth.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2welpxcfn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpjdmqhq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lzicrlzi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2srbrvhcd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhwhxnam.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bvpjtltk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kilijugz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xyhxvivb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mffqnqkx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hjuyywnf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aodvfzxx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pxddlohw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2cfcitjoe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2imgnjkuy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wfqtmvef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jijaahdq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjpbjeuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lahziqsv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2yhehtvrm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rkdnaiag.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkidjapf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpammrdh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vdzbcsad.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sgnfkpgv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xntcxiwf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nkwqdqev.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nnuscvrs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2saxqgrtt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2givnyuyd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzroyamm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnfslnjn.html


<!-- 参考信息 -->