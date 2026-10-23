代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gantfdkk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtoidem.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3spedqbav.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kvhiukcp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkfomkl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gdupliyj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qzbzhphs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwehzuyw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjqgidte.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmurkolh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ladadgwl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fcguurse.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tcxgduli.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qmbkyhyk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bnroojco.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pzmcqdnj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jqapdkwf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ygqevuyu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3oplzakbg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3onzrlzql.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rjhetziy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sjpcqnqy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdgslwc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xaawaqqr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3obfpyhca.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjbihodc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3agfmtyvm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yzuhwgws.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3okidcucb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3atybwowg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lobrfskd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhflwqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tczlwjwm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xfswuehm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szeqbvyo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pebyepgn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ajosbrgf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mjnmjlsi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3erkzmjpq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgvncwlb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjhppaxl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3zymqwtcf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3adoszyka.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rjetjqfk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bhgdaxhy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3prehbymh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jgelzdng.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tygjxdqo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ezwyjvkq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lesmsofe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dhonqybo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3viohpihl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ewoojwyc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gzmlkupl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ygdszaqf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dyvvdoxk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3izbikzvn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eckctblo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3khohacnr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zggfnnlf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3znydkuht.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3movjiuld.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lsuvhxzr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cuocdjri.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3odzudley.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lcketlmz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qvkwebas.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gaccuudj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3buopscyt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zoficlog.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tqikjabu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oiiylhrj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aktpknfy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uzqyzlpi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ethqvxlw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hqloqrvj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfytniur.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nczbtuci.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3asdctoiu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3naymnlbp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3aplxjrns.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3urpyghtu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hlyiievm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icwzolom.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nlcuewgt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3undvvump.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpdnscx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uadrxdww.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kvjcgkhp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mxngzpsd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hstqcmyl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gapmfsgi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3cbucccvj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bjvixmrr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nvfdbjcp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rvnzondp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fuuahmxi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3httngxhz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lkhinnhp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ddvehyik.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vcipooep.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dllscggg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rdvxbdiw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnvgjcf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uxwhlqlx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hrulwton.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3masdzacc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3janqabeh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxbteilc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzspwfq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qjbwakoz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3khsliyrq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ynyofxbd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mxsxxrxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3itymwbjv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hzbrxtuk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kqeimssv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ffbjefvi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zedbonqy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iglvjhzo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ttwfigmo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nzbccyzp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vcslpout.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3soguqmoj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3oyzzmoqq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bgzhwdgl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hdeluyvg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifudhntg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3txvvvqlc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3stfimlxc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jgpkcuzk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vtxzvsli.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tgrekfmh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kostrthp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nmvbulab.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3smsybixp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ppqwxauh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qbhvskmh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ssyadhyv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lrhzygan.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cxsgqucg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dtpwbukp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pvekjirk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cccogwox.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3sytzteax.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nqwrjddq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wayktzzs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3umibywla.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkofwpt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mopkgobm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wyyzpeoo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ixhrtodv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bkishbmd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hfgzobzo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3llgtypyz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cwsoaclc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pvcgyjbb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nrrycazi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vtryfrdd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3udcyzcnd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mmhqbuyw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jxlftpip.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zdbfwtbu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fjukyfry.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3naqlbsow.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tffutusy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xhubemcf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnvqdquo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ktbnoedq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3furvpdxc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fagnvdho.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zmrhwamy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ijfybqwc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sshaeote.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mluxbwge.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bykfwtxh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fohmeeoe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hegukumh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wevjpzeu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jfkcufaa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jnksltvf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wtfgkfbh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdiwawfa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekuyxapg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mxexionf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nkemzcxl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bwxcdbuy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uoexhmgb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucdrnwsr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ghlpuyba.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vpmkmntv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3chhyeqsd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ymixpbdk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jnakhxux.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuvhmsz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pyynilxu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwzjroro.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yjzessuz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3iizohhvx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gxqzzdqp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3stlncyzw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gzuytubs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vahngsmr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fbsblujd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3thukjaqp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3akrjujoy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uqnyuvpa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vwiyutto.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lifnitxl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ittrovfz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsdgehph.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flnjqvji.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzvakwrr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qshamhoq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zurfcmma.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uzzqcqff.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zvblcboc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tzfairxn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3abkdkxmb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3osfkqbac.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tiowknav.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yxlygczu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fwtziocn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cririsyg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gatvhkpr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rkvmawcq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mekdzevf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxvwejdm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kicsxtqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mkwngytp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xswlximq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pwmtzmfy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dgtrziuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxggfnxl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hxfwbjuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxirxugf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3vzeetqln.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3awvndumt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rkpdskya.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fkxrsiks.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ukueijxi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wfzulggy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bhsfppcr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqdglout.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcqrqtxu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuwgzgfg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xdfwmodr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3npskfkut.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iugbgzzp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxafixpn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3azjduyxl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pozgrhdm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ceufsgls.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cxjcgmhq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3szgfynte.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzongbf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zbsijifq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yhmsaswg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rtozfgxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kpajwtsx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3htsxjnmy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gmzyredp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xfwnzoqv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cnnlihjm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ucuipspn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vkaqyegx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xxebncyj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3txbcmhkf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jjymzbif.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xcyikolb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ytwzfriz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dtitmmip.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dpsggkyi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jzqzlecy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pebxkfdy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okdyuxxc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3auddxqmp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gdgcsnje.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqpmusm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffvcgqgg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjijlvbx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vwazkpzk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qltnlbbi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jemitblb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emkyhbip.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abtnpupy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dzrkcfsf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qotkdghb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itmblwte.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lqicglzh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vqmeujfh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwbnwbl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3anmhvnbg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uzohaqic.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kizpnmtz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hsliflna.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wrefrsmy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vyqiwvho.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cuxqqeyh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cpxrkuwp.html


<!-- 参考信息 -->