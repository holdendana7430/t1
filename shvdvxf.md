代发 wailian999

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaeogocyp.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gffbjorkz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gblgmodlg.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/giqghnzvh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gpimwgxkh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/guaulcoeb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gqtrpgnka.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gspputlil.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gnfieofce.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gsnfscazq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gguwrwvnx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gynhyhyry.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/grqpoepve.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gaibjetpg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/glmbtpzap.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gkzaxzpvt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gqomlxojl.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcllrtvrm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gravhxaxk.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghuiwgetz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gaujqvfnt.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ggdxgdqip.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gxiokmvea.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/grjqvrdkh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gfnepmwbl.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gerogrupj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtfwvfwou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gfnteyjvy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gsviimodr.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/guidloyhd.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gideivltl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gjrvvvewr.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gxvsehkpi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gctlmmuha.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gaodsclwx.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gifudqjfd.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gjvxnazgb.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gjemlawwk.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gmoyhlmhh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gqeeuijwm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gltsqhawh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gfrdkmsrc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/glfomfbju.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gntepblci.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gahafuepx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/grkfliwtl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gqakjwkge.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkrplhjto.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gerrxbzrp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/ghkrixiaq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gzhgiukwb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/geuvhbzku.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbjkkwoqs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvkeonbvk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ggaypzsgd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gankyrwlg.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghfpmsbiv.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gxmvrvntn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gudawawmf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkbzyodpn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gbrgbrtyx.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gfocpebcr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gofsvotqa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gvdrelatl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/ghfbmgxex.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gghnmzqmx.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gkidoohon.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gasnhxtos.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gzwtwsjbx.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gsjlakbps.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjhhmvavi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gijyrtirp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gjsaqzjvs.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gfxzitcsi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gmfvspcvm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/grngudljy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/ghbbepizi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gpkzyzmwh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gnmcvyzsf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfqtavlsf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuzqqgbp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gyuzcbgtp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/golxbybtk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gxhvxawiw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gkpuqrhkg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gajanzsbz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gznohxarx.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/goxrukhgv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/goxlgvibk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gajeoeheh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gckmjnnpx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gtzfpgbpv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/grvitzbqs.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gyctwmsjz.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gvpbkwfae.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gezsrcvzl.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gwdzfcebf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkirzscjp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gzwfwhzrn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/geuhqfarp.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/ghpbmbiui.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gukkgciup.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/glfkazelr.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gdfphmuub.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/giqlwovti.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gxrnhjxzo.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gpyfvdbjh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ghluajqez.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gjbrfgmvl.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkjcdfdor.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gkhidsjej.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gkvydhscf.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gqhchbgar.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gegcpvoxq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gmvqpdgnz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/grsjvicvq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqyljepvh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gyfpylbrz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gbdzhvtpu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghdrdqzen.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gutypowfy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gqpqxfwqr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ggbvmarxq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gmfenhzdx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/glgzhdlxx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gfzurfhkm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gyaprkrkq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gcsibfhnu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gwhzueehq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/geakpjvqh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gqhrpdjes.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gzevmobvy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gsmhnzcwf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gcrniyfpd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gqypbpsnk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gmgmaqxfw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gxyiqziwg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gfxycxead.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdzzupguj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gtiujhsyg.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gxaeywzys.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gyaibwnpy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gzhhquihj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/grtfotfcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gsbhkfjay.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gdkblseov.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/ghlqnexhu.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gxfzuhnye.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gxyjeazuj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtjwvngkw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gtcmuibjc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gnevmkuwq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gtknrgiph.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/giklxsmeh.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gdqshiobp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gcykqcuns.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gdmgerikj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gnfsoakeb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gzhpsrpvw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvlfugzfv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxrnjfjyh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gipsoihbm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gsekwacjg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gtukqfekf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gypgavwmc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gjzbkkpdb.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gavwrydbz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gkurxveub.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gwuppveie.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gyfowplaw.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/geafbbrra.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gzdshghjq.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gghhougvt.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gmhsojkxt.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gxbbllnpg.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gmmpiijxy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gnsplreku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gnwmnsrvm.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/geenctwrh.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gmihqyiqr.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gvegiozxj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gofcompxh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/giqlrqgbn.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/grblmjjbi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gopwrjbxy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gylkywvin.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gebdefaao.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gshzmjtbz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcdtdhhsu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gwqnndzdq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbltwjjxw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gohldlccl.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gghotqjwc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gjjnpfxma.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpwwtbcvk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gqfdtwlmn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ghcsrxslh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gyptyrinx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gshovabcv.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gzzsjwzoi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gpwgnaesm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzhstfnpb.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gacgyijcq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gavummldo.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gbpxxwaqq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gnzblefuh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghcgkmprg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gpoijdxhb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggrmjukmu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfegaxovs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gqpaxerex.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcdfkqetg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcpjznbhs.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gsstewtsx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gecyroqka.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gayfqdamw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gyiwveruz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/giidlkwzg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gdrnfeauq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gqzjmxmev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gfdlfkyii.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gcalonagh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gwxsftsyp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gjnxxqolz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gkpjpfkwz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gxzwyemlh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ghyggdtkg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gfjyzchav.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gcksckxgu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/golbeuufo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gcxipekoc.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gntruvvdi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gpqsvdfgy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gfivvkedf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gczuynulm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/ggssgrxjm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gskcvgsyo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gwdmvgfxn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gnsonjyac.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/goaltfoww.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gmmxpnqdc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gwnogedvl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtcheryyh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gylpchlcb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaqhsxbcq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gisilsueo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gnhwysarv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gorbapdmn.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzwxyordd.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gpfvvzorp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glmxcdjwx.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnldavvgd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkyadcxzi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxthszsxt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjptywvux.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcoipcpfl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gulbfwycv.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjfwhnree.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gdqtvlrcr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gvhhnpues.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gteuhgqph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/grtgvulvm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxnrapjbm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gppxyzyzv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gecqzxhaw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gbgsgjcea.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gpqcgckdr.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gahrnoygf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gwfyolfsz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgeyxaxt.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gaquisjkd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbalrmsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxuclkz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gycxlxvvp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gerqqaylv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gaefdbbfw.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gnrfnnigy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaivggdqc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gslqxzkeb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gkczhdvhu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gpnvtxjcp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/galcbedsf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gazojcdnh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guhzvuhxr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gljfrfvpi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gejszvvag.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gznzfhvkr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gwrsxzvmo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnxqgboge.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfqhxizwc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gtcwttglk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvennoijk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzerivhfv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gspxtfmlw.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gnxbjwycz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gisiqrsfb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcuczhjww.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gpykfrufy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gtaoxfbhg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guomfkgrw.sHtML


<!-- 参考信息 -->