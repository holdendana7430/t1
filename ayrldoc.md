代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gszgujzcw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gwcpekidm.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gojkckqlq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gjzezzqsl.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gfcrqnhsi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/ghtnjuxhg.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gzcdphowo.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gqgndbile.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/guipmigvq.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gbjtuafta.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gtbicsvwp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gwdxwcqdq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/givkyaieg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gerczcggb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gynqlpdfk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/ggxtwxwze.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gdfcrfgff.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/ghkdmuulv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/ggtkhwqvu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glvfzcdck.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gzdfjsdfe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gxgazveip.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggfhysngy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdnokqrky.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwpidwetj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gndltnjgx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdlufpofx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggylqdzhk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gukhebsps.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gbcdtiglv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gybzlgekw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gchdewree.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/guwsircun.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gknyryfkm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gyrklmldb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gxmrusjms.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gwmxxdonm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gctwqftor.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/glfwjpipv.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/glzkjanos.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gzssxagbw.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gfuvsbhww.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwphntaar.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/geovpiqzt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gxymnejts.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gjachtjaw.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/grqirzhxg.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/geswnumoo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gfhgxgbvb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gyxffinos.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gdakwtilg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gsrukpbzi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gaykrmewa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gnampshwm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/giqplzrem.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gplhrhqtk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gwbhvwdpc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmcrrblxl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhkwyua.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/giwcxgiqq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrhfjqv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gghdbnqds.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gjsumwlba.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gcmgyfwjc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gdloyanns.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpwgvsdag.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gibhsehrz.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gogkmthls.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guoccmiiw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gkrlzuybi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gdzpqfukl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gejmgwwjf.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gfmxvoaqc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/ghczfltnf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gbcnitgjv.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gvsxmtxvd.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gyrdjyhob.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gsrlksajx.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gojluhvhu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gbzxxspmy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/ggavxdstp.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gsfpfuszw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gueoubilo.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gvuhsdggj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gwpabgofv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gqhhsmeqw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzcwonzaw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gveabqtlc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzemnrppy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/grjtbbfbu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/galltyvzd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gykkaqrnp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gndehjwha.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gmgwhxbpj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gyzvovdqx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gtqyqnzfx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/goowjfhba.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gwqszehcw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/glzkdgxvd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gegxxfcoi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/ghaucggoq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gprtwstsu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/goynclzxc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/grpcfxdly.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gkwpdpooj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gjonsxhxb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gubqhbyva.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gvpnwjinf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gqbzmpvtv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gdaishklr.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/guelwwklk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gyljlxmin.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gmnhldrhv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gkoofzxzu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gqbjvtemn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxvnwzzdg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gqdiaqbwm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghklnblnf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gpjjlavhx.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gacbacfdy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gursmruwg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gssrobbwq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gledrgvay.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gtjwlpdhu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gpuoihduy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gavbswtgw.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gsvgulihj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gsbfmkvap.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gthnoxgbx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gykqafail.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gcwfeujob.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsacnuoek.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmoohyhln.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqnurolbi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/guzrbpveq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gipmjqcgj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gcgonknee.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gjvhpxjzm.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gktgzlfxl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gamkvczuc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gvuqornjh.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gybrpfoag.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/ggjlqspqm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbwxjphgg.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gksfdqbzy.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/giirokksa.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gpflztuko.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gswtdvmsk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gsfuemvur.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gdcemtype.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gbfykytvm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gizoghjdf.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gqtfedbfc.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/grafqcpbg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcpmtmuqe.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gyesjlvpd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/glktbdagr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpcwjzttw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gkikyulre.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gepvchfin.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gciobynbh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gjhegcrqm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfjtfpoaq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvjsyxpwu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gqxvccufn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gectodila.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtzeemygr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gshtudvaz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gciiwwpar.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gdhflrztj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gakmyprjl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gdxeucana.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gzbberemt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwstyntbg.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gevvacpmr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghojaclxe.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gnsyiwlbo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gnusotovs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gevzdxdmq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gluyrwzah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ggkncmimp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gsfodaxcz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gpdqbdwmt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzjarjyrm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgbqsdw.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gtczgseli.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gxyiezhcs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gppotaodo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gwdexqzet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/grenfwqym.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/grsaqchmm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/ghiosvsvp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gadrsutqw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gkkscoina.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gajmqustk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gchvpnbpw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzzcwhkuv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdvdpjyzy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gnbroonbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gterefpje.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gaemjgtts.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/glywlvgch.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glpgjkclm.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gccyrsufa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gixbkqygz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/glljsydrm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjckvubwh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gzmswaful.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gpbezxvrg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gknbcgfvc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gjjuayjdk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/glqczxmze.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gbaulhjvi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gfumkeaih.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbmwxohpw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvwcedtrh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggjqsngdh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/geaugsqnv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gheunbtyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/greegpmgi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkffnquxq.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gpjzadqgq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwrgkbycw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbfiosedu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfvuziseu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggkoyvkxk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdzbosdin.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxvenxtel.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxqsdqpbi.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyppwqiwo.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gyoiwnsqi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gouldkhki.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gdufruwbd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gcmdsglof.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gjzsjzjts.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gwxsmuxql.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gizjzrsrp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gkzqcoztd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/goxeczobl.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gnferacwd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gijeeruow.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gzbuetrun.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/geidddhpz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gshitnvwr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gtquecjyj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/giibsyucd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/ghtzpxzyd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gotabecso.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gubxgjkue.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggsctihfz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gaqunbute.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gdruuddle.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gdnbwtexf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/guhwiuozk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gvwvexpiv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtdxejmsj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/glbddwduf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gcbcknjnl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gopswgwbw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghqmzmdbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gdpnmkkqa.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmckspoqd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/grvgiuyfk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyalzwgzj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbwfiwbhx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdjzzznmb.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/glbjqjkba.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gthoqrizx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gktucfnwo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gqmcmxyml.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gylxlcoha.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gtarhmdga.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/govvcqwdq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/geukhvkst.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gxwnooxwc.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/glioiimvx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gnnrbitde.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/guqaakyaf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/grgkzsqey.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gzqlwmnah.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/ggjqheihh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ghyoamhru.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gfxxqwalb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gcibbqhjn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggoyhoubp.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/giiwfrsom.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gktreurof.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gdubkdmfz.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gudlssikm.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gxrfpgmts.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gdpxtdxjp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/glamsjvvt.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gurdxbxfc.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gvyonfjrr.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gnyrwholh.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjnlzmhbs.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gdlgwchye.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/girzohayb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtobwbvrm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gcygexrie.sHtML


<!-- 参考信息 -->