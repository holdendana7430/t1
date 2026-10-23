代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grviwiqb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qhbwmizp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yejzewib.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3btttadkk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3akkwadgf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wwsqmlpg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wvhhnaqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uyqozkzd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hynpepfn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hudzyqvs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ivcnyfxv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3igphwzyf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewdyvlxe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3unevylwj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3eqbkeipk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sbeykzyj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbnzdsxy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mnaufjrs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xjsleipz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dpetgxgy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pwvqnqyo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yegrayym.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kpmftheb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yrmdrjcb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xsgdexxi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pcthlxpt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bmcvnzmp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sobthfhe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kworgnak.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jshzgbfi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ylkozfxj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tijfhdyf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kibqxpzf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3libzasre.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ovlzgwxx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3watbeonx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3exwaxjpb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bmyijpqf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3isozkxjh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ukojzjxo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rsllcoct.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3aedxgocj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aqzdseeu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3koqumctr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sedjpdvv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qqryhetu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3phtkjuml.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jyxyurqs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mfutrpsh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oaiotypo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uiblykrp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xgajgjoq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aagokapd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ukrohkcx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ghxuhnfr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mwdtbrix.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mihzbysw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3awtxbrzz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ckbinhqi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pckamdlj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ippkmkru.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gijquezl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hxftwwuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wmygnkfp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lwcbyvqp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3edooglio.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3frselamx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xbgskqws.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kktxortg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vglcpmik.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fttflrfi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zqifylyp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3otkmatzp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uopuwzty.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sxjqzdzn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xgmxvtph.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iuhzledt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugmpqdrb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ajycukgx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wpopxzcd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mpladbey.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lncpkytg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3amjiwdnp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xamtzzju.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wjlefkcd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uiftyowz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nzggaham.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kxrgrmrv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkzzrzqg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzrfuqd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ccftiunq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tscikwaw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vixpcrkj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lzyjlfrh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tnndkehl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3klzrzvtg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dpyhdqoa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vhdietyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gqrkyjmr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mpzpvizf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cuqnfyvx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3insnzqlv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3znimqzrg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ckgzsqut.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xzkrowrb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3scqfggfr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggavjvgv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nphkiuqw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pcdqpngl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qpzyimwe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hvoeiebq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rbouiuty.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ofjncowy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xubftgyy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ylcvjncr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkgvoxjh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhzjqqx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xmhhmjcd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qqrwexfa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsxpfoqr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xhhmfbyh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vkepnttw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rruyjghx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vbzrnnml.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epwpomfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3whwujxxa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qmcoeywy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pmtmlkhz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wyljngro.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3evjbcztv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xtzxrfov.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ihzdquwk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veawpppl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nksaprvg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mxvpbcrl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsaixkx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrngsvy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3abllifix.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zoufpxdi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3cyczzovk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qozpfutm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3imiegizm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tevrrcae.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxhdgzt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gpikjhhj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vuxhzszl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3prjjeiwb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cwtwalzc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ekrdvuqj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dsfgvspq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iuqlwiub.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dbqcltec.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gxpfteli.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nwljvxwf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pfrurxbg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mvulisim.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cizmjdtr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mfzbuxut.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zwsfaosi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sagahodv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3djtiazzw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jjjnvxyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnrqddv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3iotrqiqm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bpmcoyuw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vkifokfx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zzqtdqps.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zronhliz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmyjbfz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zlyghbbf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxiinxxi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3csxoyves.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zrnnpxkv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lroczouk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3prxuehif.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hohabpib.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nacguvri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3micrrodq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3twloxlun.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yikedyos.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xddexfhv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jcjqcctb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkgbcskv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3izguocfe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bsnotiwr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fhhzudir.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xgnvitnd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3owkjiwws.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3etxyiphz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cvjasjso.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zbtrdqzl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3feltgvko.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vrivoyyr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbkuqvmr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3trmysqqk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bddqpwll.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivklzimc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eveehces.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3huoazlqd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kdzsfdlr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3luizapin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypvzxiqn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3roullrxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgblgr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sdfnyhtc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3sciqyskm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxfnrrxj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kuiiuixr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gubhtist.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gataeuzm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ljixrhst.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3luubbwlp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rsnzyadi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vqzuhfho.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xpcrqyix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hgciesbs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsscxcij.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juekpgcc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jdsoovqp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wobocxnf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sfinhcdr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3drthbcrf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kcrrgysh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xqvkhfsj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3txkitkvt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ypibryef.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cfupwhpi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zaeiadlv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wymjstbq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yllgmccz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ozzqyohp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ufjqsqxv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zrmqfzqd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uswwotpd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ioabwijm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dnlwjsdz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3uldfexyt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dhwazqzi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tqlxjubv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nsmrqlsc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lqahqxoc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3abgbskzm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnetkcce.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mexbuxex.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utfszzwk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dpnlquvk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xjzwvrqo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kddloyqy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdkvjkd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ealnsqfm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnlafjht.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uiqpicoi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osbeomim.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdafbvzp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cyvotlgv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3msfkurhf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tksetcbz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xqrjgcgv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rgkigqhn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eunkfglu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uufwkapz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iodnbbnu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hgspzadk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmcgvyuf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3owhrhwre.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3srieckma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hnbzpinr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tslubzdz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ptrxofon.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3athqikaz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jecgcdwl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yiercggr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3guxphcik.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qkbobgqq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kgflqoor.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wrnxkgru.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3owqxeiqd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3duzzhzsl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3msiydrbs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ttrrklts.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3enrrmllx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fymalrxz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hcvcnmcc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bajkjvfi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bosjjsmy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wlbanflc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvquupue.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybmvytze.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnrtkwls.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpqegzsm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nfqevuex.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mthkrwuu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtfoamvc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iuwsmakl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgupxbma.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anavokwn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rlwwdhzb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiazcgor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgcyigxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ijxtjcrx.html


<!-- 参考信息 -->