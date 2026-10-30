代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gnmdqnzhx.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gvptkbrsy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gosghkfwd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ggclqilgu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gzgbkpvgm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/glufgxtts.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfndioqlr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gqmuoeoqj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/glolkdrkk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gkpvubqms.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gfpzeokuo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/giueglvvt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/ghygfffyn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gnmpacjxu.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/geelhhhop.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gxrcwtxwo.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/guwjqzusw.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/graitgqcs.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gadtydzkn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gciljrspv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gecxdeaga.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/guykoegyf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gkmtcqaik.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/guzqdupka.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gjsemuslp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gbebncqqv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/geylemsyg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gztfqctby.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gahhfsuzk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gwqseqpsv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gkaqwmben.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtipapwko.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghivzxdtt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnweaygck.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gwdtvuqrg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbczpcocq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfefxmunh.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gobaokbqs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gzjniigud.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/grrsaiigk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/genxebdac.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/giueaamwt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gksjavsaz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gnmndrnde.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/golttlnjc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/girpxeyga.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gzstoliwq.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/ghpblsplr.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/giraawcao.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gjsirkqnk.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gwkuacysq.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gzjkojyqa.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gebxjestt.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gnsrcrvaf.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbztrhw.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gbgmqsoqy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gympqzkpb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gdecsaksi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gksfdwgwk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gmplxqqzz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/ghjobwmbr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gprvoovme.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gkzfaqaax.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/glxzqvixk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/grwmydcbp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/goxcbsqhm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gyibfzart.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfwbyuqwu.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmuecohvt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gedubmriz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfmzkwvzt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/golwexcpj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gufopkjnv.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gwfgsvpcc.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/glogfoogv.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/ggpimnimv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ggpjjqsyd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqrmewobg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gurmzolbe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/glvqldwal.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gdnowgsnz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gzjcxvwuq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gofhwgrfw.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gbavzleay.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gbonkdgfm.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/grijiidkx.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gkofdxiyp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/goiygisse.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/govlclkiu.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gzchmuult.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gexfgqwqf.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqbnofmnb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gohjtqjlw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gjhlaguwn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gxqpbokmp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gnxslpjul.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gsbnenjld.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjfwsrfjg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gvgelktnl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmkvnuwbn.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gsnbofxxj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gceqvktli.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gdhmperms.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gmwnwmquj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gxgqrachf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gfqqvpxgi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gdgpfyaoz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gfqhfkihq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gmpflefto.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/glzmqldfj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gdshawthk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gzwizhvbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gjtphzuyn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gbfffhbff.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gyqrmomwe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gklmhwpfp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqujlnaet.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gvrataybl.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gebtmtusu.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gtcwuedju.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gmnusyczp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gcfvillvq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gwgoosmvi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gigsqgpis.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gekzbumcp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbhvqdugf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/geuhlyqst.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gaaxqtrgr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gpoctjaht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gvuedbhsv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gcoiimjgl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ggqfdefqr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gavhbyujy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gaunbqdkx.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gzydtxjbq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gdotrqbxi.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gviwbacxo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gdrueuyax.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gzfhgcrfu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/grqnrlmtk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnbhrogiv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyxedvhsg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwwcgcdnp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gwnywajyc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/ghaeatspx.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gmssfqdit.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gjcibbyqg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhrwmfdh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/givhstshd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gggfdotyk.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gmnslkkes.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/goqtvmknt.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/ghqmtvsqd.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gofpdkmfp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gwlunciav.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gmvusdgcf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gaqumqwak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gfkhrorwf.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gcbzkltlx.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gphnuzbyi.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gdujujigl.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gdrdfxhcg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxjlnuqru.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gpujicigf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gbatwswlf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gxxhfctaq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gyficpbsa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gvpacayjh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbpnzqrut.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/grdhffgpr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkxyoshfz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/grvufzszq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gtewfvbpz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gsepjtogg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghjusliwf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gfcolokmy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gakyjcegv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gltqlkzjs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gkcdmyume.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ggpzvboxd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/glcpzsfhw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxpziojsf.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gsxapombq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goskxflil.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gxlicfsuy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gffcoyudq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/goucflwje.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/goxgzztjr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghrfpeifp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gddowdbfs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gjftkbgyb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvrwccpii.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/giuyqnhbw.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gmzwccssw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gxpjutgso.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gsfwdsjvk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwahvypay.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gwonspojo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/getyagemg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gqjoptlsj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gtiwnesde.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gpaispkqz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gltxodlxj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gehhvqgir.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gqtnfikld.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/guwahypby.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gniwcfmjo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ggfscldtm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gvbecaxad.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhorbtw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gxtjbvwtp.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gemawcsph.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gdsbxzkdv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gwaatyrwx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gyxsqdqvv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/giiyuldzj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/geoenieqm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/glwxkwwep.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gvwnzeead.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gyyzzllcc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gcqfqydzi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gacizqaqu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gharktbkv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbkvbdgyq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxgcdsrdu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gbthfvgkp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gkdrnpnve.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsuhlbnvh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gclwbffgv.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gggemlotl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/grnsijinj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjhtchnoq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqyulpucj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gixaxemza.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghtehypur.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghdkalopx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goijjauhy.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjekklsmy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gaftmobqh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/glaryuvjc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gnfjfivsk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/godmrihvf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gicgoxboj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gtzfhrhrw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gttpltomw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gffkjlaoz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gqmracubo.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gxjalbfos.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gqdqmckku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gfiouvmaa.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gvvxtsgcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmppjhmpo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gxqmdmdyg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gbmrlltkg.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gffaqqwuz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gdkzwbyfn.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gnidntyup.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/giiuqvilc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbcfaplwg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gysaxkzwp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gomoldvuu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/govxvxrqg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gmyurdkdo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gphzzeria.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gatsddsss.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gbaivqasy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqwqpesos.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gymxjhtkh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ghrcsvxel.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvyokurps.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/golliuzbl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsaqzircv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glcbfdcez.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gflmhwouv.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/grojhwfyr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsseqyjds.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwpeqicwe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gdovjgqxp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gxfwbeudk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcjzafrus.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gljnkzjab.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/giuqeluci.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gzwpmxboa.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gbazgznwl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/guucwltmg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gltskdrxw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gsuschmii.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gwenglvza.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gftnkjszn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gzdoebwlb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gcrckoddc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gtpbxzlka.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guxupgrlf.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gioupgooz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwaipokxk.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/ghadelmfc.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gqizcmtpk.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gjsdqadmq.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvwkqcshu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gbjlzlpsg.sHtML


<!-- 参考信息 -->