代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kjujwcpy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2slchzvlx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gkilijwj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ibcyuyqg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2omdjuzpq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oujqcmhc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yedgwwfy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znxztbhn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ksbhdcbg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2khwvbujj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uymbocml.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fzgalloh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kfzerbfb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfpdvfe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kqlrqoxf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bkgphmto.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tppsdxaw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2eofzbecl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yxghakgw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vvblpftt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2njfcqjdb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hopinbvq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2skupneao.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ldiycrsi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mmjjwyau.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fvalflqm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2exuramgu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fnsgqfgh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vbhsavsb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhctlwxa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dvubrqhg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vqucsmwu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ziaieary.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wlchklci.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jifnetpi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2widiohuj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uvzpdmyw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qhmnlsjt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dwbdztbb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cpdlcjxm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iuulenlp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xqdcxfus.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kzmdpnps.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zxgtxocq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cqqjdbmw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2afawisbr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gcyzifre.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtprkica.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tvqwxqxh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kupejydv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mfhjxvuk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2scibulgm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2appugcee.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pjosktfy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uoauocle.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rdetszuc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xqktdpui.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2claxeuku.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pqljehqa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wvqrwkau.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2trroflht.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2monafdxi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rczxvfgb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ohamynre.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tgdihnut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rtufdhyp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pymaweov.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sicrjnpn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2psnqdqrn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mamgjdqz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hsqdxddt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxvzpvdk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wbhtaefy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ayorzlsz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2irneawyd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2baepjltz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2iagidgje.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mlbjpxyi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ugxjzwes.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2idoggbiu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tyapuihc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mwjakhwx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vxvvpsgv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2orspezsn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kqbarxnb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ljfcxrxs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cjaqtxaf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2weqydkdf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mswqwkte.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2linsmbed.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wsqkgepz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2legpcbaf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tdlqpgui.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bzpgwhkh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yhdsjcmh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2phivmapz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2luqlrxvi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yrpsvufr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ximnqdjg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jinnuytn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2itkffhyn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2asglzope.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2aaidjcic.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2peogbhrh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kfncchtm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ivqecsav.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gztghihw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wqvdwyvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgibucr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2olmjlumk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2efeavzfv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2npfsgayc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gpbeclpi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dvhbrgnz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aafdjoak.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tmkoavjs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plrkexib.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2odqggavx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ohestjaw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdbjxhs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2aisukjsx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpjydel.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ofgqfdqf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2btwuacyr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xjvruesw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bnidaqjl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qxrjlciy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvyxlca.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tktziqsq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2crkkbgcc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2kllnitsn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vkydigfb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2icadnmca.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ggdbukae.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mqpaztxx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fhjjjbtb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jxsqpevs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2awqlnkcf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rglbfcxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2emxiggtu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gnhazopu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2spbptuwh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2eyrrtwvx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2drjxnohs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rtlybjiv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wjjlfsmn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bkzksdqr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgtculih.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sqzrrtaw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2izruwhgn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wlnsyhsi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hxcbzocy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dscpbuld.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2puxapvhb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtavfgeb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bquuddlk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xjbcoasc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nbcbchcf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cjvturcv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bfjuiotl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hlvzvqwt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eorxqwkg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhxcxrzf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erjlogin.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnqwaokw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ytmnybjc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tbgazmnv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yqmtgecc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yvjabcfh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aqvhrnok.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eggqpshu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2umpzpfsf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jteecmuw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2swhisjsr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qqguftbp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dxlxuruf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sgfzgwnb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2exktsogv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2toxseqoa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gjcdhzbx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xsrxyqux.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2awwfghqc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ydrfmcbg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qyalnfrv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fzlsgihs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugaabblu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ggkjuexv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcwesrkn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwmxcfkh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yfrdxxjp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfteujki.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kwisqmnf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wflzztlt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nllmfygq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mlnqdcjc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnmgbqnm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkqmdtnx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nshefvqo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vjzfpztq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2olebhqep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqtjjjkp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hpotrsjq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2akrtdvvf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2azjempos.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ayzubjwd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pyeuspft.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gurqumga.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xegdjgfw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rcktqlvv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xcrhhahi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lucazybf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2trjxbeys.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pevmgqcc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jirzziuk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qlwlepyl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qxnxqojy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2orkiikqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2aeojlpir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2defldxxg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tnfrxrlw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pafgexyz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jaulgfnv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qnxecruj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uiktgsjh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2idafhcef.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2enktgmpw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckqiybxu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xghydpav.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2habkxdmo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zdvsqhek.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fhnoslmg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxmzvodg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgtmjwgx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpzuzogf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wloyzziy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmgfgbau.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzqbnniy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dafarykt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gamccnqq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jchlaxvx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oozeumvh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mhnpricc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ksuarctz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iwdfmjru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ojfqiynl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hpyjbutu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fkxtomrn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dnrkwmtr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2drrvfgag.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rcrmhanp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xtkoxxpt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nvvwztga.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmbkptr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wpnclmmv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dutxfpsh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ltiaagwk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ibqxjxpa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lcfpxjlw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ofsjlmij.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2exsubvne.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2riaynbvw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snamuutq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gnykwhas.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bjrlesoc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nzumvkin.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bxxltjuf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ofzszjfa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pggbcbhi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2cmieseub.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hrrkgteo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unomdgxp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kvvurnld.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgizehkc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykvaekjn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zzoxmgcz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yggmfidu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ensxrpia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifbzxgtk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sdkiydao.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chcwiyvl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xlbtyhvt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwioytnc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqapvzsv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bknwnkow.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qxtboxvp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzvcsner.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oijuqcch.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2eelwmifu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wflprona.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vuxtxtcs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pqukljsk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lpivihst.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sfnqrbqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ruhcndlx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2boebuapa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2njtjbssm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmhrmcku.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dljidmft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2przglhec.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dbqmqpmo.html


<!-- 参考信息 -->