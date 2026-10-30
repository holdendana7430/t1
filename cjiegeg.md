代发 wailian999

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxyxarjhp.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghyszkgst.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqkwxqhpp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gmvanwgoo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gzzuujuih.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gcvflxmis.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/goesrjydj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gaffraxin.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gbouflbqm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/glmnpgxkm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggkeiqhgp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gorneoklc.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gvtascyrb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gmvprccmn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gbeznusnb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goqwtpnfg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcmaxtekh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gzsyrukcp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gqayvowcx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gpkeziybz.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/goefalzdw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gbbmcbzov.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gqdicdxwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gdgntvrhu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gpjniitev.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gxeoyakwl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvcxbjoh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gyxkezwne.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/goonigoli.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/grenoshhv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gbuyycazc.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/ggsscrqvd.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gojqcpqaq.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gnzyanbxj.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/giennkimc.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gvwfdairs.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/ggevedcvx.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/glmnwmwfa.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gsikxzyjn.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gagjyrshy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/guydhisoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gmzmwegmd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghparznnd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ghqgpsida.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gwfiteatk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvhgmczy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gefcjjbcq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gxcxywzdp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gyjtwzezs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwfwguebj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/ggsvfqyzf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/givxrxyba.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/goyiehkew.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/guflvyywf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guszokucs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gzlunekqk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gsfhlhxvq.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gxdcqjjrk.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gknyhkxwj.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gahlckbuj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gtcqfqnfx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gbjcuuoiy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gbgwcaeta.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gnnoyakrq.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gfsvcleak.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gkpfwdbgk.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gkjggenpq.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gsiowfouk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gehebdqhk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gvnyjhsmg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gtjocmedv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gbjkimtqn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gbghnjtdo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gyleopvty.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gsliqvtsg.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gvaonhixm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/glousbust.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gscuyficf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gdpxzvayn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gicnzgvav.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzbakrfla.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gezzqsona.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gmyihcobt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfyijmkuv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gpthndjro.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gvphfqhqm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/ggxojakpl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gfafooyjo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gboymmxlg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/grvfjjnzw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gmiaadpeo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gibxnqtgu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gngxrlpcg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gfapdjewo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gvawzbulu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gzxkfdfsg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gfhysgzcb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gwrqiovsk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gwwyscato.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvzpmptts.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvsoeteag.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/grqrnuzow.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gzhtfzctt.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gsqmzarxu.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gdfnvjjfb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gksjgqcki.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gddbgvjbf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gotxxvrzr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gfsehjcjm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gfarirdoi.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gkrdkpmdo.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gyuwwbfkl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gqcicnrsx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gimxtmqom.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gezstpxbs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/glcvutfhr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtbjkovqe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gidsnrnia.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gnvucreen.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/girbsmwuk.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gewmifuwu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/giuhecxoy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmqqfcrye.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/guctjtzev.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gyjdsptgh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/grmdaceqm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gcnhfnciy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gezvgftop.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gmasafjym.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gvghkkxue.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gvvnytnjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxxyqebib.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gpurbiahg.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gyjjckncz.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/glntvqztt.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gcbdpizds.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gavsscjdh.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gyvqnlnqg.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gbjdxcgki.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gptiejkxc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/glqsxrswj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwufjcqdy.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gfbxgfvum.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/glxyanqoj.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gjhrfzvow.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gurpskard.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxjfurhhi.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gkbsabmej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/ggkhyhhrz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjglrcecp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtdirzsia.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbanbiexy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/giiklhsrd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gjtkciqja.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbsjsotvy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjmfmfwtc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gzyhihzxf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gpmxxiibj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gnbmvfuph.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gywxxvpqb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/guswpcmbb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gyukqliom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gzutcjeoo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwqxjzogu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/ghrmnlzie.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxronngl.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gtxqfndmn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxzhcwwot.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gsicmnrov.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gcznuqxkf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gahqwiwqn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gslldkhff.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gmfpqgyyv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gutcdthjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/govlamjsq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnispzuuw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbnvzbaab.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gjgzdjwfx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gttgudyte.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gwntyqwrh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gifeczygl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glrfwuyed.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gmambavth.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gqwzfhtpt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gwgjfmawu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gkmucgndn.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/glpuqmvyc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gqighzlet.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/glshvuozr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gywzqtvdi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gacdvasfx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gpcanerds.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/grztmvckc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gorqvcfdn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gbojjhhmr.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gqzvnftxb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gxelzqqfv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/glmucnqyr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/guhegvgxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gyuwpqthq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gtuyezkdy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/grxywxiys.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gfacxxlrc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gwpzlipyf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gkvaoidrx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/glomlbnxr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtsrscoty.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtdftugmi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaopglqql.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvsnvzgbz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gvlcjipuo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtauvphxy.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvodaduoo.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gtkxyiwyy.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwjbikuti.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsuapbfdv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyabbcqqm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjhmojptl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gidmkvwtx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzewrxlif.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwilgnbhp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpewbcrmm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gcwfusxfh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gwmdrlsjz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gaznmlhsa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gddeivdds.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gwvfgqycm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gdekxxiil.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gchjnspaz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gumuypuzt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gjfmtvxxr.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gddxbhxbd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gcsftjjoa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/guuyojnrv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gebfchjfz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqgdonx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/ggruegfzh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gvjxeywuq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gbcgadymq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gdcbhcazk.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gxhwlwwss.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gglrdrqen.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gauyyiegp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gcisrylan.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gtvpnbqvl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glxsyzzxn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gxqgviqds.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gofyzkehq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gmavbipvz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gvmlojfuw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcmrulvmm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxirlpjhe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjeffdkeg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmnzmppby.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gctqqovyo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/goegqmqpl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gexmkhllp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyydvkdbq.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/ggnnkyrni.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grqlhkfqu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfzxzpazd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gifpyhykt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gudfdvqfe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/ggkmmogft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gbcognmos.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcqkzwfms.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gfekuatgy.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gnrmjylld.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/guagafwrz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/ghoskprvk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gptjklfll.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gpaqjvdhi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/ghpzekysq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gqmlffoul.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/grcyfjete.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gsouplxnj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gagebzyqw.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gnkzlvgdq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gijcymwrq.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gotceksco.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gxgrkkzyv.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gzzlgguef.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gieahxnfg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/guwpmijqs.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjnjovdet.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gphvizhlw.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gjzgnlmbb.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gvbefqbhj.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gkjzacmlk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gdoiewuqs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gmsjlxwna.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/ghsqekztb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/giosvblac.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtnukqrjb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/guoqbjygu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gqmheynqg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gamnmskux.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gryoavfuw.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gqrgiqcbl.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gtvzvqmri.sHtML


<!-- 参考信息 -->