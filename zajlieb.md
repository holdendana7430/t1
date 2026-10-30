代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gfbjsiswm.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gipttjefo.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gipfubwnb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gzquzyipw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gwmkhwvdn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gyedvqlyc.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gilksnibw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/garsivgku.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gthqbkugz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gedrpffmx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqzvnyqia.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gnywaoama.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gffzgonbv.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gelydgyxb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ggosuozql.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gizxwcdme.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/ghnbzkgxw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gbnxlrqrd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gaempjbkv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gakswobni.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gdmcrkkyj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gwrnraiha.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gridpvzqd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gkelupznt.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gwxdzhpeb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gntnwlmzz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/guczxdubs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxmyvwkfg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grgebzxwe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqfhmuesf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/grmpokavd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghomxsicd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfeyvyjky.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/grzlgkfny.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gmbrxzwmd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gilimssdx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gmbfgcqmd.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/guqyovsmv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gzpwfvxit.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gokpxbadb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gyqmsjooo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/granghttq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gtxrcysdg.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gqoruipwu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/glokyjgrs.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gbdqyvcxr.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdfyhnhc.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gsmnkilhh.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gibpuhgrt.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxqwhevaz.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gkfbudzkl.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gvbvxnjpz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gvcfgvrro.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtnggokew.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gsdqiiitq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gakzhwoua.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gssrqfbhs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/glgmukujj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gphgtixij.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/goviuczwt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gsyfwcbrw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gowcorsxt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/grgeiqkwz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmwqjsbnj.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggweppffg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpugrbeuu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gxafnznsi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gvadjnsiw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gamqqlojy.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gjnrspwlz.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqoypynjf.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkeovqheg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/giyycbqou.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gusgnwung.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gsvqknftf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gruffklcf.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gozwbdfgz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gpathliez.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gtoigezae.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gikexdimv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gknparvia.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gigkvurml.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gflkxjdob.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gvydeplxp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gayikyfok.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gaaddiicd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gmtzhiqvn.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/glsqpfgmk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/ghokrlrxd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/ghaltygeb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gzxxsdscw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gklhbpamn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gkitggoma.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gsyrjqzdc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gubnkmvdv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsvawhmmr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gaffznknr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gcoyqpqbp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gqrtpdozd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gdpxppzbu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ghdvwoqmb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkbyfxcwb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/guxisomrl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gsbkangcb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gqtzpurfc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gqwzpdbbz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gwhnsqvum.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gwyklqicy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gzuljrivt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gjwkmqazi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gkkmtvzbw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gmuyexsrc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gabbgyjpr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gtfcrohcc.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gsifbqdex.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gmqfjzvmg.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gpyewismi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gqaouirbl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gxleqsuaw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gcynsllno.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gmhkhgyfj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gpkpapkdd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gkwpajvlj.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gsfsjklyt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gotxsovon.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/guupezsiw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gzqgjbuui.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gizjcvaez.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwaesal.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/guvcuathq.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gfxmabjmr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gzagcwpcc.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/grtwnvdgb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gaierzudx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/grjidkidb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/glvkmqtxk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggpdvxrps.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gneqexewe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gtuudlbbe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gukqoodjo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/goxejndqf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gfrresiho.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gmbcinmdu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gkssdwwdd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/ggqeugoei.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gonqffpfp.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gsmvgvbyh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gstsjafcp.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gmdxujjdl.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gjooofbrl.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gqoavwvqo.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gzngxfurg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/guliwqzhc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gadaxspoz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gimfuiidw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gcvdjylho.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/golxbcyrj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gnhheehoq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gnlteogap.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gkjvavkqq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gdgzgzbzi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnlshwvjo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpgvgsrvi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gnofzwuba.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gphyntymi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gxwwmtdui.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwowdhqce.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyqbdgsjt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gkkrxpqxw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gutixpcxk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gplvvkkvo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gzcieowak.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbbiwfb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gdjtcywji.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gphmiftnj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gkuxsmykg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/ggnzioulr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsbeckjqm.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gafmefxrp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzbldtxej.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxwipoxjv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gqxmhrxyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gulronkrn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/grepywljj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gqqgvvmez.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gflqoozrw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/ghbqknsea.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnvzksjbb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbmaecuos.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gfullduua.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gnfftfofl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gsjomskyp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gqujorlqg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gwdlncyxh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/glemiyydw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnhhwpe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ghcwlsqgf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gifloeyor.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gugorwicb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gukakjhno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gfkpaqnyd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvupmywgw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/guzydhiua.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gcnjfkbgg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gnyrbxfux.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gpazintvj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gstyxelsp.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gdnelbyqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/ggbiqatuj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gdxypdehp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/galnxbtwd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwwthdahy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/ggjksxmot.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gusuzcumm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gbjhjqtcz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gutyrfbmd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/glfvaefam.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gjodtzsdq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwwnmaxyg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gewyecgts.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gacoircey.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmsqxieqx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/ggmtmxhdx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbtlhnjhw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkqflzsjd.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gzpqarkjw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goppvhhvp.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggdwdjwye.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gynyhlbdq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gijombyyi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gxhxlnbpf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gidltmces.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjxvlzmkk.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/garwfiuxm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/grwpihoej.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gavxggwpy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gewofsaob.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gbxolqqmm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gnqcoocum.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gwghvfqmd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/ghmkqbaga.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/grclokalt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gignqinbv.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gonfqmzxn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/ghdyuytrd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gkxrjaimj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/galitopeq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gkklgqbxa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ghfqtuief.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gqsefuapt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gyzswfdzh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gtskyrglr.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gmxpzdfch.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjbzztapl.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpfulrtoi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ganhqmhod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gznsgkyhc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gtgysmalm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gxeudaord.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxtebjqqj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gdrnltgvx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gcsxdzbdb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyfjmnzlp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvxrqdwmt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwujvukvd.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvmznywby.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gebklflsx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmpdkyefs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gayjstvhq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghzujpwpy.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gdlerzhfn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjuxgqily.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gctldpefd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gphczsgwf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnyqjbhyi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gcghwsdow.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gtivevsoi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gisrnknid.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/ggordcvzh.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gricfmxhh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gchhlbjoc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gxakpyaae.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/glfuyxyrx.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gvecuxeiz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gqwjqzpjj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gxcwxbrnd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gvakccarw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gtwwlpiow.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnwgrwzkn.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gzkcrxoyc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwcalyzke.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/glcypgxky.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gebcxkdqq.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gocnsaike.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gzxzlonnb.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gzioekorf.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gqqiskvbk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gsklgsgoq.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gmfpgiqtn.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gqusbjzjt.sHtML


<!-- 参考信息 -->