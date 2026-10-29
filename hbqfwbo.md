代发 wailian999

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gbczmuodv.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/grbzbuxdl.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gejqmitgi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gbbfzqiai.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gqrotkyxz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gbguomkkp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gzhtcnxdu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/ggpyttqhs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnpnjlzas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gsdkhdmhh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gxsqxusnn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gxofcqege.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gzqknuios.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gsikfbcvg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gsuoczrec.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gsirueieq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqroomuoo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/ggvzwlhvh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gllnafhmo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glipncywj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glcqsqogz.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gyclrccyx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/ghkxxkyqy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfanlqxic.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gqmoboefp.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gsieofodd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gpmqqkaft.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gqapykvis.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gezpdxtqo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gtypkylkw.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gtjfveidw.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gecuxjvcv.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ghwkgmlju.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gccxafyam.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gzqkierog.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gvylvaszv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gxnhegypm.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/glfinakcd.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gvvscyojg.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gnywlqsdj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gvwzoaawa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gwsycsvvi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gmfplucnn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gntkqwzcv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gchuvccts.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/grfbdjosj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gnsvmxfsi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gqjytaksh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gakxhdurj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvrshfqzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gbxtxjaai.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkrobvsgc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gggdnjozq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghtaywbzl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/glltqgukt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gwhnwsnse.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/ghbrzpsvx.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqhzsuyvr.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gubsorhkt.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gfxnstwnx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/glnwvjxax.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ginaumcjq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gnzhejmse.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/georxztzj.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gramohlta.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gywkvblns.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gakpdttnx.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gjpzuvhub.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gbdzmiwxr.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gkhamjosd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/ghubsqkxp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gsgairpqi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gxrmkkhhw.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gymgnfacj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/ghsdwotad.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gnkoxcdwv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gtpvycqef.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gtowemjxr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvxaltrxk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsdwckdm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gpgaufhib.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvtchyuvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/grukteaux.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/geigwkwch.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gfovaexwy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/golqmoeag.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfvqtntjd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gwevkmimx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gtigkjkkz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gtlxwazgu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/glmsiypbd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/grbjlwbbj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqnbserck.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/giyxzpaad.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gjogodkds.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/glsoqzyss.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gxokymcwz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gfwbgkcpb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gdtepqerb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gdtfdyzjv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gybybwfak.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gdmimsxrn.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gauovxgea.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gccrgifmi.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gjtbvslie.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gmlnblmva.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/ggtafpgub.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gkhadndie.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gocjmvupd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gyglodphz.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gfhlygtgg.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gocnkzbmg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gkocfxoha.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gfowkdhph.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/guergruev.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gatplywkt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gbcwdlyee.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gnyiyhlbr.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gwcbisvkm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/glsoxwhgc.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/grrsqqvpf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gbhksekch.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gyudcwmnk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfltcfglr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvehwvuta.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxwsphj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwscguzzt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gvmmaujkc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/ghwrqquyz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/guccpnjma.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gdtbybglo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/ggyrrefbw.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gjwkgibfy.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gpljxxswm.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gkvuyfzof.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gxgeczngo.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gxzrpjxjg.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gbwypmabh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gtojhxcrm.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gkumfsioc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gowbswlse.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gpvoosnds.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/geurprqfa.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gqijapbqu.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gqamsasfm.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gntszmstv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghdeijdwd.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gugoamvgs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gdymucden.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdgvirqow.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqbcppkmi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gcexvthxy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grnkxdhks.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gemqppbrm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnykudcrl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gspqembsz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gzaazztor.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gjurwzfxu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gertiakwc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gusrkgqvi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/goxagdqof.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/galnkzwci.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/glpdspxby.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gecvvvsnm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/glmtdtgun.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grpmtlvfi.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gushzhozj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkcjmtupo.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gyycumgcj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gxalrlbxv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyjztmjqs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gjivdyhhw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grisxnnmc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gulfziqtf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gpexnfwnt.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnzuxtdbn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyennatmt.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gpxavoirl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/grptpikvl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/goujiadni.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gbpwibqnt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gnvgfzvnh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gciikxkuc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/glzoibzso.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gvhyrihah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gyaohnpjw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gjqnjwuan.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/guzgbxnsr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grbctgkwg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/guzwscbqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gjqmllaln.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gpquqdxjm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/glouaixim.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gvpujeddw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gzhpzzdmv.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gmwdeqchd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/goejutwxs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/ggtirvuvv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gpfmrevfw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gupqacyky.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/guraaztgz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gratboyym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gomcrprij.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/ggzuiiavv.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gsxldulok.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gqqbttwnt.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtclocdew.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmqfgkmdc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpunnllff.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gycuyjsep.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gmkhpdxpj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gscympyee.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkczlimrp.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/ginknwggw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gocwkeyrs.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdsbruvac.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcybidxob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/genumxraw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gciotpzmz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/goxvkvnls.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gazuqkqwb.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/googyjaff.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/grwzctshs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/guvbqurwa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/ghwmzbukf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gxqajqnfm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gkdbukgdb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/grvoborzu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gdxzjvkfk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/goxuwatcf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gsuufvdlv.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ghldqglzo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gjwcwqeeg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gaqzdtwwg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gchzmapyo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gelzviblv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvfrizyzg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gcrxyecoy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/glyfjcvkb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gzivjlpby.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gymnuewjd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpueghfze.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyvkvoovd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzwpbtc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gbajnobpy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gcjjnquvq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/giojvkkhu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gttpigqfd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gdgnmtexo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gahzvxgmg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdoufjizz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqmwccpob.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gczvweimr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gslawniby.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gedvursjq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcjnyqijd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gaiwiinzz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghdclvxtk.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/goawmtqcp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmmkgczmw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/guqytikkb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvmecxazg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjdkncvrp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gfxdtxhco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gscmmecta.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkeffitrp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gnxzuwteb.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gghwyktxh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gxoxbapik.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gkrubulwo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gfckexsry.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/giabwwrxd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/glgxjjthj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gghsniotp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gvmkcyxdh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/ghpevfayo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfzwpuiyw.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gldvudnbu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glspywlyy.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzpizfmsq.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gltcjkgkj.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gfllpsbdb.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gnnbehwtr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gojvnxdgs.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsqjauqco.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gpduwejsj.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gjspeiydc.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/guncjzidk.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gnhnlusqc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gdxtaywtu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gbpozdlfz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/getsmqcxz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gqovdaatb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gywkrelnr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/ghngpzrsn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gywipihbd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggtpylftf.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/geqvpfcew.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gsklnoqaz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gywhapryz.sHtML


<!-- 参考信息 -->