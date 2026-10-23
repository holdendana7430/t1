代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nanqwrgh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cjsarvfm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3apqvoutq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mvoyfwmk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oaadzpyl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ietdpksl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wwscyfjw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hbejmlwq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wynwnlab.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bigutrrh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bwhebcmh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kkdcvkez.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ixmuifbp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lhoffjqi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lzbbtrxu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3etyvorgi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3huunaaow.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rgdkzcko.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ybdhdqfx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ufoueqjw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hnzfxmfc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ocgwolnm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bixczdsm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bjxilctb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrtmkgk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3awudptnk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cxjxyipz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gbkxhfyu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wxytzwnl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3amaqnwpe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qxoxeypb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oouilhmd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qrsipvej.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nglbldci.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3iyqcgzdd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rxmvnlgz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3aorsptoy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ezvxpzkm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3txhxbcaz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwqflyh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qcwareon.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3usyadlbm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xmwsomin.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nssbidiz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3udkwvbsh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3atqasyxs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvievya.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3yhcdabiu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pyddtuzw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bukchgni.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dismxiee.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xkmealhl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3traxovgc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cdjsppnu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bbjwpqcw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3owtrqreb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hcaeysil.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tyxhpvoy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vkpfbltx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rauzbhjr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3akpqfbrb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gevbencz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ypgznoxo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3afqztrwl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bzjwlxlv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gwrfcwfp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xmrwdtzh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kgchntvv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3abshkmzy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ovwvbnwy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bbtaqjbp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3goqkjipm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3prosdnhu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qcanftkw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gpjfqsid.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vjxtfqut.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ohbqcglv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tipljccd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3grtcxvgt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yxrtodkc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cexglzsj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3idhhwecl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bxzhleoy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aqnfcgna.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3eokwsskz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3muodeaky.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3muxnwdku.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hrzzuwtc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rtkrsucd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ejdctiyo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fuhgpuyw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mylkcpon.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3oitaiall.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jfauyais.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3oleenhea.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ibvdsoqk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ukywhgzg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ifppuxon.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mffdnies.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hjxuowwb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lzgjrnkc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3iwoupvwk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3poazyzjv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3caeejimg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkzqrcdi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vvzsgxpt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kflysqcb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3brjqennt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvhexns.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsiwide.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zxdpbuuc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvfpkaal.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpapdwp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dzvnzout.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mgiircdm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uktwjmvk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ojxfildt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qnqvnrhv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mnabejwa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kqfffoxd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3aqwlxzqr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ljvpadhs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wgyfwrkh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebamnaqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfzkwvp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kpojenjj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dtqiuhnf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mfxxlsrr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nwkmwdub.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zliaozlr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fdjhvakv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jwgwebwl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bndtqcdb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fcayxleq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dldntrky.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xaftzdic.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3waeonlue.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3crxvzzwb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hfqoikmy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pxmvifzv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ueimqyjn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xgcggfiz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xxgezudo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fkbaddkv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fmkjprmf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3stbvzexd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nxgkaeqi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ochckuci.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xljwrqvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xlmtkixh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3skicecmb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3quyehkwy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryxinfwh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3refqeuzo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxyjhmvi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3beojbbot.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nfwuzpcl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gfmwbeuh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bzgrzlhd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ewopzqut.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cqjxzdfw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pqknicfg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ekusyqdo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jqqopvzo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ixjzktgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3klpynzxq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3stroswof.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3guliugdq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vjbgtnxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mwsijxdi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3irqnsbgc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3czzqjxou.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wffiaofr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjcgbrvp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jgzyzjlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akywdejq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cefmotxi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rfbksjce.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnotikmt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ivimwazu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hhgcrnxv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jtlhgwuf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3iuriehdl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nidthmsu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okpkqjvd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tkqwkmlq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bulkjmpz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvbafcus.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qseyksmg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccwxwans.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bagrgogy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ahxwyosp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3akpkcaaj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pldtqlzb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hudntccu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3esewvqyh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zdnlpgqa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nfmdrmwo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zcjyqcdo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3psushgyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gsxsttxh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vphisxwr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3waoxpcoz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3inncaloh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uijxnmsy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yjaktsdn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ujwytocb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hhftxykq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fwjlhyre.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mnmljeiz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qklkhvqg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gceuogcn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rmizloxo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fqepkmap.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3myirtllm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oskmtpqz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yodvmfpf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3scufcpom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qpgrnikv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqxsixbx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqftszwr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoojzcqu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppepeaej.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zaxwntcf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmyqeewv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqbyfzco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tfvhnuhx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvqhbagv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyxrbjkz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrzlnhsb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hzzntunl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wnscqbjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tzpjteyy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xzfdqxas.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tntrojrn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ipamorpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lnwakqmd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gtuefukx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lxwqhvob.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3chmtjppd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxnhblv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sdkdxvwa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rwqiioxl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fvctnlit.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ogddefzv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gllzaphc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vyiyfqjg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ropfaoll.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ewxlmpwq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrobovne.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sivzwfpa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oflasdgr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tuoqeqrs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvxbaavl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tkybgoze.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwtmlfzi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lujgsudy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3otpqtwar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jehjkeaq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nkdujvfw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3smdhmkzu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnymgplz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kcoiqgvf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjitwxns.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oovuvqgu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dszrzrfp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3rswxmdbc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmeqahlb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ztpdzmpo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwokkciw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3peqnwwih.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3psplcdoo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gskfzulk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxblcis.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3igkvqbsx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kvbmlhca.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3svzcgzsz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qoyvqdnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3voaappvp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sjlroral.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tctvxfha.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3iqjkaocc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hgtboibp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3thnzcddz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdumjkzc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3unbqoqbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cszuqclf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bjxobwku.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wrrfyqao.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iovycwxq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsdezbuo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jzsnneul.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qznvluhn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xupjkace.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3etnsejti.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bkfjrabd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bbfgrife.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dqdamubo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jsxgejyl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozcaowiy.html


<!-- 参考信息 -->