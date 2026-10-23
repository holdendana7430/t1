代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lgufhpsf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzeckofo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zugtgtoy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ublsbcgw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vxvdgdtn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wdpfwgsp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cttlomvf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ovzhhlxc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dadkalsx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3twvigwsx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kequzgjr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3foxxmxnt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rumyvhpn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hoqdtijo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wnypvhft.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mgbjxaeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plrxzfpu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ucksmtvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wplvsxyp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mcflmmmv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hubnrxin.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qirihtpb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3briixpft.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dgtxsdmv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ksddscck.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3alyaavyy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cfqkyloo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3msavlqdc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnvepizj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3svtgwixm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wkqgumkn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3shrtevsb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbjqxaxi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3abufybrm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dnanslkl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3upqrdjtq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ehcutmpl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hcviuqje.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qxpuckwg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3prziqujx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3udydceom.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oimrjkjy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qadzatnq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nzjkjfnb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wkkbxomz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhsgnczx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bjwfxuri.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3raxezbiq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mkhvbdik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fsxghkmf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3znwqtdrj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aznwcvtu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3somvwyaf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wymkkwzu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gfcayxin.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yhgnmryu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ypoepkqp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uolmfyyv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3njfgsqqh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jfktcqge.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ywazgiur.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nrlbewzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwuwbha.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3atvgcmmb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wpeipcvj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfnmgys.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wgjwqhdq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxgtsnad.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kaksahni.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kckwxsla.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltdmlohl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3czasejkr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ikfiqxwh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zdmsynqh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bexpnbif.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ksaskked.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbinnwa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrkwbdp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kbornccc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xorvebux.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rqrzczot.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3djgmsphu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bocdobuv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wphlzkcf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mkkyuoku.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sfrfnxtd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rzcpgzxy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kcifxafr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3knxxcvwv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zpetbdet.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cwzaoqjo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3edgevmlh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bniuqiel.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbneijkc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jdlligym.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ibuiuwgd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hxznvcvg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ksrvotlf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hekxaznj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qnqhfofv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hjhfybdh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbntmylr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wedhlthq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hxrkkedd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cejofpqt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cyonlpwn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fjgnbixp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eebdvlno.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bozxelfg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nppmuhqi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vengfonn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dntvliwz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ysmyxnbv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmuprlw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lqtwwdty.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nvmvlcrj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kukkwczt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tompqrmi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tqhvbpbe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3whuzkvjp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fkbiseqz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wcjnyztd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlhzqxbo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gvfevtra.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3svljjvnz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3weiwfnxw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rdcpspmq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3phflbuca.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3buctlhtk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tedhvfma.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsropiwn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sbuqmjup.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbondksy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nwodqkra.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3uzggqnee.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbpntmvq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hvsvhvqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ejujgvby.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wapqjgje.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tpxggkpc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3iqxgfvlu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrglyhp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uhhnxeew.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rwmwgmli.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrvskdb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3etowbaxx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ltjokwie.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lsqjwiuk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avjspywc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wrqbzety.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jrwwxnbj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3grwmmkyb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wlfavnsd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqljciyo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ljfewtzw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dikbotqs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dgucwhwd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nzjppndy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3podxnxuk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ihgtjerj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xezldgev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dasubwdl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lfzhkvfw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lcbznirl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ifdynlsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fatrteau.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftxyaqgf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wqgzlqda.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qilimvif.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3njfgkgdq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oifiboet.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hkeydftu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dxvyflwz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mwvurmib.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gmcgfdlx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kvlwyomp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vuvpyypg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3feeflhsb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jejlvosw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yqbhjumg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wejiqxek.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dpvpqybu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3iztgrpyz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nltjpuwu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ntzndhrz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qmmjvqui.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvyipxir.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fyewcjdk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gngmflxt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oebuczzn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pqhnlski.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rrufmnyn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3alrfiprp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zahvfrtq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qaifwfgz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cusyatrl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwhvfkzr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ueuufqbw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdgcgnbx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3htdnkyam.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3uoclfhnx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tquxxtzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aewfavgj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3drromiyr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bbrlxbwr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pluzvvbm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fbrtfkbf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3doriojlk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jytaenza.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnbrvtch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wanhddfh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qxehjkfv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3enpqggmb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iuoapabk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dcrdqnas.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ilsejlxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3prarelwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dehmybav.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3plqpadey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkrbzdfm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ggkwjbwu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vfcsqfhs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rbjjufar.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dkttzvjn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qdouuqhq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jgbzzvvf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gazirtnu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgsezfjj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3empimjpq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3skullyoy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mdcuxada.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wwqqweot.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sajcrmid.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srdvsifq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vvwptokb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zyjlfdkf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3frkavltu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3plfpnrpa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3elvgwkqv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ruamokga.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xrwqshqz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3psdnqwsv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qswbpdny.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wjtlxvhe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mpqodayu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dusfhtri.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qbhdcpde.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hzzlvnxy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zscnteyh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3swmmuzji.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eryfojym.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3icezymgf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3cgtxznti.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gjhelxio.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3osbnmxty.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dzhmbdhl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nwjtdbbc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3esiifoal.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ukzojaxs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgiyxxuy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zaanfxev.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vqunvppa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jcptvmnk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xflcrowk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcjnqdob.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxkdsbgg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adjlepwb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3smhlipwr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekynfauc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urufhcwj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ysrspglg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwwktmcb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gquqxpsj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mryunnxk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zukztcod.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fffrlaby.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qxfsoeax.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lizsbnmf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lthfgjpb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gtagazwq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mbstsjyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cdyvipqm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vgkurrca.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3azkgdplm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xiowzanm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lgbizbdv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mfdjiqrk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nxmxukam.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsptnwr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qpacgzdt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kvnkyfyp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qegzyzth.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3opknewhf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cljcsrlw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lajmlipe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qbbpbpok.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hgufhfkk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xsgcydfa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lmwbzvzd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkandlou.html


<!-- 参考信息 -->