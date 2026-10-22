代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yxnuzfih.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2slufsuyf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lejzanjn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgsghn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qtivxysn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tchllziv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kaorfmyw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wygjyiqk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wdvyqwst.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aripyniw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2shwmonkg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lsmohmal.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vlmntydq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrmwiw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mbzoidni.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2coobuvqs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hstxxvdq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jzejlvvy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2klvxurwx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gdsmnvpc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ziuhpeoj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgfriwub.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqpvsvjt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svvueumr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lhtlnbyf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ynxqqkju.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dueysacl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fjybniyd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bxaucfhg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dcujtedw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2grxeegvj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vdzkgcht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgbqbqb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wkegcxsa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rbrbjbjb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hwwfhlxb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pjxnsydr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hqhyrzdq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iddcoasj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dhidhbwu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jjvgxasa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hishorys.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dzklkmru.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxbgnij.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kxhztwhi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ppuyepjs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gvkvecna.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tcimcpvz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jghnrkrk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2agtogfnw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2btkkdtta.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pwxhzkxa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cowjvxmt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wjvuzxlp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nvwmyhno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ejudjmcd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zpbbrzhd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kntunyzw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zsvdyjne.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lhwttlvx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ribdrxor.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2paxytquh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dsmqfaad.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qpnbdgec.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zpaclgnb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jvezkhmg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pdagluid.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvbrwifl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ztbmsupv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wxcnkffp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kfdqmvlp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bqcunpiv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dgdlvohb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lmtivsxp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vnibxjhv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2usbzxhip.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mayoghlp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2norpqapw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hevcikjt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ethtbgve.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2akksaqtt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jnaxnfdq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ultkysqc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zpdyrafg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wwtfamfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uwgvvcjk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pboyewna.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lcqmzket.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoecugxb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xiwxmcds.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kafdnaam.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hwkgnlec.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fwvrbmab.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wufdwtlr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2aiucvxgd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2aemlodjc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2frswosbi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwyuyet.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zezpjjli.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tylvkcrm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hqsegfoc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qbqhnthi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ntftjatn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dzumwkpp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ncbhhege.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2umhpqgqo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tfuvhjwt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hktqltxp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwjlrjch.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cikppqpy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qixpnfyg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rvcgxifh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2aifajpda.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qwqialqn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2esfrhvqd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eotqlywu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rqnmcdku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tuyiukoa.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qovnivyr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dgyobatb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wrjlfbdk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdrfzuvf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqfudtyt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bweaycyd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyczogyr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dmpqxgqa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qvglloht.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ixgkegxq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kkfteuzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ssaemjqj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mdotrlmc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pcihqpvd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gvldwwxm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rnxmflpr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xdgxdpdw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hfbyxafa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fllvkqmh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hajxjdiq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xybtiuuq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vjmwxnfo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2urgycimv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wkncpbib.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ggzcfwbt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dkrurpsh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zvupzvod.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mvfswqmf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ocwlwvtq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cimcmtbw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jalecamx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffxoclmy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ivhrycui.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljteszid.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ooccqmci.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nahafinz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ulmpetyl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bqvtcfqn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zqxhcjwl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2epawnidg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qvoupqas.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ddrgupeh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wujscyfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zrrvzuwz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mjbncpjm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mooftvpd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sifdaaqk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2avpgkjwm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vdqgvufu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2recgkznq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jeawzygr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ktqzyopr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2aichqbfp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2erwvdgxl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ltqyithi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egxuajhj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bigrslxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwwnyonl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcknsrqb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2covcwbpz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hfydwsjx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xlcxaako.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rgdfqqcj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uaevscfn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2awkzoqor.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdzslybu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wcralrfa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2drwwqbnz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qkxjfmqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pwecgsfe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xecmbvog.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xewilmgo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vxpwlikx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zkugorjq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xcfdwxux.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qcyiwxvq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hhoierck.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kpqhdrhb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qshxihds.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lpohtzgh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xdmfbahe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ezkepltn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2diubajwn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wlupbwpd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2syavsktu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzngxjik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sxddawcd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zufhithm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pstqzksg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2erqphbth.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ujyiojqm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wxhglpop.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2peheyhtm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2csjeclsh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ifsyduzt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jogggbqm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qqvudbto.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jaijenjo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqnxkdlk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vkzkajur.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pbkbvkwm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjfuuxlo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvypolvx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekgehmpv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2peujxcgd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jmnepbht.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgyxltjw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfzkqcja.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hdawcqwp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xadtwtmd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbncdnhv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxihjaah.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pnoiditv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2atppvkrw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nvfcxmvy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qqwdlyqv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2izgcahxm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jormsmfz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nwbmkoqp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kfmrawtw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zgrqmagw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qwhskdrc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hbftoson.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2astlbcxf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gbguswdd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ygitfaia.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpdbayy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jxciwysz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tegqbryq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vjrkgqnw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2crdaaugk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrlfyirt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rugfttui.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bgvwzwor.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mesxrbtz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gbmrrgmn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ibqnaoiv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2krgaeqgz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rjosqkxm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rypbtolv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqqymlji.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tyjiqxwm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epiyzbvu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvstoaak.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pewsgdki.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vokrmhva.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuiiwiuo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szabsfus.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ggrmqflo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxizufnx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dnehakqj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebtnpgot.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpybqiix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cnxfbocj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aubihcah.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eeaowfxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dfolkqlc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dydfvipg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jcbeqkag.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rldfrvfg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zhnwfbzy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kckjfjpk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2iikfonri.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2flbtgfhd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wxifyfkk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lreghbuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckgczhsf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2loqkztix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkpbectx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xsupsiuv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dgeqrawz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pifoskeo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dxlvfyxu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kpkrlafs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2liyvjsmw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wsymgpwb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqkxssna.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lfxavaom.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2yelbafag.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rvrkaatd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psirmszu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yvbuxvzr.html


<!-- 参考信息 -->