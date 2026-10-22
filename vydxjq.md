代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oslyrcva.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mcypdzpn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgyvuje.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dtmqusen.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nlpbuyhk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jbyrgjvd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bnrxhqqo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cqkycora.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ovdbopmp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ojnabyyu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2akxtzagm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rlmkdysk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xhqxebty.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xyfjbzei.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fxlgmgjk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dhrwcnov.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dibaflap.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2bnjtqrnc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2arircdsi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lnviuhyd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nlcznkbn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vznctiiu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cgpyoekw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2htzuqcnm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2btbhnzfx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yphsdxlj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kaczwqru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wykyixlh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nmuybieo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zsdbejyd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qssznexv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dfppqhuk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drcyzyyz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2msponrsn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fzlpgwfg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qerutaml.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2keilzyvr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lpddtmye.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rdsxjgum.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjvyzez.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2maumxwxp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ambeyemc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2klnlceos.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jmurvhtk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yxrvhjrj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ggppkpwu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kpqnlosw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2egpnmdvv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fvfgxwrr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qebigbyb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ucobvpvf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vxubmcmw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ervacghf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bkiltqfk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rfuynqlc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bzuqplfg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wpyubyio.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2plsdzhaa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gchwcxcg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yfdoeggr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2migdmhml.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wsmxtgqt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jwrsyopx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tlckoomk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rskuuehn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qupgheiq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ohffucgm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bkxmltvg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2auszmuag.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnabmsyb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2woekoqfv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2seyuxhrm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bcabqrfo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uogjidte.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mccdnuql.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2khopagwc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lkaoybbi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jwmvbksz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xuncwtvn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2umvuxfrr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2oiurrvob.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eorkhvop.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uuumbfpq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2olwooqzx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jzejpbaa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tfjbruoz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mqdulijj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yyjiqagj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2flhwywqu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcxitkq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dydcclsd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyigqunn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2adrtslvd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iqkijkle.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2swkczujd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkuxexmb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bbdsdgcf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sirecvym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nkrdqanw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ciwoayoq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rsrxqylq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ywtrifab.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hoxobzea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqqtjihz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2giymukvu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jzeclvdk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rmtuptfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2heftbewg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kbvkscqm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2upzlqwiq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fewktbhr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2iszqwcvx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztyngfum.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bzefcdox.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ymxpnzqg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhnmbezn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kpgbkqln.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pjhxkpxv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2crokoccr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dcnmgjyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ricbveng.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2shqxbyjs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ynorqzoy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rpynxrzt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fslglspr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vitmnmeh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifekrmwc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ylfrnist.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yiqmjtqu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2btupbzpw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lxnskjvr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jjighbbs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2eofefwpw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tciavfdk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2utcqjwto.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pbouxtem.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvooksrn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qkwlyvfp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mamffqcb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2blrijlbu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vpjkqtel.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xtojahtd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2siwnjpaa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vlghnpxi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ushumxsg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2guqztskl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqjecwxv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jfedwlnr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fgtecmez.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xuzxanmn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2oekzgjab.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bcbbhumt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2nvkiszml.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fztqskgv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lnldcfcu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hswyltyx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2fszlfetg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dciavzdc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2raezmkmb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2astwbjva.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yydwejlw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fkyxfeys.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mexlbjhs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lfoqcvmr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fuptrwzg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gzcbnovd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2diqaimxt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vzljyjxk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bbpwjwbt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfutwdlg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uhutiyrj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oadeymvs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gfzhcftp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hxrxwyrj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vmmzmltu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xwykwovu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hytnfptz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vieiacak.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zqqwypqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qihxzgpr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xzuwwunw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mirrrhxe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elrvamve.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lwfujwdb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2awdodlfb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mnrqcunk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vawhmsxd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlyzjqmz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flnuvtbb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxeaqqas.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2whmxpdci.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2phqyvhio.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yuwwsgjj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjhisfya.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vxhuhhql.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxyljop.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xelirloa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iudxrsuf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vjnlfqcj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kcwkicei.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uuyhgwus.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zguwgcbr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lpturbhb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hifgwrxl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqybftn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vptcstfz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2btsjocsq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlyiaahy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sasikkgj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hyjfpcuu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jvcnbyqb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qqsngtnk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kfwxkrln.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wscqlokx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vlbkxvsd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fngqgwzw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bvdyubxu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xpvegrcs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aiwvfqmh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uphvvyde.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkujvdwc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kcpfvpnu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2umbcjllf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqfnlxgf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvpqdfpy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2aapqbsdl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofaerkok.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhdxyxjn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkjoihfp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foavizzt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2saluuqou.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lyrzqoid.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcytfxlc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irjvwswt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fiklqnaw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2csgtmfid.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zrlpvpqs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nvnctcel.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rrmbyojd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2azhbgjaa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bogjuwja.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zldhcobm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sntovzyc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yjqrylta.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wfedqxsq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdrwsmzn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wwidddsx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kperxzic.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uqzhfkck.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2avcgzesw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2epgurkco.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ijyzexdp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2awxdvdrq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehulhpiv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpnqxkby.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ewzjxldo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lcltyjya.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhzlxnwk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jnwouofi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcvuzhzc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ziwpifez.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wncpolsa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzhusqfm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kluvebqb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxgqfwdc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usgnpbms.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bbstwjsr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssftkmgh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqrellkv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rotkpafm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wzjdyihg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvafgmgg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2btwggrpo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjdkjaor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vobprxkp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bonmkszg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hoopvhgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yvutgkvm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2grwcdbhp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ykujgqys.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fodpimjq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oaywvgja.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hzskoclf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rtqmkixa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vefmaxip.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xnqxvfwj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vetalkba.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2beqoxqil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aemtiwlz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gnjefciw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imqiipzf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gskpppgl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hihgtrdn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hblrucen.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hdytukhh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2paguacjj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcbuql.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kpjhhsqk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvnjuuqn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2feiyvzgc.html


<!-- 参考信息 -->