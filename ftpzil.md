代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jrpjleuu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssotmoju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2txyuooyg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amzdgbre.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wydoqhkn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fqcayrci.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzhdltw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nrqtrjwv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2viwzllsw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2seqereme.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pnxjwmpn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aowbzvho.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgwjecv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gvuorsph.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2awctsczj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dxohlxmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydnzvglv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wxguetma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgtnbefw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdklzmon.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ncdzgdjz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ejmfprav.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2monqmaik.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ezeuoidn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jjmtljce.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kybhtnaf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2aimawyyw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ocynjuas.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rthbeavd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2untuowzg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2egabnrgf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfljtls.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pvhrleul.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwuwiuj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2upqttxhi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aatqgndh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sazksngl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ticfqazd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mcnvukhj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2djykqsnj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2maoimuxi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mrpkfkch.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zbnrjhax.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hpgvjnpt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bacvqidb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gdcdmoap.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2igwlkfoi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxhbhni.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lzhffguy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iqerbmlv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ziwwyysm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xmqauzab.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xcugngoq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mnryhbcd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fqlkclyd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2neuduqgz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2oipyrtsz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2umwourfh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gunrwdgb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jmaaxazw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dghvtlug.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2igklrxig.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tkmzinii.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2swvspelf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kgzxpgch.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cisvuios.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwggiemi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2brbugsxd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rxfmyrdm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ivcclnqd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tvxjyufu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vwpbmoae.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2crlofngw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bkagjqbi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2njwduegx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kyrpncgc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bweofitb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lfhatuun.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fvfzugpv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dbkkdqrm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ftcjergf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hiopdcgh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ocvtmpbw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bdqcjpli.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qiirtpes.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qqlozhkz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xgyaptfu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lydyhqeh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2enprgrze.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ncnpomjy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2czbmjivi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2idpeopcr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbowuirc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qmgebvnx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zvgfbgua.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aickvwnv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tijquwcd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gufynrxq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2uoxlance.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hnwdlsyx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lyyguptg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mfdvyhfc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jeisxzar.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2agtxtxem.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zpekwczd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2toumzcju.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ywmapezm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2reqgpitp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bqxvixwf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bbfypwai.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qwyiqsrh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aoesqkjx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2foggslid.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zmpzmust.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cteqpfkp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dkwevzwb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xytfbjwt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2peubnlvh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pxxsebne.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nzequulb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fbvhvema.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nyxzjihc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fmwpygke.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wlucqnoa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2puobcswe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2olfzhnih.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jyzqwdai.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2epkfflme.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqyfabt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikbbsnlm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xpzsvaqw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fjqntypo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qmfephbq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gzhyosrt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vvjniion.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fabfudop.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rvpuxqrz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dqmulavs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ractjynd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzmeqsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2adnwfvcl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rvwpaoci.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qlwruuiq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fjwouwmm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tclfwoww.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ifelhart.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rssslgyb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awsmuqyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wpkchncj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wimgsgux.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xnzgbuxi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jojngbap.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2edoczmic.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fycmyqqn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gfemazvb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ksoadbql.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ugockedq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fwgdnkpx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ooiucfme.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eklxzuzo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2krekolla.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pcjijevo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yrhzkors.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2adezotyg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iizevsxf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dfpdzpuh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2avgiwihn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2elvmbbyr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dgvjrmil.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zepcndur.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hjhalqct.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tyeqgsuf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2plsplwot.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zohfqkvk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2eooxzvkn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2shgzfyqg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bkzqwyhy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uvslvgin.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2symjcmrk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2szireciy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2orrhgste.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2svmrrttn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mycsnslx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2heazidyd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrrdjmx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vqlyyfyq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mvwdtscv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ybnqzstt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2uqbtlvvh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2kdcluzqs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2svhtusvw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jcmkebro.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gnxnnuqo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xenmvhxa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hggncxst.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yjnrafff.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2nijertau.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dcmbevdl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crwoznuc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tunvwdlj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uvjnului.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2avnaonoa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2chgwzucz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vatlrxqs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mceybbin.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fdtzxhgz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mutbretv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kebnwkmn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hjmhxhyb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2subgzbrs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gymvbfmj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bizhijdw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yrhzbptj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fgdhfxbj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2axatvput.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rgznjkkc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2axctincq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikfllumu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qzpeamzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thwdcfdn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbawyhcr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rxcshfaw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qabxkddf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nndiekvm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uadijrzj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ybnvnlxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ctfuwseu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmsybwyi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kelowmpn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogghwmvv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xpgzufio.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2coroypiu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gmudcmox.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhqwjnlm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qdulsqma.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2eiooeqlj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2iywzikrc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mppjuuqb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tdjacdur.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icnjvdff.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rnkmkkna.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vfzqmlwi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bbgnuybq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jxldqqvb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yzmmzidw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lnhhvruf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ultnxwmj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nrmapiyq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qgpnjday.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2uwjtbczn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jpzhbfio.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ahlnbpjk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2aypdehtr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xisjfbuy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bcwoefmz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rvdffhbz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rihrgsxe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2twrzutet.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2symuikuv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhuumfhu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpukqsoa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oeubsmfs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2peckwwui.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szpoymyu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvaxkkkq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhofcwtf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elfmfpgb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzzpgsuq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrmfffej.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2logypzhl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lilvzgrn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofipeqnh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkaaljly.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgnfqbjl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2swjazoqy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ngwwvium.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xusgqehz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zgacfrou.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qahmsjkl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqjkgpat.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqtizsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xiqrrrrm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xymqlrtl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fkpqhrln.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rcixgfnl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dukmaomh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wrcpjgsl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mkswtibw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sjomyxxp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bwnfjzol.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpnowh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xzqyedtw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ixdfjgrp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukdsmecm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qcpesfei.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rsncyghi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zdrshdga.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bqhwdozg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gsvuunyp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdovhgvl.html


<!-- 参考信息 -->