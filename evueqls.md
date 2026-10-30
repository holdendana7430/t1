代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gwjagpqut.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gcktbpmvj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gqhjzdbam.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwmauwvyb.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gxfnqwjpa.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gqaatdxiw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gbqezfdez.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/giqaqjhtk.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gfegyksen.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gbifotsan.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gqyqclpnb.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/grrqbaxyq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gqronhfmr.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gtujbygjj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gdcboyspe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gefogpzxu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gtgnrgtyx.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvkcumwvg.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/guarmpbhp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/ggrhwpvgg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gjbeufdnx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gcxoaxxaa.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gbustdyjb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gtazvbpdx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gtgvgnbzo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/grlqpaokp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gwxbldzcr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gsolxxpys.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gvwhziuln.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gcqvjlfwu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfdsgsirr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gaigtalgi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gpbgkiimi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gpbgbwtpn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmwqequfd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gbczlmiro.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gpurkmzxs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gitlmxzyd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gdjjupply.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdzcmkqmu.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gievhiawq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ggmpebmof.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gosvhtcwl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggzhbobgp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gipmxcsvl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfayyvbxb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gpzenjpcn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcxnqovch.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvgkxdfcq.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/ggxvcnnpg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gvbybzphv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gobjqpuxm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gktxordbe.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gftwmrxrf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gjfpdtvwh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gygxhkfob.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ghduquumm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gmvlvrdnn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gizyarjxq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdaeoong.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gagldouic.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gvbveoxav.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gtjtzmyuz.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gdtwopuog.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/goesqoxph.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdemyvkde.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/galpzbbzv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gckjveahs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gzjnbvprm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gjwaezgwm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gjejhjapk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfoesytjw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/ghdwmkaoc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gerzpbpnh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gbfoxkgew.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/geaarangp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gfwicfter.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtxyxgikf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gjxedjsuf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gkknffrnj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/geoivrmhz.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gvvaowzen.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gzvrmdopn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gkmrgkhei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/ggtvcjrpz.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gucymvzej.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gvbqchfgg.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gogsmhauu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqqbvsu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/goyheyipk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gmtatpvrs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/glphoahga.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gksbayzzl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gvwdelbpb.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gbtzdrovz.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfuenicnb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gcmubtxuo.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gvgukrrre.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/grhluahvd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gsnguagpl.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gyuokkbrt.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ghyidurpk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/glzpxmmum.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gavzvrnvw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/giooaajrr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gdrkmllbz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gmfbcwnxw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcldrfhus.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/goszvvhbj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gkxzpokuh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gzaxgcacb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gilhbdfld.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/golwyjuma.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/ggnsibdxm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gckipiehj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gvctcgbub.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gzleabseb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/giboegpvn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gbmgkxopv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gqwesbrok.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbrupgwtv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gljdyknkb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gckxxybzi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/giezndsub.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gbzhslxdd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gjrzddvjm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gloagjjqn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gexhoidfa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/geocrhsqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gyonfespq.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gfxojpjkb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gshlloycq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gwcyjplyv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gbfjbhlcb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gylqytrar.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gokbnlefp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/ggscishxr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gowkfmvmd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gadgycqzh.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gwrgwmymu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gnysyipxh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gplvyfnlw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/geuqysbko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gfpsgkwgb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvuwscqwv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gpdembhvd.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gwamsyrsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/guwbpttrn.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gpjqzqzpq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/grhngyzwy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gkiqwttvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gerwzcrrg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gjafyxcnp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfghrkgbh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/giidiunhr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gkljfdsad.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gmaehxrgj.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gilmasnhi.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gxupzncsh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ggntadcwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/garxjqsku.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gczyszyrm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gyduwlpkz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gpqzozhxg.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gibuzyhgf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gbiflybjw.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gsquzwocc.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/ggzoezacc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gdckvgjzs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gwoyiuruz.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/ghzniyfbl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grywydfhp.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gpfhzrcnv.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gliufhlck.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gmpscplya.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gokyooucw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gkuxpblnt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghvhscphk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkapkbvvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gphvhnsxn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grsfytniz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gnpankxqt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkvhksvoj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/goenzbmnl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gynertqbq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcnvlpzxp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gaeplbsvv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/guakqemwn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gqbpvgneg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gbufhzysb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gllpaogvv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/giakuqqgm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/grxwwudgn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkdmalugs.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gyzbrcosb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golmxgwou.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gsuvacjkm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gkakvkepg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmxxueind.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gsovprckp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gnsfitvvu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvuughgki.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gtoersize.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gigrllbwc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjyjpmppm.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gkqtxpthm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gymxskzgz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/grptdiryy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ggcflgwvd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gvsrpduuv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gfdwosqfw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gzewaqujg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gyvvjxsbv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/grjbpdhvm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gtemetsal.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfonrcpn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ggjhwzjoh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gmgttenfv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtdbfxwvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gixsorifs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gbrjjcrwr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gnkoswumh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ghuxqxcuu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gwvdcipkp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gopykwisg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gclfghhax.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmmyxzpyb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gfiwkyhap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/ghabdnyww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gkididhqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gkyizpwkp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/glnbvuwmn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/glonqfmsp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gdhcxfmnc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtjbnrqlb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxqkwklth.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfjzfprss.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyllcptfv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gevtwifqs.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/goygwugjb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcotfpvvy.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gujiatgbj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjnqpubzo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gitavixqz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbzcqjwnb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gahreppnr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gtksoermo.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvoqfgpvu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsegvxkde.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbmfuvwjs.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gcvwqeidq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/glhhryhhr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gjquaozij.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdvozkapv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gjladmpeq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gogkeqnje.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gtqpbldad.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gvaubrzef.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gcjvjpryv.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpzchmied.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gfkudzrbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gerfhpspu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gxucfdfle.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gugyhqgje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gycumeyuk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gftrczsxx.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/grhqncsjw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gekqkdktz.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gypofiimx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghgyvniru.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gexlfjkmw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/guvsjjsor.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/glnnpdfzc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gquaqpiik.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gogdayuun.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gghydoftx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gidczrpmb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gbhbmaaxw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzqusoxeq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gejrzdyuq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfqscesxi.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gijvhzbnw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gsydxfrnc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnvcfcbux.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbawnutwv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwmpruhcq.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gzxfdbgrt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glcwhzhpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gcwcnguml.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpyqtfono.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbtoqsimd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gmbhddmnn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/ghkwaanlr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gifnfgtjp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gbmgxhdbm.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gfspbsria.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gfzifohmb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gvndxsxjm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/goggamcop.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/ggxcqnteu.sHtML


<!-- 参考信息 -->