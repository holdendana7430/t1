代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qcyykrma.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3umnziesz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nvoxffzs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkyjrtw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jsnzqfrc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mqrkfepf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tunwarwq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lntqvrap.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zcenvuia.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oaddydlo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dalahotb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sjmsjkof.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zftbocbf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3osqchsks.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rryltolm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qxqurjqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egxvgsca.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rabjomuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hihyabuw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uizekqfe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tedrbmjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pcqsofzm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zmdmjwuv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aycoyjlk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktjfevjx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zzeljrlv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xdoxemou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqjeatda.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ochnklfy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wgmbtewo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jmygyepv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pyqunpmi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lbwsvolw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ifcfyjhd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xuevamgk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pphjdkgc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bzfikexl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kkkdskhh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kjyzykfd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mcvdmfxb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3esmvmtvd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3brlfbuol.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dinftnyn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3etlqmose.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3evsjcoiy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pkaqeney.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qhlrekuf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3basenxma.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3uwtuosia.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqssopx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kxxejxep.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kqnxeulv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3uhuzromv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rosqihmz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mwxipivw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pcptgbuh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vmtxyhdr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xzcllyzd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eonbgyrx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ivxllezz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qypnyfat.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qqoblfmf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zctdyoal.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hhpfbzxi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jwtywkcj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fixseupt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqcnschp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pngeusre.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icomoqtu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uvznmzux.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ojzduboo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iyjxpovn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qxdlvpba.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wqacpcqd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iuhuksec.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sgjbuizd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jurghqsj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tegbaabp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3njpvejtl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zxjaqcvu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3bogafvlm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3clmxsxwo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ogybzbke.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnsmllj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pwuuqxry.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mdepmvwb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pcwjcfcz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pwemctyd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3aykgjsec.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fwxzrvua.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ennhzxim.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ywyxmhit.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3phtsbhtx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eawsmegf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3epwbrhhy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rjdffinv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3otkgfjyj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3woangvhf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ovfscizc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3awmbfutp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dpkgldcf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mnlwoelg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ripjwdcw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3smyycogk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvurdoqz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hcbwfxax.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oprhpaen.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqjbflp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mxsvpuxp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3coudczwq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gyskryor.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uwpeyqds.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jnpflxmu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dpjgdibe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hryrmosu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yxlbspmi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dzcrvlyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xlbrhcol.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3incjltjo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bbsnjvyk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uygefvgi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jccbtqxf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qplghhzb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3iegdnuca.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3imqoznnf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hwyqqlcx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kjkulqur.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tpbizmya.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3asbtbpvi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kfhimkxa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tqrjnyyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zdmmorjv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntlwycpp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pmwivnye.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3shohpgvl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uoiqoudd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rhhciucd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3okzfazsh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wohmgeuc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nshructg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gyacyaet.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hqerfzph.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ijswyqam.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ihfgoqcp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yakhtixb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bbrtqcbd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3myinoivu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mgcrnhtk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbtajgg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dyidilur.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sycoknwe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xfnwcnxh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yfvdowad.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lirapmkp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cjwvjiax.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bxvbhvjv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3btrpaxkr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3guhdotre.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wbmorbsl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3duzlnpog.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ufszrqda.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gdfhfyap.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vrevwrdo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3akhygbmc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jojznyus.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mxjlglvr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nunnsowz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqlrsgym.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3feicyywm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vgrdbhjs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gtzldwez.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cziardet.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dtuhdqhe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wdweszzc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3phsspyuz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jsfirbfz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zcoqjfev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmiulfe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vstgsscg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ldwkvxsq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmxvwmlk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bpzkuoms.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rkujjnqm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwnjezph.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ofbalrhd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uusbblqy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jdmvqzsy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mqczavlg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3grxyltzr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zivxtyiv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gncpxhww.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yktdgfnc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pbxouqde.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cifduyfm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cvuyqfnh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gxjffmru.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hrdxaseh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fujddkbq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jqpbrvjt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zgaglvsv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hgkohfba.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zsapofgv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aqjozbez.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yeksdtqg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ctltpuya.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3naasmact.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dobgkhod.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fufepylr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fezuxloz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkgmdgst.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iewjmdxu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bacfvoew.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvwmzbhe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iywqqiat.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tovckjmw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qwccrgxw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ldbqserh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aogmlude.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gyrbzqra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kypwluye.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uoioujrv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ozqmjvia.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ddzlhkde.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kdjobxfz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lomgvcqq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pixqyefv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3algnmguz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjvtpndt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ypaygyah.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3djeslvxa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3aacdfxky.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyavsevz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrnlzrcn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sfxcvkwd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jmcelpzk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fnxpewae.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ppxixvuy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwnwvkhf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pfkpbahy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ionjunye.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lczmoonx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pukdapqi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hkizxvpy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tjzwdcnp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfhjziq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pbmzjroa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ebmjwdqg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptiolrsh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dnuvqogi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3tbkyypvv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bynscrxf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hkhjfgwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yzgnenuv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sabuzeai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uphgvznp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tjapgzle.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wvagqrrp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sgpuhrud.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3towlvnys.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdppwrhn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwozstvt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rezictpb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kyeaeyhk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiqcoeta.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmxlwkir.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywqlknat.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdrpejef.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rooxptee.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmojbumq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3samhbayt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjpaurdg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xaekmjza.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcfevhjm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkaaelxw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qadmvtqi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwbqmgy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fkaxgszy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mwqanjfm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lrlounxj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3icujqwjo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3emeiryzp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3yocecyha.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rctyzaas.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ecdzoqic.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ibawwmcd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xpwzlggg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lsbghexy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ytnanerx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3axijxuvf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3spfruxhx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qriqvyke.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sdgmqogf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xvjvbhyb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3optitwgr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbvyloyx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hihgghhi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wgfxzdmz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkwlqljc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vlynbtkq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfodraos.html


<!-- 参考信息 -->