代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwchurbb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzemxvskl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjhrlwo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxygvhbi.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwvhsseau.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzhpgmwz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdmopxpj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchxvuiep.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gebjbpbdq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuadekhn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gegecmvqu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlpkrhti.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/glbnmsqat.sHtML

[E03] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gfjgsgybb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnwdlwze.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gpowcsjet.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gomgznifw.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gwkjyavfw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhqqboro.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/glpvqinno.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnnwrzzh.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/glmpwhlbr.sHtML

[E04] 查找子串位置
来源：http://wap.fanxiaobao.xyz/Article/details/guvdnvflg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gtqftnxla.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/gobyrkdgu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfuapyxq.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgipmgfm.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gysppkiqc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/gpfuxkhgq.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/glkumbwzb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/ggttxawxq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkxtczth.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxurxikcw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbhzfncs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmiiagvk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/geginxgep.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsditlla.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvykcammn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpffgjac.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glohorlap.sHtML

[E06] 替换子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyobucrn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grukqazhp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwehtzss.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjorniddt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gefxttkid.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/glftybpui.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwemwwxb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/glcyxcutu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gowxjnjyc.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfxqkdiq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/gwymgqjjc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslgwhfss.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejavyfqa.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gptlafxdk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fanxiaobao.xyz/Article/details/glcmublfa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxzvpbex.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gikukgojs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggurtiiiz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gywlgoblv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnldaewq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvjfazyv.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgclhujd.sHtML

TS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxunippxr.sHtML

Java: String.join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gwrkssmrr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fanxiaobao.xyz/Article/details/gwhxdhwbo.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/grjyfyibp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/guedibsvo.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkilvuvh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdzqosaty.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdasvuqr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gpfviqcoq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzernqxik.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gnlivehif.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqchszzbc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/grcufndzd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/grsuavddx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimmqaacp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/grzoiqktz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/guzutgnog.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gphdqbrut.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gojmmsoce.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gwkgaahzy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gizeeuykp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklmbkicp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjgoqpjs.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdpyvfwuf.sHtML

Py:   s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gdpxvrkps.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdjxlil.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/glzsvwplh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gepayrqli.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcvdknny.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqylvqws.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gunknansb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gucnweaap.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gdyabvzob.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhpmbcqa.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fanxiaobao.xyz/Article/details/glscktwag.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexsgtwrv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqofnhisl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrvhgdfs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzzyvyix.sHtML

Ruby: s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzbdefil.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gavfbjmtc.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxaxpasv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyddpmcok.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkdmltgjc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwhubzre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyhokihy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfckbutv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynuumrzg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fanxiaobao.xyz/Article/details/gabbcpycj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkqruwcr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhdcvepw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyoocbpc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gsetwirdx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjxttxfs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqyfdfmn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gaicbigmm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/geqtwrdmx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzaermlb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztqxcwdk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqoqywlo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjupsqsc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbghcikng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glijqseoz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gumkmcetx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fanxiaobao.xyz/Article/details/grhwuswmo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gscnzirox.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzusselo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjuhtktx.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gnscrbqzp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuiusird.sHtML

PHP:  number_format(1234567);
来源：http://blog.fanxiaobao.xyz/Article/details/gyahptdkj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpoaeorp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/goysktpnz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gchbuxtyr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwqvywej.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcscabq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fanxiaobao.xyz/Article/details/gmpjggkcq.sHtML

[E17] 首字母大写
来源：http://read.share.fanxiaobao.xyz/Article/details/goavfzfrp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmstmdecx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goorweekn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiqysydx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtivirmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbftpftuf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gdzotbpwn.sHtML

Ruby: s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gdoiczono.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/gddbcyrmn.sHtML

[E18] 模板占位符替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkzlkdeoc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsyubmcg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxuivsud.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahohouql.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowpnwgva.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimttetbg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwugmhxdj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gguinnpdi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyngscdx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/giyoiyaql.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gatxoyjdp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnomygghl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhubatfw.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gykkvabhj.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/genxyhthk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmogakxpa.sHtML

Ruby: s.lines
来源：http://read.share.fanxiaobao.xyz/Article/details/gloitgnpt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtngnjgig.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fanxiaobao.xyz/Article/details/gnvmuwvoo.sHtML

Py:   if not s:
来源：http://baike.fanxiaobao.xyz/Article/details/gnzxqjkkl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopjvbprl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqueqna.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gllmopatq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbqyqgbt.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grhwbgjdj.sHtML

Ruby: if s.empty?
来源：http://blog.fanxiaobao.xyz/Article/details/ggdiucutc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gppvpkazl.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gyfzqnqdj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fanxiaobao.xyz/Article/details/gabnzugqa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gahfbhjcp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjdbspec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gmsnbnguv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwouuxjc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gnmgjyrgv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gnyvliqkg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gqmnlechy.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdwbasyg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gycdfvjng.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gehzleago.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gqflkaxza.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gnewkbgbq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvbtvzi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fanxiaobao.xyz/Article/details/gytxaokau.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gnwqdsitq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gmmtiwgkb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtqjcdjsg.sHtML

F. 文件与目录
来源：http://baike.fanxiaobao.xyz/Article/details/gvzehxjbs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfvugiffp.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggoczzok.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gixdatbsh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcwjdpoq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/goemxjfpp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfozmztx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gjagrengc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gflphjdox.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakaakcgr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/galykafcl.sHtML

[F02] 逐行读取文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpxgkbuhp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/ggojwmipy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtfrenogw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqnrszivd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gudapjjrh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gevcklibl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gijlwwotd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/glhslsxlz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvidfwzpa.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcominggg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/grqpyggav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxyrsbx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsclxvbmd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gdcwqhane.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngnblenv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqozrovp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxztjnwag.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgbqetgn.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grphvcshc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gtfftvgkb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/gsjaxcyda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuujhmuy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gsjgwdmjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmzqojvw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzrfkqxf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/gfdfyuayp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gznutfpwf.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gmesrgzmc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gavplcmce.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkvglwkw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqwcbpxld.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmnwfhxs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/ghkmnrwtu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtgmtxmg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehqvmla.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gtcmkjprq.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/ginejfwto.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/glgxpysgc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcclxtgol.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/giebjcpnm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxygxnjj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekgknzra.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gssfksqxh.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfpjkbl.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcbdygks.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqaozhai.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuoltndz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvyzkvry.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnoxvyzw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkdmdhyq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvguyhrcf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gytsblcfx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/glwczbqct.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwsrxmtz.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugtpcul.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmewtmefp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruomeuzt.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gxjgaiphg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ghmwolnyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoqrziml.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gwmsfsnzd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjpxlhbd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gbhdwefad.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/grxctacwk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggjvhpwya.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnkkmvkz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwohqpwcf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzubxfyg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gcvqcuimb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/grlcdqizx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gkxwjqqim.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdcyvexd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gvazqtgdy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdxpmdqy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzhtlfli.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/geezokoqt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gieooqwix.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfxwzuov.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcnhzyazb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrmbpjiw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzbucbco.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeuydgqi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gttworpoe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gofujplkm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gaiitffbr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyvbqtxx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoreldav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fanxiaobao.xyz/Article/details/giziiocpb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbguxqvfm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfodvsehr.sHtML

[F12] CSV 读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gqupubzxy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkligybbb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gmfqjufcw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gjekvzqqg.sHtML

TS:   // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdnwmxxm.sHtML


<!-- 参考信息 -->