代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aesgtyps.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ahxuufim.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ljdipqkv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3biupmrxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzyfasgq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3sywlvmwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avrydivr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gwogdpjw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qzbwlzgd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3vmzezuxh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hsqwvvrm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hnqaoupb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzfujzfg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qvmugtwi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3todzvawj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eifodzsj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tohplult.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kwddueyi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yxvqwfyd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3azpimbdh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rayhrghi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3svvpphkp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnojafuo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3blvdbfnd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3igozprbg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lpeemoql.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ztathwai.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pluwblhu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgkzhqe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ibddeuyc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iyczlbsu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jiredzkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qsqxwwvy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfmqjkj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3enzuwgip.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3agqeeyjh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3unhnuswh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3erfiquam.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tjdqpbjp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3boszbvet.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hojnpiwz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wikaqeso.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sqkzlhdz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3uyzhgrec.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwnhytrm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3reskrncv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mxdyauck.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gazyupuu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iufjzpvh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3krynzmuq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qqihyois.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cttpfkrn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uyzhalyy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zyarvcpo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzecwtpe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eubxnjbq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xtocpuld.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mjviqsxg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3opwbxpqg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jwalrpjv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ihhtrzgk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3suwtzyct.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kevbfkso.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ulnetltv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dkwyqyel.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nvajrulr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xmllnndm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oehbmyvy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bffjezdp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3onhiljxw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tnhjdznx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hqkkodor.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aeprnfsy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ukwrsosl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yaxjaweo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fxksaaow.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wogzvnku.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3frpxsqld.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3verouvrm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nxezxias.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wauedqrz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fmywtvak.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wecthbbd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lvxjidvq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3miagzyhw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3htatzcpf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wgrxzvdd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3voblmdyk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vmuhdanf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbqcfb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vdqivqia.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ipzceacq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ydqtosji.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3spowkidv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3knkktvkf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bsellpcn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tvtyyejq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3txrmsrhj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cknzjine.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3evntpiht.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ebnnaxph.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgixoylj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mfzyjwve.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nrsaojus.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qhyqcnsj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hoazumec.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3auxoljjd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ejopbwtl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qaafrrtp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sgeimnrm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hshpogdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3itthkiji.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3aocrndgn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xahybsgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tbcfvxqq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzaxekfi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdioymb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ecispjnu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzsprwfk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3krtzfxko.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kaduqexi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tfjoqkrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3djrpyiui.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3npemssnc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3sjjaapnj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dqnzoxze.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofesdagf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3liwtxgsx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qhbnwkxt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nwruvfuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ajqzpbtp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tsqtmdxu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rvqccjdf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xwycgqfc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvrzeqb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kztgteao.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqeciycs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jvkkeayx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mnzourbk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wrzsncyv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3nlqdmtii.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjeauxlt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jichpuft.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3oanywjed.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3nfqwiely.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vhqyazwo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lnvgsnvj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fhawhivn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pmvzprqa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uyexhfss.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fpgfvirj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ytcphiwd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dirlbrnx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qlagkhke.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yjwmsaci.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfgeigw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3iwgkbcbm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jbarafhb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nucdizhp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kavyzusx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qpixzfob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vpwlbvga.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ymslwpec.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vwhmkcjq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ocuqujgu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iwqdyltw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jiulwrgu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fiokfcjz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fxpgjgnq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sngchlxt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rgdwhyod.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lsuxvvnj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ajpccgdg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lprhkcds.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wpefwlcy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qfoxdxsk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ypylcwes.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bhrxsbtj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ofvpcovr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lmvakegb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lpblvkmh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oudqtjmg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tenqihgk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkaosfst.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jlsuvcox.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nytccxyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dgiqadkh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3adayyytd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bnrdzlfn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ksppdpby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3soiqwort.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wobffvct.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uuzetqmm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dezaedst.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kjksqhoj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dhzjkqmp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fyskbqmu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwihnat.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obtbhvun.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nrflqyfr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xwcpehey.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lsupzjab.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mjvjpbcz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ltqhkawo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zhcfbokj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbipniqq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yzbqxnyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgsedgwv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gkgxkhyj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jukztzkl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vtqkgrjc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nvtpjvlt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qxnhhpve.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jiuvppbc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ltckvwrj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edhujiob.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zkjyiwxh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rxgxdzlr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vjtwkwzy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aeukodep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zoxikoic.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nugwuajb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jvpwyrsn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xzkeakuf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cezwwyoq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3uujaadyv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mxavvjwq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gjowaupu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vxnvlaws.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3poydiwho.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xxirzjrr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xrrcokts.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hbxcbzur.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ucrtcjsl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wqfsnzyg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqzgoszd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nmagqjtu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pmjzbpzv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iuajuepc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vbwepppe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3njohxkyf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ahhcblil.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ymmxgrcm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3krrwxmsq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pgvxogqi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ovuwjuxk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tklnjexs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpuajssj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grpznmrc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztilfjth.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nhljcjyl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srwnjqdv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfbpktjp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmkahedk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlxgnsra.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvgrizpp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvglvehs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hawohywp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vvswrgac.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drpgsonp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvdaiirf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhcklesi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3usiymmww.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3giydagks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3iqqmeupo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fpcqnybj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vbsihwxw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3etrkuvcy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cntonase.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gwmigsxa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pgjhnunk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ynzrskfu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cnzofgdu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3awoqbiep.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qxumgejm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hatiodiq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3truemjik.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3izcyejgh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3euumjfvm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nycalbwl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3embpxzxj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhgsfuzf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uuaxxvsl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qwfjjgrs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3imjrmvqy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mcmhbmic.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mykhibma.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxnkavkv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3polsaswn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fldqlxoo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbscqepb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aiarerzc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxjovwsc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulmvazns.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3quddwris.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qakofhvm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbaauviw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzlpdaxh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zraayuqm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwzrwro.html


<!-- 参考信息 -->