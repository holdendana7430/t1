代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3teocuult.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dkrfyaio.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yyyszbbk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uebeqaxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhbvaghn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rnnxdxwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqcbjfhn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ypcaxlcn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3oexgnrov.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ixhsnegf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tjjsszxz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mntbvhoo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzlutbqk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kyztallt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zxozbkba.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uryvvjvr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hozazxgf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hlvqhlrg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iufbjrzo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3awgkqown.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejklflyu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ggppawxw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3oyecxycd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3otjbavir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3runfrrag.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3spcjvoft.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3suninyha.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jwqiohal.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwwjfrg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ndfiayln.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3frhbuhsq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wefcdtqi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ltagrgjb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xoekiequ.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bcaiktgo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wxdtidrg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tqruhzbd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3anwvxtwo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ilillfki.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3imgxkkre.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ivcuamgp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sdqpktuk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eobhudno.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ewaykdet.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wcgnphos.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yevugpqt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xbohwrmk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nlzordyl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jbvicuqh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3oqquxdol.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3egznscht.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3arbybgxj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wognbghg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxiglgfu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3httidbgx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxrtpm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtbfjyoi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkabizf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wksmadzo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xycbaddm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jpzgdjkm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rvexkohi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zcbzqltz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3skmtnlyx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3paslizpb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3yblqlmzm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vxadtcta.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhrmdgxw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jswsavyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pgsejdnl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3abykaflt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rlbmosjx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dimekwqc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3myqqxcac.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pwgtusdq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ajnzglxy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hfwjghtw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iwfawtge.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ogsyowgf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lyhaccxl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3eagldjzz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jukjjonu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yfigoseb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfysnttf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3slndzucw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3grxwnmfy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uagrqzwm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rhipifxr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ngrucjpl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yquycrid.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtvdgp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3euwaywys.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jhgmpyvb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zuwxlrdr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjmjaoh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3byhahkbw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vqluyifo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bnnirwew.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tiwdtuim.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wsqdccbm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cffisjiw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tcfkgojw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uuczftxs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3knampgib.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wcguvlcv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3citjierd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oclcpyky.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3guskqshp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eszrcvqb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bwhyivmj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ykchjacn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ezgfimid.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jbghvtdq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yjejcqzs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kwvpbgda.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mtvzhwyy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bxaykoap.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgprulcd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvxbmsyi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3grurxrjq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pkfpdeeu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zfnsxeln.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3biuqvsoc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ythmmnxq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3awmchwxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3etgunjbm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3obrfsoql.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ztsljpsb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdebxktr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zoxuviyd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hlvxjlmv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nobedlci.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jrfjtnnl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pakvttcm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efiquhcf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wchqrwls.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bukufzvl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ldmytkcj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fohyjarp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mzhcqqfs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3scjfyhgs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ymkcyfhe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yfdotboe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzdpxyle.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dfohbcus.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ybrxpxeg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3djqmbfbk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmseeha.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pezdiynb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sybuyduj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uvzgluyy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3msjomwml.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gdropceq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3egvhusfz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mrmqsgju.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nkctppuc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzmoinuc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tfuuhhis.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3swlxamzb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3diwyvcdx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qbuocghj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cdwvjlgr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mjziyvwv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kodmgvhq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kienpirq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hwdnuwrt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cngsjpnr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxgogeli.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gobizfuy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aomdoyej.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zvotvplq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lwwheviq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rcqdqftj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sughxryw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3nthmqdyu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ycqywvnc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ffebaaju.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jwtwgpsm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nhhvkdjp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qgedkcva.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zsjaagnp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bxqpbfmt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jkrsvbve.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibkfggkp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijyioxds.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cbulkkgp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3excmttps.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nbmdizha.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ubexrwqn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3buaajsao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vvfyxuzx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pzkiluys.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fygiolcv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3sdnngfdm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sorrvsya.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ppeijwtn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3aqsnjlec.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nsposeht.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3blptuwik.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wdbujxmz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3limfttbb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cxivxzkf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3aktvtxng.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3enyjpfsb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dpuwyuoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wturkvkk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fnpgsrzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhwqpqyh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uvzqbnvb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wtjegmgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tsmhryjj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3alvdgolf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rdmmgjku.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3swpupbfd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ngqcpimb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxxfstaj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfhyeaea.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvnyykle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rgncfgme.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vxibmnjg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erzytoma.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vpojlkwe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jcpnwotw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnzurxoq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jktqkydr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cqszknis.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uligcrjd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjswxsc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gaoauexn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xsceplde.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3luvdkivu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hpjtjzfx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zptrdezc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzadmyq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nfxdqmww.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mzwgbmli.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vkloxlqe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pmllroaq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yaiapcmx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3npsantwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpziixv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pubyxsqj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ujfpvwgh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fwwkejev.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yozknhuu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kwpnmfga.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrztglay.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hejlkknx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cclzklzf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zpqqfekm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gjbzwfpl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qurrbmcj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcegwzpo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjwnwdlb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmqzhcxa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yllrdkjd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nohgfluj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3haxrpyxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qsirzmof.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwvumemb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqvnlcda.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xhazxias.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3accbwgcn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3szuxmeff.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tzffszks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mxioyufu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3psicfbdd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ppaunjay.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fvzkltgh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dlpjccez.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kohqwlcr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lmkznxay.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlnsyof.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ovpkxnxk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rtniuyyg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3guqlvqbx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeyzwqn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pkuagqai.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahlyayra.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3unnxzibq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nyxrbsrn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfelmxpd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ggvsiddb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gibxrfam.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rscgwmyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mdojrupk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rzwpregl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aendagta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wrvggcov.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mnsoghxi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bckbpblq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nksoacat.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfvrlenj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozzcgqnb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bnwwjfmq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kypusgmj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkygejoj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iarcvhbi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yturelgg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqgpjnji.html


<!-- 参考信息 -->