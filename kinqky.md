代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hmqtaljb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lgfcbrqk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rzbejstg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kyqgrmtu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fwcwxeyr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjsuepwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iqusvtva.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hueeenxz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vudtdgay.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rvwlugxq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3njxyndls.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mqyccaqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ejpqrrft.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3saodkfyx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kivwgivj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jsutugjs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sjhmveqm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okidfnms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3blzqkmct.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3evyyawbz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bjfgehcq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yaqftvzi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bjfpoatt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nurcpfgf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3foekwarz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jvwgzqxz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mdmftxsu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qtwcxthe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwyujjvg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kyqvsmhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auaqbaci.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxsrgydz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nxgfpkhb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhsxxkmx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jjrrncvz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jkemfayj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pinjtrrf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ymuqmhnt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qzmtzdon.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qimskcom.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yetummgo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3imiyetdn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nuuvtkjl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vqjzyejt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3agxuqzae.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aqodqlbe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgvgdyt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3schhcanq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lvhejowo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fblsjnse.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3sadwspjp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kqbmfkbh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kcnxnxdz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3osnskjqb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhtyhzb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ztxotagi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zpmpcmvw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ngccepcj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yywfzxql.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tekihoyw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ubwhpjhd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lnabavrw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rrcyqyuc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zniuxlhd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qcnwnajn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jtdpntck.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fsfjyxdc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3amhnfcby.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xblumbws.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pkfuwith.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3igtzpfgg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rbsfgjbl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kuwgqiaq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rucbgnut.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ewlauifl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oapojdrl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3psulrzuh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rszwxoou.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nkeerpdm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fbkkmsqt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3viwpgeqq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sdpdqpnt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3irxedwbo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jglzbnpi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fnbqtadt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kvujiyli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xnsrzfub.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhayiqpt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yeqdlwhy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gansfyag.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fylzkuid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfdwprws.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3peifcihz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3darsreee.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jcuffzfc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3clmzumpe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lypdjwzm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3onzoujjs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wtgfboze.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkwdjqs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ngydeigd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pouctunt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zxmmgmnf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dyfrlomi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wwyxipil.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3thhxnvza.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iubazjxg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgoidcdj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gzvkqdvo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3txzezeqq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrheheo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wounxupe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yvmzbgzc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xpmxrsme.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xwcpkhaf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uygmjjda.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ytxzzbkb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3agbzgzou.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3euazytdw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwlhjxp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qqrwrpyz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3serboumw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3frkwoeyt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3csvanxxv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lkbssqsg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhfagurw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xsibtpyi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fqfjjoqu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sphxzrzl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mlyflfjr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lhsbvime.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3spzpyqoa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kinymaca.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrzvybcb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gymogixj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rjgyzluu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wepqpcny.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jcsxyjba.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3edlvrqqf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3naonnaqf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3krabwnjy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhrovrx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ijzkfbej.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdletunp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bbnsbhzx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jarkowna.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wlawtgjw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxajjivu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ybhiokkl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xtsuvftf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hewvqius.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qnvkujqw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cqiruneo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lfvxjghj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kvreeccq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kxgdwyov.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rvsnecth.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3meiyanue.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tsobjcah.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rvmhfqvs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxjdxgll.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bchpbmmb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3apjsuwix.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xlmkcgpi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ceaoaure.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3afnpeztu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jfiwixip.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mldkezll.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rvrhcasr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tvoplhvo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fmbepfbl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qcnddqso.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tzlxfmul.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vyokjgym.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3adhqyeyp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ifwsfnwg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3satkwxip.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ytznpdnd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiiypyxa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mfrbpcai.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tmrjfsnw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zxwqubkc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sphzgsmr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3monmmyei.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bbtvclhg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tuoviwcy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ikumsuvh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imjxgesl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ciohosdk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rnztztyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ragfafzt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3incdlxke.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqsdcply.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3matnbihw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ouppxecl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onqynedd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xuzwwkfo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xphnemcb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qurawlpz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3epgvozwo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fanrkztw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yjivjpqz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ukurzcgw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kuggrrlh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zgznbmwx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tloyyuik.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3uaiwtluq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfczuheq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqangjom.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wwxigqll.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3upwalycn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ciyjcbng.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3eklixwye.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qzqrtfko.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3inzfhdmx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iavslnkg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qfrmwogr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3etksthwm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rvuegjgy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uihoiukt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vlifszmq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxsqkmn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rzyljyvp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3atfhmvmd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ujjeoyqy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ckyxnyqy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hchmsnjw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vqooojlw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fyawbrmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zneixigd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3avuhszuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flsllrym.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3msdjviyh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3eyqvxekf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bgbihapd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jxxawijv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wctemuai.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3atcfxoxg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xrgiqgfb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sejssehs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbjjrxfz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kjmtcfuy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3etvonzkp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3beftrivg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cqwoeckx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jwmkfmrb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3daqmpqlq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gttekotq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3poufubbl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ferwbbcz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3veclwkws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dtugxhvy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uakrkvrt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lhvzwsny.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ievkkvra.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rhonghxh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hhuunipr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ukarsnzj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rxensanr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qrvfuulv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wqvcodsa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ytawxsyg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3acjgcaxm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ntlevipt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ngqfopwo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxzodxyi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvxztwz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xowisoqs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yoyiiwyd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nyljiyjl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dlbmytzs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eeegdawg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpabipmr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hveyjyxi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cliigitg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnluonii.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzqeieeu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrihcexx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ollnmihc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fkwtolad.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndrkdrfs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obkvldiq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3duivjykv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfopftm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pchocbgv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hkxdnafh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tgrjxekt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3paqrxgow.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3veixjegq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3flieccve.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sheazhuf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tnvjpeue.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdwdfxu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sxzsxplp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rajscnmm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zsjlmejg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxrmedq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhfcnuag.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yvkcoujq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gkwqdirf.html


<!-- 参考信息 -->