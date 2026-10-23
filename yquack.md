代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuswmkas.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3beweuhvi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fuoedctk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bxnypupd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3buqwofta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3emomenuh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3winttajm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3torsoltr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uwqfmdhx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ekmsgkny.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tyirunlr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3aephopqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3evelxcuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbayjsd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hmyfwaun.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hwrnurdo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zlgfpnse.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ruauloti.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lzvgvajs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xsyxvxds.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwjhwwl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uefhzbeg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ddqtkeyo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cutxnfxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfzxmuih.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zernnizq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aggnxrjo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3unmjxzcf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3plellljm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iszezaho.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmflawih.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3scepzfke.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3shwjikko.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ooidlzvf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wmzaktxa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3joxbxtsl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3shldnbiz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fsfoajfb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hxqkrjit.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ogahqawp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sizznubd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mbrrhdxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qhselzge.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3edwfntvn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fkfcsyoh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zegcsiml.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qsdwebse.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dakulsvp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mspefsgu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tsdyvmvt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3penoqhgj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bymkpamr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bycaywar.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mtgbwaal.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ewkhsfko.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sxprcbzx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ncpcifws.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3whaxmzoi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eqzjjwxk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3segchcas.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hgobhyir.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vudsebue.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpioemw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bfblgckw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vfzfotug.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rdokvgyk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3odpusndd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xsfhjvlu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qjvnkxbe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzybcpmu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vopzcsib.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lnncqdil.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zfyorbew.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rdynpgcs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3chkmrhlt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fepykjfl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3itumuliz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ifjqvyjg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jojqgpgb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rnsqfuig.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cehggkhn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3klsqyolx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iuwfspcy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3syhttckv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlndegr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vlfddbux.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dbmruawf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3txqlsufa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ntkjopdy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ukgkgbry.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3labwbvyk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ywbxjfus.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wbixiboa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mtmdstzt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zkrdsdfd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqawyvf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eyozudxf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ngkmogmb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dnwuyxvx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kftsckgw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzhikfze.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jnoyphzu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pctnryvb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rjzpafbo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gmpwwhsw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3poedjizj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfeljtf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hbxsqrke.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ysrykapy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qukpsmrx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tzlnbcus.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3urchhzws.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lticfvpi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wnexvdjv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3szetvarc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nfpwkzgp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ddtxtkph.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zmjpchik.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rjgreeus.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sizjgagy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jpnyyiwx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cfbtymag.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qggkyfbp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3geqvgppz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bxofsrhl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yfpkinxw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3twdqnybr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dzmrhpij.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xaueijoe.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3reqvfien.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qbtsmtrm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3htdufysm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fhxpcwvx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3akuamuvq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rzwihsml.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3arhmaowe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ihsxkkzc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezeklseo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tqxmeamn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlfwsifw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ynbmkvej.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oipdghph.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tdtszcnu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3galqqnjf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zfypjcih.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ewfmqifa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3pcyipnwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ctpoduou.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tgqymrmm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wsqhlfvl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3abggoafu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3phoxnten.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mqatwojk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yyjjqrfp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qgshmimr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zaqqntcj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3znzfivjq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqpdfw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pxqielyy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bzgfeahv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3trzthsut.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3curtaarv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ftqzgobv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3icyefobn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kwhrykgr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lulqkzhj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jkyhwjda.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vvbvuvry.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3svjnxcpc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pyhyxlbd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jwiybxik.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3egdqsuez.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3trizyhsk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwlbsngs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qdkgdhwe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jocnipqr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wmkntpnc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bqaqcdme.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jrzkktlr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xphukmhg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3filigyib.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xvnmmzhj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tdroihte.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ahxsaxns.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uiihexrg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3swhmitxb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3icwlgjav.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbgmixwj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mfnyralv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jzmnrevw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3apwznvfd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ahntmrys.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oayzqxzp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qqdgujvj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cxpktecr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wspfwlnv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3plahzfqx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hxnhathw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3iyzfjvyc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fjmhcgjv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zuqczgir.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjqrgq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcntimlt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3shttbave.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rckhoqzr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dxkayaqi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqorsxqb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zobgmbtu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nakteisq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gztqovpk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rqhqyies.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ycwjgzzq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qxwdonuc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ndzjoftn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lhfawpus.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zizteyyu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qegqsvoe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jtrzkzyj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3skvwsnhm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cgowqzgn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3urogshya.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ijzsqxhg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3miwywpdv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3srwrfdqd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zxgriprc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaukmtrk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3szsauidw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxsmyewm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3twzxzjrl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hofhqtzo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iucsjioy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zpdrgcxv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ecjbcons.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ifgjupyg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qaylfhpz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bowahzxq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3evutopbm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbttyyld.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mlhpdjoa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tpgxfvpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hppnoiif.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfhdmlqz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ctekucri.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xzqtsimr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gediyjbu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfzlwbri.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3spakzzyp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ghomupon.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yirinvsp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rlbvwkcx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qiscmgux.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qxpisruh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pqatemsp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dpmbdfsj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bflolzgw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3anhnirjv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yvcuwxlp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uzpvduld.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3isilplra.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kgkuapjx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yohtkpvl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3knylswad.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3iuguxstu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hvrjfcyr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3armzpodf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mvhgmbob.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xymdlyvn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wppkjyaw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fncbrlzv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3smwfwslr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3udftwsbt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3natxxzaj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddcnasuv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3txuuqvky.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kezkdbuk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gtkqolsf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocoecmxs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrsxubiv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3awrmsnrf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3apndyaul.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frankavq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xuhthpbj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pomwqxkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ivokkawy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3calfwmsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kntmnime.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kkqtwdfy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cibymfer.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkboldo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3arxpfnbo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3agkxxkyw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3olwukqop.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3abjoxeha.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3izsmypcl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vohmfuts.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zvlvgvdb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ykewpidv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bulrlnrz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fecjfdud.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nknljlgf.html


<!-- 参考信息 -->