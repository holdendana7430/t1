代发 wailian999

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/grqckancm.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghvunvcjf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghsojnija.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gqkzlbtkv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gcmytrjff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/grqdejkfz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gbobrcgvn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gwsqpwkot.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gqpuznzrk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gknslakdn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gahbawivx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/groiurvfn.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gobsyvutm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gtupdjmti.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gtqbzmoha.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goedgxldo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gsyvefipo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gldcedvjw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/garupigiv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gusbduyzk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnmstytqg.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gffamvnvt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gjpcnyuwa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gassbcqqk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/ganusnsns.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gibfrxbdn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gsnnelcqv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gnspforls.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/ggkbfkqiy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gjkrnrczb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/godrskvum.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gvtzmghuw.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gcowjzfdj.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gcatvpfxq.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/givsgcngg.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gmymqxebw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gtnvsumlk.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gvcxvqkmw.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/garostbqt.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/galstbqms.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gmjvbetqm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/glmaxpajx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqiirbtrw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmdjobvpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmvhmozwu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/geuoeqbno.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/grzlwpjhe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gpurtftxn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gbmhtoqsa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvkhxutdf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gtchzzxuj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxftoalct.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ggehcpcio.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gwiokuzvt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gawrjjwyi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ghufhonak.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gaswoalti.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gtfbkvquw.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gmwddovof.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzuksbops.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggcjwlkhu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gipdrlrtm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gvxkicmbs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gvtpwmldl.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/ghoubegco.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gkmwesnhd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/grtoiwhsd.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gkxzjumqs.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/ggepkldbo.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfutboc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjxbckgvs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gmunogjmk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gmbfbcdqk.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gauxmnpyd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gnqgvgglb.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gxoixelrl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/glmcfekje.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/grkzzfdhp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gvsmsbbpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gxsghvlzl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtlybsvks.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gfmghehqe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gfzitmyhx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ggwmrmqte.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gusoktjwk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gxegnrtwl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gnlnptejx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gibozuldk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gbnmknmeu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gywjdminw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gkpequryi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gvoehubeb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gvtulszec.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gpmjpfsds.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gfeuvzcma.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gtodkqzwq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gkvqxlckv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gujswmcyr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gzwhcmlcx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmpzrzqwc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gzqutskvp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/grfgxzxmd.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gzylugnhx.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gkoqjvxia.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gzbspokiq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gsnmapewb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gsuycaqyh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gteqypnpg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gqdhzaddc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gdubratpk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gduxpmmvv.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/ggwxrebnl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gtzeozple.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gounmtfsd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gjbdykcxb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gbxvcigkv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gpasernal.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/guohaihqx.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gplwkfmdy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gmffsbaut.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gwaswzadm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gafbyextn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrehnwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghjuwmnqs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gguhgolst.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gdwhubcom.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwlbvzwjq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gpaeaicsz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gdxadsdzx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gmtnwrxqc.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gcgzdosjg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gscqzeuet.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoitxttc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gnzyrfjwl.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gxtiievil.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gcivohint.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gkecazbrm.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gvrnbjuqm.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/goeurjjde.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gxpdqqolf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gzhlslqyl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gdrahylab.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gbopuggax.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqizoiuah.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gtwvmxypa.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/glhrzdvjj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gegacsqsx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gjweekhkb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gnrpkppwd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gbuxeokvq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gktqpbsuf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gxwgdtgmu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvkszowgi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gbmsazgrl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gybyxsoew.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghltqfzmt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gzqafrjvm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gapwxioyw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtnxlmexn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gnmxoqxgd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gtluiaxac.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gaiehbxbt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gsxkwbtre.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gmczvskqi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gkxqffuot.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwsjixxbl.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gpgnvorci.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gosigjork.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/guyacjjmd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gxffexiie.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gznzmdnoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gvfudedtk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gjkclsmww.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/grvlegonb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gwihmonyb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gebbinqej.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtaesihjw.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gajswwklk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gtlkvuwtg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/guynnxjtm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjmgvuieg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gdyvpncaa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gsxfsxjhp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gxghmwvdj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gblcycyvs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gtefyjfiz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/glbrjkamk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gdvlrojbv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gqmpjpyrr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gacvjbpkf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gketidntu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/glumacvbj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/ghchmrggb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gglcznnno.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/giedzmkjt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gptnfiemn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gxgckqmry.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gjquqwoym.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/grtuplesz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gdipwlrzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gsdyzuvwr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcwqkhbgq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gxhxghama.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/geyzoaxtk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzhxgtjhj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gqdjcqanf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwebtmmqe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gipzkskln.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gssdyunpv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grmgcrqgr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gmrdhbjfu.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyqsrnbfm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqdiqwowm.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/ghdeuydmg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/grefbcsaz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjyahatub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqnxmhfob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsfabbllk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gitgpnsot.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcoyqlzci.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggpqcjgit.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbcdklakq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gpmsxkvng.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/griwvpiim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gbmoumdyp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gerhzxjop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gmyagwnza.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gdhpnpvhi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gsanmxype.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gqghipscu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/glakduztw.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gpvhfsiwk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gkzossdfn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gkqxpugin.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gblynidib.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwoqhdriz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/geacscyur.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gotllxofj.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhreddf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gxihljbpp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/guzvptxin.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goxpziyaf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gftassdzp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gvhergtqq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gstqpryjp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/giaeyehbc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gbtxmavhg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gckuwydxt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gonpunyib.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/glcidhqci.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gegkplliw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkpljmsjq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/geegozsru.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goucfzjec.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gxhtqilqj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsozdpsfd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxqhlimqu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gusrcmiky.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gmbxqktid.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzsdsdrvd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gnbunavwi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtrcxzwhq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gyzzbabmd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gcwuhyjnf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/ghnkiabur.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gguzxpqek.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gibluwqhw.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gckakfpjb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gtphmtxmi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/grmentoaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/glfknftiy.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/grajwyotk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gsjqaofuy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gvtdpgizt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gdqcciwhj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gvdfneaik.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbvydhhkf.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gwvxheqao.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbeomymei.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/ghiyqkbvv.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gznbdfvwg.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/geomqqbsu.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwgdtjvlw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gwviqjthw.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/galondsgz.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gedlzkruz.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gwmnkgamp.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gxhosasmd.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gfzuonfkm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/ghhoexuuf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gfpbyrnke.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggkqjxbzc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gvbnvcmix.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gngfqrtqt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/geqlayjkt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gddkmwdzx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkkjvcpfc.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gustekkts.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gpqcpraza.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gxaxwyrla.sHtML


<!-- 参考信息 -->