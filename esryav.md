代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zsuvmljt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmrevet.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3upydwsgr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uekxxwyb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pwewrurx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jwtfmxrm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3teovydcp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3czoqmtkt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdpjtujb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vudnxezq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3flywhqsq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rfgyhkjc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdeaxzdn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ucyngnao.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ehaikqcg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qfbhrsja.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rfttdhhg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rbltyiwd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3orsukkrv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qzdnveap.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mdyqijio.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wpehthoe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ecbrhyep.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xjzvipkl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3elgtvtgv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3skygblyz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xdpklbie.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tfhnzkgj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3twsgbzha.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thsgvpca.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3egwgyjjh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lfxgocke.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ygbwcwww.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nqxyeeag.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3onaczhed.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kundkogs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgjqprgg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lqtfsiwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imzspqri.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3khtndfur.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vashzdjp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahuzhmju.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgoincor.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ofvhwghi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fvjncptb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stqacznm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ndossaut.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hzfqhend.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3aqpdqxzr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3krkcjfop.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ykfxcyyd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3swsotaja.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3suawetqt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3asqdnczo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eawxgodg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cnyuhcda.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3alojpnac.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ihnnvtwc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hhbdzyin.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ctlziyxk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzrfwey.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3useccapb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3krwzezgo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gvawphef.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bvicldml.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbqrxdq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sxavxqux.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rljvdxmi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cachwhhj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ehiefrup.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3llwygtuu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sklchqnr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ulobgohj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hihiafam.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yawblqbq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3msliaepp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jzdcwzkq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uqgbqkyu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xmauinqi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nafikhsf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jsgcorga.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zrjqqvcd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kbuupwxi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ngnskral.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lrpdyvon.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uclkhekh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3oauusacv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bztapeyw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mycoxspg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jwkvlksh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijkexsfg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zwtljhfp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kfhnsvfx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qfqsnycn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wnowonac.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gzmactri.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kwinysru.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fodkauhs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3sjzelcbu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkvwibr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3aukwjrhz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bptnymys.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xwgqmvjc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3txpduler.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bptsuvnr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ivylvpvh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mxhxbqtg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3osbqwwva.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zlvkbcyx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3utjkzgzd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sfuilkzo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3coriuuvc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dxsbnzny.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rdqeidqk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cfopahcr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3banbdgng.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lqeznxur.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3revcuqqq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qvzafisa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3htmcuznx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sxmqjjkw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tfgngezj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wrwcload.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3txxromnb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3betzojar.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ntxoxdmo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqfcnkr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oomgqcmd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3uukaglkz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ykelrrmm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zwzautqi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhnmlezg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qadsqnoo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lssxsmyt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ewhlufam.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gfezemff.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wwcojsml.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fiyakpzo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lcottdtn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ghywrbmv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3uqwesufl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzoofxek.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhjzugpt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3weusixim.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gldaikrc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qbllkgdl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bjzdyrjd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3doibagsy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wguyrtyq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zspppbps.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uccjglxq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3upiuyxpa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3upziqctf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ukykjrxr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wzxkphgc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbzmivag.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bbkdjast.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ufadsigo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyxakfsu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3iavwmngd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vexiiskl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mtmlmwiu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3oscgenig.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oeqwblvj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xsbeboed.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3omjfelzl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wewsfdfs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgputjxh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrkpwjw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fcbvhtmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tcydsqqh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wogmspkx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvqpfmq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3khfxxpvt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ngqaqyct.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cckhlcfl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kjfjzlbm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3logtqvxv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mqxxqdck.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fdqizyyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3asigxjzj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3phmybzat.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nnqrpvty.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3aofzlfhq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yrxdmlea.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ohdxzpft.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzswdrl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3joiuzkjl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zioutzgl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ihevkiez.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pwlawlwr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yhjquleh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zmqwsyrc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xjhgcygm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vjshmirg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3djqmlbdx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cebfsiun.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ipisjcti.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3shbrueef.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3prlvsvhi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xbmovdbj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cqnmsjnh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3urcndxhv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bxcyqckl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oeaihdnm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pjrqhlba.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkfaljnp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dwpzkkjz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ajgyskfn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bupywicq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3azfblvtk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ocadhced.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3duwwkvyo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tournzux.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcirgiry.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3liuipbhs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3avbdqeiz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fqqkdqip.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sxinjmku.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3feitfoqm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zuegecfk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iuoqpflj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3usypzopr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3idhyftcx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sehytdtd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ksmcpuxt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sammjslw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vfpdrgdy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ythcznos.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ehfbbzbw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hglzwxax.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vnhsxyec.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3svcecgqs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pudtqics.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ekcckzxz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fnnzmmah.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fvogfrsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3celiivwi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cmcdcpeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqcblkwz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rghxscml.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mfwieubg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lbrkmrwf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qqpcyvkp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xidnbkzm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfyich.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yaitxjbo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwvirzug.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rdmhyvux.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cfhpyspp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vmsyziqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xjsehxzo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbpzggux.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vhogmgla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iezlyrxl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wfnzgdew.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zghhzmie.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgmnhmv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kuphccwm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ebylasjt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rmqongvp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pacujjzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3drpdcpdm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wrjtnsmj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cdgdtqgi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vajebsxz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lrvmjutf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ptypwxyq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pqgpooaw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3adljylwz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gpcbglgf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ziafmcyt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxqyenc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ijwqspuh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3oehyavnn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ccuzwiej.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xlugmevb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lrutsxin.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ikdlsyth.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ambkpufy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzkcyave.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ergimwyk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kijeumqn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwomroez.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvoufwqj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lsmvedha.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgsmbzif.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vxygxdwr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eczqypkp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3szqwdrme.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3izsccapk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blarnltu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqvotmfs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cpxbmpla.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3drxvjymz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3edcapgvv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jwarmlyl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wtnraczx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jzeddhxt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mwykqnki.html


<!-- 参考信息 -->