代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cczxhnnb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3abvytlbq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3symzruku.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3airtnhnk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ibylzuof.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ilsbxvqp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qcyzrnmz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3raqcehbr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aotrulrc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qefhevfw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3enjcktrs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rsbvshgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eozqlgzj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ipnkihsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3choxtbjl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwmxemzt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rtpcavyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3frlcqmig.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3snipmfse.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kbrhnoiy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3uzjgreoi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qcsuzvqk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qfavemay.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nwveqykn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oirxyrpt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bzrgwrci.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vgfsgrmu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sxrsonuz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xtgoqiej.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrarfofp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bkobupkt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dyexehwy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vzhnasbu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pbasjfcy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zdmaemft.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dfncoadx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnnhukp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lhlnxphx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mldmwxeo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ncheoagb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zmbygnvi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yeroagel.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qqwmzjcs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rcseouql.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3grdzlpif.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnqjizla.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gyrgdhrz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qznqsxca.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3daebobqu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3enbvsppn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cnmmiolt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lqrcprtz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jtzoeudy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hcdhjyql.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uykpkkrt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zcizdgwh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nhojmhom.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rsngsgqv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mqwsozdh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xtczilru.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ymljqbco.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddfwmtin.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jlbwxaua.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3idfcsluw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wzgskrve.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ecxeulpy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvhnlfh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bpxnpzzc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jdcdvdwm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uwtwfuch.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3abzzifja.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3objqfwmc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3szuhaotj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ulepduis.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qzkridys.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htjedosm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kgnttbyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hhufcygv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3keddudxh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3iexnbkva.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qpuopwmm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qgjkxhza.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tbbulwtl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tjldekaf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oisbzbgg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tmgfegyb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kkuffljb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ryqgcjsi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hllbfhbo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gakhtrfw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqonvftk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nwwmuxgs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3znbyhgqz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ikkziilk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cfjyeemm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xicbbfsd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3togodufx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rlwqsfzi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qyalaofa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lhimkjbc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iiizyuow.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cretpcup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kicvblmt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3izniyhub.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jylrctte.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qcgvwkbv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kgyeitrz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcccemlz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mlssnixw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rwfzmztk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvrzeoka.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uthftvxk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kawxdfvq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3axdrelnp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xaqgskli.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3magjdklf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vlsewpen.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3phmmgkbt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pofzqvda.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dmhmuddh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3netniiwt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rjhjsdvl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gwcpplis.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxpcpqxz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bmelrtfm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3boofvxfx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzijfzaw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hhyzyuok.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3evfkxnum.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3phwmgxwy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wmplfssj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kangaldz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3esvprzgc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpwzxzz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ksckysas.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vysnuzwi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bovqdnpz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3aztkcrbe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dhrpdlwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hanwdnwr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rgmuyrte.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bfmlxwqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxkknzu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvluyjzz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fsexbwjk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fnclteom.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pccmxhgq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cstzdnwa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mfkrvjob.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mywqotvg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3eyoyupqa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3begnpgxx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jzsbnsll.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pmoxpyea.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lbnytwim.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gngpmnpo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3klybmlgt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kzybtrat.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3npxxqcqy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gltuzzvg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3iqmipnir.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ghyylbfj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3imyehqyb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ltddurdq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3omerztkm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tuyinfhb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wrzjkznl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rlszyzec.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pjwzhfyi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jpuhgjuy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pnbktblb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qajpunjm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xlpfaqjm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gusuvdms.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lqivkirt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uyoufhvb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lygqktou.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wktkfxhv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fidgzvam.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mouddibk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sxgefwby.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eiaqdjti.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3czsfzgsx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cdowuklq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kfzcrpmt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sflzeaxf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cedqoczf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bdwfjgxl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jrbuvemx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tydrnhua.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3khstwpgc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxdwdnea.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cxzhzdlx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hklrwcpd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3iiybglwh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wbrwnadp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3izjjjqtp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ryaymehr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ytsymsff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rbprneya.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ijjiuppk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ltzbigpw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vjxphmnf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3huaehppx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kuxxyyhk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofnvmngj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hxrwalvy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pjpnsghu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jxowccwv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3npzxfjjb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gmfwhymd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yeioncla.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3onldfsvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnvggpvr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ssztkrxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urpgttjn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpygbsjo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yhwystbc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zbuwqdqk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nlioycau.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pfeoztsh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jgovscmk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3aijzsppz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkvsnkm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gmsbuedt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3volblawp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bhvskcxx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ohyygzvu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrxpugjj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wazgsraa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pgwxxyqo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wtrxsxvv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3txmmabtg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vvhbgkho.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tdbgskml.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wvunxqbh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bquxlznx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3islouzws.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sfisjnhd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vhuqtkma.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nxoqbstw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rwxzegzi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dnfljnfq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3amvcafug.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3evozbahn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mhadjcyq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dtryerdn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sydvibol.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jgoombbf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zgxdmhnq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kiyxkvyr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ioidbotr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eprtgkkl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pbcskgzf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vkouvazo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofqduqtn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jorwdker.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wyhhzjbz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3apavdllp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlncasqf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbawsymp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ygymoyxo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfdzzaef.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ifrweyuw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qltkqxoo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfwvsifj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3grqyiynq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnhdvhth.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aymxcsws.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbkiwaiz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mmvscpnr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3upqglgzv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jfpncaji.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uefzkwlx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cdmjkmqt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wgmwedki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pkneujaz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zbxtzbrj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3goxlmvjd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ewkhlivb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yrftcelp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gncapfmg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3elidmwwo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zbefuhpu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mbjnupsm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ovhldxqw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gsyacmec.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3grlacofb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lphemmzm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqbdveby.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3izhfxvax.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ifrmqjdi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qlooyghr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3evavvlnp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xnhzkztq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udpjxcgt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kvgtejll.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nmfqpiao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fegzjihx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3naskypfn.html


<!-- 参考信息 -->