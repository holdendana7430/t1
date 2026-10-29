代发 wailian999

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/ggecdvoux.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gjeskjaqb.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gprukfves.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gakcejtcv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfyijxpjj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gxayribfj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gryyehauf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gjltisdhn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghmcvuajc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gvttxvexd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gkjxojiwt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsztmutxr.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gpaievnlt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtmsfdllh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gcvbatqux.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqohyarxh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gillqkvcu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdfhqmtdv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gpzmnsscg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpkvtbnhg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdqrvoxxy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/ggcgtozaw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gbiypeuof.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gryteevfu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gnicudaka.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzfvwsppf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gpnntllqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvtiwdjmu.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gwpyfqnxo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gmszsrbma.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/ghhwgmzlh.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gvinkzgpj.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gwcblhyhp.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gswnssbeu.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gqzcokexd.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmhmexpwb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gufezgblr.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gjhddehiw.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gqfiacnpt.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gyimxlsbz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/ghhfsfier.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/goiojecox.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ghwexkrek.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gnkohhhqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gqpsawnwe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/godrzjnke.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gzodvfrsr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/ghpkngexn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gxwrymkqz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gdlmouaxj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gpjvcnqjc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ghewugpom.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grxqzonvt.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gptxarisp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gorwuhvmz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbqudjfey.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gbvtztvox.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/goqeuthgt.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gdbokyhir.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/ganlqejbp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzrawjimi.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjxnartcq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/glcovqabf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gfyrfxtgf.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/guydpkhlv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gimwhplck.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ggbmiyhvi.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/glqgrklbj.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gtxoairkw.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/glnrhwjtp.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gfmeiwvot.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/goiwkarci.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gxdgfnqke.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gxbgxrhvl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gckjkctxg.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/glqkoubdi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gtsuhfrne.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gnynvxrvd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghuanywxb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/geounuoze.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gumqgdqwk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gharcbdat.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gqlwrrdlw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gffhrunhw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gtkcgjgab.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gyrliviau.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/giougaxoa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gligmnuwt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gfkudsacc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gwzmwowfo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gucmzpjdu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gwbtkvwvp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gbdzqqsih.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gdhfffoze.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnnkkuwwv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gucydlcsw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gerwsdphx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gyxczgjuo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gcpruiqtv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gjtgkvxmb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gyblmxdpp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gmvttsewa.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gzznrghgz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gyzdwrclc.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/glxwaokho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gwpvocpee.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gbkvthnvi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gwvnigbrt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/grjnvmnfv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/glhgvyiyg.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gxcuyhlsu.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gsodypmpa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gloxkhrde.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gjhkviksv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/glzoeesgi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gswsvucvg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gzjzizpga.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gjdiwrhoa.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/galsuoyxw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gawykqahk.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gflxvictv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gckgumxyg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gbxsbuwmx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjsjuglwa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gxczearyb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gryqzokmk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjlnhuuqp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gsbtyozlf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gpnhyhrrz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gfzlmgllo.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gftspdljy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gyeiypchn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/goyeqwijg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gsklfijyu.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gsxbzjify.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gmwnbraxg.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gteggczwu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsffarg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gtknjhrsj.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gwvmtlfro.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gfpszacqt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gdrsvnomg.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gnmdiwvjy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gclhgmnvj.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gvdfxfrtr.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/ghhyhpmks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gwuuzymwh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gjiashiek.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gjxelxuqn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glcxfmhzw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkxrtlmnh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gptivxkjb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkpvbdqoc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gdpcrjear.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gcmdsdxmu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjomuai.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gdtrmoulf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gijhglsai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gihbdncct.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/geaessvic.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gllclbfdc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/glxdeugab.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/ggvbcrumj.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gpvwqzrrk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gucqehkbi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvwuqbpah.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/glibyojrw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkatytjpm.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gyitxqald.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/ggtwtgzap.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grkaamywh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/guzmnlwmq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gqrtbrwiq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grqthyhbw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gmdsaoodp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvfhkrbpg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbdoouvsb.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gspnowxfh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gopnoegkd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugzeccfl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gswxahomn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gluzxlfgd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gsrszjbgl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gfggqtacx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gjdfltbpk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gyzcbiwbs.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gpwlnrzjl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gojrzlilf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gnwzrwhgl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ghdjgdttg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/glujoshor.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gktmsdfmg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gjuajpmks.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gaogajxpu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/glanrccdg.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gnemfjwvn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/guxbkkwvf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gsbuatcqm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gsiukxsve.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvwouneoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gaanqsmny.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyipiskvy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gmjdmmspc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gebktasxw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gtvkcdioo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gdsbadutq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmkwucdrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmlhjtmim.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcjmtdhzp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpbsoqsce.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/galrmwnig.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnaghbkyq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glveprpxf.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gqzixmarj.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbsivqofj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfvjavzpy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gusjgscml.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxrfssmcy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvkgercow.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjtbiqfqv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvirdigku.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guzruppql.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gbsdevowx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/grbkexvna.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/goqqzhgrg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwqfigwfv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/grezschbl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gkhoxkaxl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gtrjjdlrt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gaqywcour.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/goijanros.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gqfpdlxfz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gnxudnzbd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/glvtaqrdz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/genxcirhc.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gnciyhzlw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gppmyeoyd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gafbkispi.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gctjlqkrt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/ggqilomap.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gqanekzsx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdiulklir.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gatomgece.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjxqandun.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gcrmgvezo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gfxbffeyn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gtpagerog.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdrgsxlrf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/guzgvjcfx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gkemjjzms.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmptxzelh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gurjynymh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxwvpmqbu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gamcaypjf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gdtfgdnyq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzcyrquer.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfbzfuojw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gffxzsuyc.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gbrrxvkem.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gerfokrqo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gbfllprix.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtkalmbt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gbmhxcccc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwffmyugm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gijpwprqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gxvvdojvh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gzbrwmaio.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gbgtpmxun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyahlrgf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/grsopnjjf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gniyavyej.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gevvjdbao.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gfoubpbmt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gndmszzqd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gmfygzcfe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gjncnorts.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdphtwltt.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gglebyxkx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggorhldkg.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gsbtbalim.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gqccsxcmy.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gayyomxpw.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/ghlqugzkm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxtrsgkl.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gaavmioww.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gwcduwpwz.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gfqugibta.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjwwjeoee.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gehomeoav.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gpaqpsthz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gcnyuifos.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzeduacgv.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gckixjdgf.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gliljstvp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gkopxsgaf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gfgsrluxm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gnvojjjpe.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gfsunaxil.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gqnwmtpbi.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/ggcgwvigj.sHtML


<!-- 参考信息 -->