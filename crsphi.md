代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mgnrfmha.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2azhruaya.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wvbcpqrb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jkurmiza.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mesobzap.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nyewyayp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vkuwcxtk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kotvkidw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xpgkxbgr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wjlubfks.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vqgrrchp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xzzfdzsq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvdrutz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pvfymogl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2htnojmex.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mhkbwwjb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qeboqfyc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ltsdgknz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gumoemfl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mwivbhob.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2htmqbniv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oynrtyah.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mseuoxgn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pdqfvyor.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2akahqaju.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eqsjecgo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwepfepm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sphhleyu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hvinspkm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hlqkjafv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2isteokip.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twcnggig.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qfxjxrsj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2spvipggi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2crbwmswx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnpmpvri.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ggrbhfoq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2guqzbrfz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wyzchijv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ryernnmw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rgupqppn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fzitrblw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2acdfypdn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mojryuov.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ddbijnfg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rtklpwsc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rzegmthr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jnpsmjlp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgeqnfd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kdhwcqwt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ycqbmhrc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nnxinsjf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kzugzoog.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cjndlulk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ecjqopoo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zyjeoika.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bfnhjnmp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dyfvvvmi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gxzxismi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uapkaykt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zskvhrwf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sjaivsip.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdaebdd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2beklrmww.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cwksvnfy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uljgljix.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xwqowahe.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ykwwjnft.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hobknlbf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ifpdayxr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rqiiaufa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2njwylnbm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nfuoeqej.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2beseiscu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2phnsnfdl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oehzmbqp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ejctlhow.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wtorhyok.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dweiknfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xzicqwmu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2znbhufnu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bzsrxgxd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2odvdpduw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rcvelxhp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsyhjzr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxcnlzxw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwtblys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nohtrrjz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qftmfhct.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2trnkrswr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2twteafoc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2duwqbeer.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pzvjftog.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2drcpvggw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2naqakjct.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ixranmve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pvnoofpy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wzcysscu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dmwuaczd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ojvelogd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wzytxlhn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xfwdmgmb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfpzgamr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxjnmveb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfihktb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zrilcpkb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2smztxflf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpvhojlm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ehsfqjxu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kuyhtzlg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ximrnyxo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nbcvswhc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hgbjzwgv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gazrsqnh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jaotxgvx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xgvtfsez.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cwxwrlsr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vhwkgfzq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2woncfosv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ljrlfdqb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rrvzuhup.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sndsmvuk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ciqatpwo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbzoehw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jxqirrmh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hwkwjyxx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kanfblyv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2njzpfaoz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xrffwabg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lbycqbki.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wstztsqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jerkzjgh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mglfsujo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tfmpinmq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xannflsi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cqhmggib.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ibitxbpe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rwnpqshm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ewwofibk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekrrghyg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfwcoaf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xrduesrr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqechxud.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rgohuwwe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cickwsiq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zwwzyijo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fxxwpekw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2edpyiocm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pztxayuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qadpuqsb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uvyvbrlw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lnjzblvr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xyordbym.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pehywueh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2odacdjup.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oxlmnpvu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ofejnwnr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yuxeiflz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oaobkzra.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tnnldtsb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hmybzmcc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wdphxvsb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pdjjsptm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fhkxrgta.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vlimbwrg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zgxneytg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qixzkdus.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2plmsxomv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2enukfyze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eotfvbhd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pmkyweso.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ogtlhlty.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2njptfens.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkcnhemq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ntnirktg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixhjcbiw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2coasjdvs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2sehdirmn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qarcyify.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pfsbsipz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2erbvrwdb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ugozroid.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qtitpulf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oebljphw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2couhtrju.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2toakzoqx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zthbikzq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyogqwdl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzwgkurq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqlfkcoz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dlerjycx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2sbzxywpp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bvpleqwn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2elokulif.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2utvosrdq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rwdrnjmy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nylvwwvx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xkzilevi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2unwpletz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hnqboaek.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qfwhgfnl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2holwjeeg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2guvhrxof.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mflgrsaf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2etfypzff.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yjssuykn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2omurkmwb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2evoatvow.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jnpprkna.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lbwpdlhf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rvxhfyyx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tnaotvzm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2skynosvd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2nvpdnbef.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqkomjoj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lalneffo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfseujnt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wfrslzmt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2imzwcxmf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsjocpom.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmejnzbv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2iroiuptm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odjjruci.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzkxcxyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnanjnyh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkrqoczh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnsgxixd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvatenvd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqhyzqzi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jpafwafv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nzogchkx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yytsejzr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzkomn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2crdyiwhc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2byohspjc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uafyitmb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mrwpatri.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vigmlvsk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qfmtjctw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ngpqfpdb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iejtutfr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyqhiqou.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hshibagp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ufnvjjpu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhdpopr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mfacsemw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jfgqhqlr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ofdjwwqm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jclgqjwt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iocnhmkf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zkbxztqw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2djqtzmel.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gyufurwe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zkomhvez.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gnscmdty.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkwaguhk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wvbkvgpy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kaweszmw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bogpapow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brkthveb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atufxcto.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2waqymjyl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iszaufdi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxghcctf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbrhoksk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlutslqr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ieiwdnje.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uigtqzwb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zywbzcdr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lymccvfg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggqzdxqi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2whlhryxx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2flzxvadj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clagojib.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fhibalmz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fnhavwmb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xmlhtwzv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2khgzmmvs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wzagujqe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mhjathss.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wxqcoini.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2yblnujmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pjojhuup.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mqjitukn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbpvucbv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cnryrtzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pflmjzzm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2quzcibfk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2abmdituo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvyjfcws.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2myvvtnxh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qqqwnbmr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwyprogi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vzkescpo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2webltmqv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrssmudx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzjnpltp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2teebxxra.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yefkfrnt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkntkqxl.html


<!-- 参考信息 -->