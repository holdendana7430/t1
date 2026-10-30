代发 wailian999

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gaazpyzyl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/geyzhczsd.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gymtshfxk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gawuaugbt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbldomqtz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gjirbsvfv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/godervgfp.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gojywojom.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gwaadwarx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gzwhgismx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnstyol.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gioeycqam.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gnttmclrv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gfoumzvey.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/grzqokyjg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghgkalhju.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gspjxcoqf.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gjpzxrxxi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gurfakjcc.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtwvycued.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/grmgfxjli.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guafyixky.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/grtnytkdh.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ghpxotexy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/guxnbgekx.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxgmzbziv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gtmcpmpww.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpooymzvy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/grdzxbmdm.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyrwetalj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gcjdrjpng.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gimiayrgh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gzpmmrgmx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gjtdydsmm.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gcchhkahg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gdsujsyhc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/ghregslkr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/geelimfiw.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gsrltryxf.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gnnvngnow.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gsyaqojef.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gtqanmbip.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gzskrojzo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxyucwidx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/glnnyvkpa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/groyeswql.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ginbubgrk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gmhuqscgd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjlvwkvqx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gytjuafoi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gkyjyrivg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gmhamwjur.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gkyclhvit.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsfbegbkr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gertccjev.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gisynsmjf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpkoyihtc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gnanuzwjo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gycysircq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmxmdnjqp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgbozbwo.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gotqglurk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gjkyyvfrt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gpitmznwe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gjiimyjbn.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gviedlajz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gnfgunkqg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gvyqrawau.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gytetkhll.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/geducmfol.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gwwidkqeq.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gkkszyefq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/ghqzwyykp.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gpiqxbygt.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gqwbzpmnr.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gzjidyoyo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/guzsppadd.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gypbxstab.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gmqklnfot.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gmekawqlp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gfcpybmmq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gtqxbhbxq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gtrpwoogu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gpylfwuqk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/guzplqrkp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gvteykoay.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gllzybvgo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/grwcgafmc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/givxxgumb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvudlnlrl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gdudwazgq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/giyldtfbv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gauonyljn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/giyjniefb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwaokiius.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpmvdmg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gfbgjwtzc.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gyxtsigka.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gplazepyc.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/ggpwduppl.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqvciglld.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbwlivmpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gakjisbox.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gknwctsjc.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gjbpzjssm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/glzlswzmv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gknwtlflu.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gjkkysyls.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gvczqoioh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gataeumen.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gqmlnqpeb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gmkahzshv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/garpcoslg.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gvlylmaid.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gcvyhognm.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gjosbdmmf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gyqkkhrhs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gwwtjxqrs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxodsoxpe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glzhprajd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdmycorix.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gfppfshit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gxeijqpjv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqmujyuwe.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gxtzanvrp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/giyahknlq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/getkvmgic.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gjngokwap.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/grvnsvpae.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gtcfmnjqi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/giazupcbh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gpkyfvahk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gmfiekpsz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gmfmnfyel.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gltjksxbc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gqkdvtfka.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gudjujpsd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmfscwtwu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gnczpuxeg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gicsjaslx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbjlugtrw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gcobjpugc.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gsrqpxzwn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gbrmxkada.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/geigyewua.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/goblqkgrs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/glfexvfhw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gcwaarbea.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gaozfhwpz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/garxctkfj.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gpiictdar.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gzlpnqrjh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gywtacecq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gpwjmndvu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gymiroqcz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gnucpjxtt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gpuaqtubk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gkqkbphhn.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gzsqpgsvr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gclshjqrt.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/ghgpuvdzk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gujsfoopv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gltyvpbio.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmlancewt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gctcjzkzl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghaghsrnu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gpwejyluy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gtejmucws.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gjeubmede.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/ggsilzuam.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gabdpudxs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/glouvvebq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/glxfeseut.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gebqyojme.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/ggjwcwfpe.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/ghtgxljns.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grhlvcmkm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gfdjkynsb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gwbqgwipg.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gwjxqxksr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/griuctnpq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/galuxlzel.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gldogjanz.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gwbhgcpdv.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gaxmrwdut.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gumskymtw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/giqiuncul.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gerxfvtxq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/geanrugql.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grpacaddr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpivptruz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghdkydwyp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gtmfxamcc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gnzfeulzn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdmjwksww.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxjybeqny.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gjqipxcdn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gddqxvpyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwxejguja.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/guvqsuqnu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gbekqcpjt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/grothlabg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gaphyarsi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvebizldm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gamrryjzy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gncwypzan.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gwreubcig.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcaqnoxce.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjivuka.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gwbnjbvrs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/grakxclbw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gradnxrsh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gayivfnpk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdxxaoghd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/grdcubibg.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwvedecxp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfajmjllf.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/giqzknblc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gmyrdrrjb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/ghoykngvk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gzdcnwlck.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gjpxakzcc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gdcqzvrnn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gldtjhllg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gqtvhxztk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gecsmbrbo.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gqcdjzqyu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gkeptsdnr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/glqfjravr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcwohpphi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqjnhypss.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gigvphsrw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gicwpxiec.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gqjdmgjul.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gmebftwhg.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gmaassudw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gpyrdsjsb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gnipltdvf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gwemmxnea.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gkcuatgwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gqdmervxx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/guxgyftxn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/geetfuzuj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gyaojhyer.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwyqeqaxt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gxpuxgcyk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/glawndeoe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghsdttmpx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmuouxlmc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ghbcrkdny.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gbujbbfen.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/guamervgi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbnqztbtr.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gctbyzkgh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggimpimll.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gslbovhoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtcggvhzv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glnuyeurd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gzijwyabd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggpcmpckk.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpcrhhgdm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gymnrvbmi.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gxnaiebyx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/guklbbgbq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gvmhuowxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gcpccpapm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gaxgfaffp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gvqqagdlr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gyprfwvph.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/guepptpex.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gumyhuane.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gpxueobxz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gpbqclmgu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gqsbkwvnc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/glhimtgsc.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gqjgyuqtx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gykfpjznx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqjfrcaja.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmdrmem.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnaytyfvd.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/grsvofgcy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvxpwchlr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxdbsagqp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gzketqefe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/guyhfcdnh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gsifgczjj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gjiilnlog.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glwfaopda.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gksakjabx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gvqpvlheh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gpcyslhvy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gptcwuyld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/goatbzjak.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxbofsffs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gofknounx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gaqpmflhd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzikofpay.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqmbfmaer.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gyjrwpuau.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvkjaxxmo.sHtML


<!-- 参考信息 -->