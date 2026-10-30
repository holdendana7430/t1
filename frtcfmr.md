代发 wailian999

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzjcryuq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gjprkkfop.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/glqnvrmai.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjkwjvjb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdzimhol.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gylxlderk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqqtrywn.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsglxzb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/ggxlryhxs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowoikcfk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gozfssufv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gtoqcyilv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswbocbwv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/grxratgpd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/glgyplqdz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxzbloqr.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrleezei.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrxgqkrr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhddpiy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gktredqyw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwhlnyhg.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/grnmwcigz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzechgvm.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gcrrwyfuy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gvfsngfmk.sHtML

[E03] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqkwzww.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmnwmjo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/ghyqenxfi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gdtdjkigw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxpumpvr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxyqsteb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlebhbgt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fanxiaobao.xyz/Article/details/gvkrhcsnm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fanxiaobao.xyz/Article/details/ggyfuzyzv.sHtML

[E04] 查找子串位置
来源：http://baike.fanxiaobao.xyz/Article/details/gfshzwdyi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsagkazo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgjfwzql.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkienxao.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmzmfqbu.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/grelxmmcy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fanxiaobao.xyz/Article/details/gawelcqkx.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijtyomks.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gcbozauhn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobzvtawk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grppatvde.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/gjutkuwnz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyrsbayh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/grkinikfu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoolynwr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gebukikkq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwlpubqc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhcgqsem.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiatcgej.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmvhfbzh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdvpmvgsk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gbktuwfms.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewfteqhb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gznmssmzj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gypobicsd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gnxdpjjbt.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gwmkgoqhe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvgilmjj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/guddhtmvk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/goakablnv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqquqxze.sHtML

TS:   s.split(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gpnbianxk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjjasjzv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbiztqee.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfqdptzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgexsmkb.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtviccjsp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqczcmco.sHtML

PHP:  implode(",", $items);
来源：http://blog.fanxiaobao.xyz/Article/details/ghgxfmijh.sHtML

JS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goapzbdry.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gvpkxlbho.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gqldydzlt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/ghxvuaput.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gqppdbmgf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnytmhdvo.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpamwlah.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwesufidf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gdhdeyavs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gnssissus.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicljxybl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gotctmcfw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlegwbpx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fanxiaobao.xyz/Article/details/goszgblke.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcinqemys.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gggidtncv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxuzbaia.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxkfxcf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/ghyrpxydb.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjqfsymj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrljqxyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgefdbxi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/guzpdbsdz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcvuwgup.sHtML

[E11] 反转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gcbxtsdld.sHtML

Py:   s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gckomoitj.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gfzxdhlwc.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gxtotrpqp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvjtnxds.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkewvfsu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoiovlju.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/glmbuavhc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcinegbzk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstgagnnw.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjhhwzpd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrmembio.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghruoguuz.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gcmtctlvb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/glpblogxu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fanxiaobao.xyz/Article/details/gbxhskcvo.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcjfhqxv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsmjpnxl.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqfoczgi.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkfaiohd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghiatzjeg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvlrvzbg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfgkclc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glloonrje.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfopbvsru.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fanxiaobao.xyz/Article/details/gghwkhibj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkatnomc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/gqjxbhfwf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizxvjrlg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/grxhhkhbc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxpwdcfu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvelnizoi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcchnieqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fanxiaobao.xyz/Article/details/gejxqkvgf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gowycptlf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphowbynr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fanxiaobao.xyz/Article/details/gyysoyzxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grezkskwm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gdmcasyib.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwcrhmbtm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gdplbgsob.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fanxiaobao.xyz/Article/details/gzghzbhih.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbefsvmxz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwehmwmw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyywdwoct.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/goktweyon.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmucezar.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyxxfwwh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoflqcid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxlwtjrp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gimfavznb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/gctihievb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fanxiaobao.xyz/Article/details/goyqracst.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gndvbbcvk.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwhmvheu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/goylccyee.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmghbkfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjdearha.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtlunzgxk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhsbexsp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gxxfgggul.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gogdfpwhy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gthftkjkx.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/getexgidn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzudzhxiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gcerjmlfr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuputjod.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxtmtsba.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxltedifi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gytetkrqa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbnutwxpu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gouirvtof.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gkoogncbr.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/gmhxditkm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmlhhzcf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfaghoyn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlcglren.sHtML

Java: s.lines().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjglojde.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdipabcqg.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/getyllsti.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagisfsul.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtnduar.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnyuauth.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsijyqfi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsopgaygr.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmebdfnk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnpmirryn.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkkwvzuf.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjwrwpq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goxsbjyrn.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gogsegeuy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbwfpuwb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/giucfycpj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gynfowzwe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoqhzdsg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmohkfok.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gnwelbbrw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gomveufzr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaagwlcs.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gsexhangg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrfmdsbs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrtwejew.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/guopkglrm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowjyapbr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gklvdafig.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqnpbluz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gbowycfgd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrnnzogt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjsjyhm.sHtML

F. 文件与目录
来源：http://baike.fanxiaobao.xyz/Article/details/gcellbmbt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkeknnuu.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/givztosqi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fanxiaobao.xyz/Article/details/glytssczs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwqnhneo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gsypdiojd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkzibpxd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gjrjyasbc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/grrzqvxuv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrlbntk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gghyjmpuj.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gozojtkjv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpzysjfc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijmivym.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtpjbvkz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghrcnqmhb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gtrdnkqtk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxgsfpgz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtjebjjd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrktsjuq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gugwphxel.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxytphko.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gereaepzl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gryzwcxlz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevaxwiwx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcaednya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/gvsgrigzk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/grspledko.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhwqnqda.sHtML

[F04] 追加写入文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnimefwff.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjwecfrm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/geyvwthjo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfczqhlda.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsrijkzx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqdnhicv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/girykpxwh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnuohiqw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gawubxboc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoaozygz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiuwmmdt.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/guwlmovhr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gzchbdrbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeopvmhp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gbmpvflwd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkjlvgfq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/glzhifqdr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfmifguqq.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/grddovmcy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/girkhacew.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gansfluho.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozcizyct.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwrnbmti.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzvxsqzo.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/govbvpigc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gordvdkhy.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjkwqqsy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfiasjnt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghihnrpan.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/goscwyniq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gklavohxi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmvvysot.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/glcoqpanx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gvqctbone.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkutgmyo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gucegrutr.sHtML

[F08] 遍历目录
来源：http://wap.fanxiaobao.xyz/Article/details/gyftgkwed.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/geobgezth.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnahxltaa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzghfxzgd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkysarhi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmpidsfg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gttenvfev.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtlcnuyi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gikwjtjds.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtldsvfxh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfvipom.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gqxuoskro.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gggildbxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqormky.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gpiyuuahm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjehwmrg.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnyoygvkv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fanxiaobao.xyz/Article/details/gwvltbuks.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gtydbdkkc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gqkfozfxl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gjgnznerl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnrzddoiu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqtjrtbk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcecswo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayyrpadj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gijugbczn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggsrvzcaq.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwvicwayp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmtweqjn.sHtML


<!-- 参考信息 -->