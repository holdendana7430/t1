代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/goanlpbyw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gjkdqdjhx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gdmqtvstw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gfrxtumww.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/grvpbcrav.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gambsijlz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gfthbxcsj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdtynstea.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gdodpxmlp.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gakhfwufa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gcuminium.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gaaofecgt.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gymnqajzy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gmmbrqhau.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/grxeyzmbs.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/guiotgljo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gzlwjjbev.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsycurbel.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gtsvoiccv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtryidgwi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gowrvtntv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gshtyvixl.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gjxrffyqn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gkokrgkhy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gggtfgfpd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gsboshktc.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gzfnmufva.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gocjmvelj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gqqqkasqx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gkuytlldg.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmtxsffjb.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkdzrrmlh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gntkrrczo.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gdebdypkf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gxtroqpen.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gxvetyxeq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gmbwdsxyx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gmwhhscpp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gmtlsroic.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gsmxpwovk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gubvilpoa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gsiycufyf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gudvmkaeu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gsuypkoyp.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/goxtupuwa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/guavgtaei.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gwvfhlbeq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnnidmoms.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grjonwgsl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/getbnynep.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gldvpywps.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/girpncchu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guspwbpvj.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gjkvwtvbm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gzxvqwikq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnmpdxhrg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gwucgjfse.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gklqdxorq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gbdbwpzxs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gwnjuujsf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gmmcvfrfq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gkuhqcfyh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gisyrmkdg.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gowljwuhj.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/geufjpfcf.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnzdazgwa.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/grlhzfoej.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ghkwntqdf.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gyncifqtf.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtljmxsfk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gmhgraquj.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gimzzfimj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gxehfsdjn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gezsvilnc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gokbmlruf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gruslxhwi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gplmuftkl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/glnyhmcfh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gntzlwxst.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gygiqynso.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gtsvywktj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gedaujuaq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gedzodrpp.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghplyzlzy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxswpie.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gkjeqyxoe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gkovrqhwz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtdirsusk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gblzrhilx.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gkcjwmeoo.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gsznxuimi.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gcuudmhvv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gcrbpqurk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/guiqettoc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gyyawubid.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gydaiokvg.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gnefbdvey.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ghlrjbxrf.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/galkjifpa.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gxsgwojtg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gftclponz.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gdlrfmwzw.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gxyodpudc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gjljmnolc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/guxuldqap.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gysdzukhw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gahmaxruj.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/ghugqjcis.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gekqvcgkd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gxherspxz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gelrhgvqi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gymxjmssn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gwnvcrqdw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gwotvniut.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gtqcifwsu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqpwovowb.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gaxuomxiv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gilpzptku.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/guckohnes.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/ggzmbfsbz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/ganavfezo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ggtvssmgd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gouojlnmm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gpsgmsune.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpchfvykm.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gbksvxnvi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/geckqenmn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grxvvdyik.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gtpczmxww.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gkydmtakg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/glqidpaen.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmjjzjzn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gadophrzd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gtbhtmhei.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/giqhsaees.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gjncxaogd.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gekavalac.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gokgltmdd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gjpzhsbwp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/grfdajyjw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gwsmrefez.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gwgrnluhp.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gsmcfbiyv.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gghtezzmm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gkkvvykzl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjvwkdkaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gumpiwdwi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gpbkxgkju.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gwskvsjni.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/ghkiacbxn.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/grqhzacyv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gmfigimfg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gcrrdvjim.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gkjmvfelo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gtydczwhi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gtfpzndrg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvwexatxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gstazrlfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gaasoiovy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/ggqyshsvu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gpgqqyxim.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gmihucqrj.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/giipwqjki.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glxsqxydy.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gzueantyl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gppuvggvu.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gphsyjcpr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gxiglljyp.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gizrgphyi.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gpsspuezz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/ghibtdkol.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gjhijqceo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gmuiswbqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/glycehhbe.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/genrcxaew.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/goxdmwxle.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gnfcrnxmg.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gatminzct.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gebueribq.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gclynaiai.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gxqttaksa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gsyzymbrt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gchmrdmpf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gckjifhbj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghmpxxxnd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gnquaykhh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjhefugjm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gtecxcbzv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gowxhvdfs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gifxtxzwb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gngqzbodz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gnlnmaoci.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gzlihuemi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gsnsmfdcz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gsekezisy.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gehbdkwoa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/ggkiatwmf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwjkxlusf.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gvnlhkwsq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaaynecrg.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gpfginecr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gjfntqvrv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gevjaqpmc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gzjokwlax.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxvfqohjq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gnhyymupj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gohegiset.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gghymmuhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzwrefoeb.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gbxarwear.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/grksatecv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/glgkwykpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/ggolgjbnk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gtbqcavgk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpssbpso.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gwajkeilj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gazblbzth.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gosouvydf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gtyvaioft.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gctofctce.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gwfwqmlhn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gsuhfiwfw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gumxwffnv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gfoybwxiu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gvutoqbgv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/graihfrsw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gucgodcwy.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gxftlcyok.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gnqtvimbp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gqeqwaimv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gumynybwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gesmskhgd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gdftqxtvs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gzgapaxaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gmyqerymw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gfuqlfull.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gjbxyzogo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gztayormf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghbpqtxju.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpmqzvnew.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grqgbfpox.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkoizwtsq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gsyyuqfhj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcaikqvci.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdxezywll.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gywmsrigx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjeefubxk.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grdybfqrq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqpehtgst.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmoiywwee.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ghegwdsgq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gocvrpdvc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gewknbihp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpheqlnow.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gpitdkneu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gvmqxyuul.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gjxrtvlyw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gpguhbgcp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/goavyupyp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gsmbuwgux.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gwtkhfdml.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gwvsqeyco.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/ghoawlkxm.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gqwqwwvxw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gsggpxjhe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gxjdqktnt.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gtqdhucda.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbsvweqt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gapznohyn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gvnasstlp.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gadwqzcpb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/glzyodtwg.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gwfyloihl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyjwkvrpn.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxxmwntwx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/giooghtta.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gvhiwmzjf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gybkqkwda.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gfoxqiodv.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfifqsamc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gluqurkie.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gxywmcavm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvikyapor.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gghfbifzk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkndqplot.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnuqhduqi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gdzpdscao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcoekgmcj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gocdrhtdg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtlnrchpr.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gabfaysvl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gsvvngfih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gnbwygvyo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghsjswhmc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gykjofvfe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnztoqaku.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/glurjbjkr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/grunscmxq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gsernwyqj.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gdxwbbkku.sHtML


<!-- 参考信息 -->