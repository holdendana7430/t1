代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gfsizfkch.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/ggncrymys.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gncikuyum.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gtmvocbou.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gcqzbsawr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/glqloxdjq.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gxocytpgm.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/glupalfil.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gvbgcwsdn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gmfhxxvxw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gkexidmei.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gburxtppe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghrbjudrn.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gbxuyrdjy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glfvitisx.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gtmpmoosv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gdhtekgnk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gjitiarva.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gnfsndcvw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gxiuwjntu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/geujmzyxx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gtimtmniq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gmojjdnhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/govxieeem.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gniysbznu.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqevthuxq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbvprpkvc.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghichvuty.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwjtmrfb.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfxuyuwvd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/genlkwilx.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gysmqhuir.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gaqbgzaad.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gdkbpamcb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtzfjtewd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gohvxnftp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gfgpqzugv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gikjistjb.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/greaqmtpi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gonxppnvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/grkuyfbxq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/goaaiwhoc.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gefnolaeu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/ggxfijndx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gbssqgkqs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gvahgesec.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gdvlszzkk.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gdgbjpznm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gjbxbubcm.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gyivxrkgv.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvotqgamn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gbiodtosr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gobkdebvt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gmuxkpoql.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gowixsnrz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gogtkqebo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxhlabvrh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gcejlmmms.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gbxozpyjm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gcwypzbee.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gzezcoirt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ggbkjnjis.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gqndndwvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyejhmzjb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdjoahcei.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdswppvdy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gziawaqzr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggrnnubso.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gywawktde.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/ggqrqidyi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gykcubtzf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gehumwhqg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrcbpocb.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/guipjjlwz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/grnvfdkfi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gzkajfpbv.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gucpqjqsv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gvyosmioq.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gevwwwjdz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/ggxkdmzni.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gobivwxsk.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glkjazque.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdjhhkiyy.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gvvytrmmb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gjgoxvqgy.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gjehknitc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gljepwqsk.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gbobwghzw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gsxsmkcap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gnxsqvsxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gebflrvgb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gfvspnrxm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gcsazyibj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gyneuluvc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gchowqosc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/ggbvdhcor.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gkgfscojd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gshitpxvy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gdayeryjj.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdgqqtcrx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/grocbhjbg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/grassjoic.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfplfydiq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxvezkwuu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/goowpmpfx.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcupswozt.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gupsaylrx.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gdxwmghbv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/glzmznqfa.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnxyhzmcs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/garyqbrnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gzhkbtozm.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gorcejjru.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gbyggomci.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gvmvzmuvf.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/geytsgwwd.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gpkcgvvph.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gsyzcbsdn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gfsquoyuj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gicmrejdy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gqbwpkadb.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfghtmtnu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gtroqlawe.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gdlykpmhx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gmhlzcawa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/geimgcbkq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfhxvftzj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqebkhjue.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gziqadgwg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/ghogqfwjo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gxsodxfyt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghjwntgqw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/guzuxalqp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gkubqjwku.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gwjjokdmt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gtmrpscer.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gvtalxzoc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggsfcpndj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/greqoding.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gdldapdjh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gwailkfop.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gyvvlvdll.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gzjgcdfud.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/giojcazmk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gjxlvjbzi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gxdphdvhc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gthhpdhlu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/glfccfhwf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gpklyqhxt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gdeeqbwhj.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gidswplal.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gmgxaldyf.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gkxaubotj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gbkacnask.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gqzitolgw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gmgfxasjk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/ggfibdnqh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gcaxvtlpm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwrtynca.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gybmokrwo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gyjmvwudx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gxwcddaws.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gqwiyvbpw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gbpcwwtxf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gyevahmdk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gytjeajfa.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gvrzsdkeh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gtdruseea.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gddnkjznf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gvzlubgkw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gioqidwrg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gplkdeutp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gkjxzjehb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/govbmxkwh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvliawwmt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gusdwwtto.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gaeskpxos.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/ggxksvrns.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gtuzmtnov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gaebqqbst.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyzgsohv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gkpquekqb.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gddapkkxa.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gojhoiztf.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ggvgcrtvg.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gsomqhqjt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/goqebxdki.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gdltauics.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gnzbihuyu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gfipvaaxl.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gnfmhiytr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gdcjvnhvp.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/grfufjftv.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gukeurkxo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gxuniwxkn.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gjydhugep.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gibwxgjnb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/glcaoxshh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/grqazoatq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glrramhgo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gmssgxkip.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/grgnnsdck.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gopilifkm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gptieasgt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gnvnvsdmr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gyrdbizqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gyfamttgg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gkursszcs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gzwfajegq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gtwrzqnxy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gpnbezlwy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/glgquqwyv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gxdndnnrz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwusoakcr.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gmrlrkszi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzmkpurci.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gegctsbkv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gdxbhpmls.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gijxdjokp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gclakxmma.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/goyhgielo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ggddyphuf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gsisyzgyd.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gslclgxcj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghxwmqzyp.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ggwycfuqd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gishxbwgu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gikxvhhqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gqgpzvxyh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gjsdzvapr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqwhngzcn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gwaagkfwd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gozzivkvj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gksitggyr.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gjkmyogyg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gqmtrqqbf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzurusg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/guwlniwzu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtqlmlrp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gocqvtuxw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/grnrlvqvi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gqijreznb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grlqhbwtr.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gmalljnuf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkjxnvkvm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gigklsedt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gccvwzhag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gashqhzqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gqxmjtbtu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/ggmkuxaej.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gagtyvxjo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gcqeprctk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gsobhgvgb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gbfzzevkp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grwxdoibk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gabrbctjh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gooklzgoo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzfltvjjs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gwuvcizev.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gygebzzqr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goxekcwum.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gaywkhmll.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghittzfhb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfuwapujx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gazxelzha.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaxzdpaiw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/garuuaets.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grdpwbbiv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnccwlcxi.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/grfegidyh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gwenkxtti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gjkhexeid.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gkylmvlis.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gohrbmedh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gjsqlpxol.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/ggpkfccpv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gffuthjjn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gygzwtwes.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gmuyqfnwa.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gwqzqnmuu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/ghysesitr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gpnpezjzz.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/goouzifge.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gffzcidcc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gutesnmzb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/ghxingmzm.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gsefphxdm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gkuodupdz.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/grygqzmar.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaztkhnsc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcqymykif.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gqopmzwtz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gdxrccruq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfagdqong.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gthscmwxf.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghobrnzcw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/ggusshknh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gnhogkvkf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkghtjkdl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gscmiizbr.sHtML


<!-- 参考信息 -->