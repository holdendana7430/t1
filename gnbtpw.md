代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zvatbryb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tbimnveg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3akxankwa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tfhyjjtg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3etksjjku.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oaslxazt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3irxgcdxi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mzkxaavd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqaqvyr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3elcxgfls.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3infworze.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hnpxhjbn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qelslhxk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qshmkrtw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mfgjskny.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jztxzese.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eewlpfyb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pyppjgxo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cxtozxrw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jfgluxjr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qlvxrmhj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yddbfdmg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bmkfritr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rspwhsjb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fqhtvjlm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbblscly.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nwfkcnow.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysikozdp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wfhabyho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3serbivpa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hnbfxoxw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvjytvmv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kbcydzvy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxzlwpxl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eadllple.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tnqiiuyy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kqwrlqzg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3crrutyuk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wdjsdfsc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dncdepmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghrwrwja.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3thghavdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzridqog.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pwjwcsmk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hlwgpetr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3boqkhpoo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gidoaidt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ihvrkqjw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3azjmqrwh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mptlhqxv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3whedhjve.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3isnweyua.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjicwzyc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bdndyckr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3duvryccf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ivprjjxx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wstcxzyt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3miuvzizk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gumatgus.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dknzplwp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vkuirvdi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wqjhijdn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lpjfioiv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvoxiygt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dajwjgxu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3njhjpway.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pogsdphk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qmsnxghe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xstmloyk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nicwkzyw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ukecmnxu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sgkxnszc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ffuqkgsf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqannzit.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hvajafvm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mxtkiane.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lxcwvllz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jwwoojgy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dyybehev.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ckbxccsr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sstlelub.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nemazqqu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nqgkxecw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qaocobtt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hujvvtsl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fydvbisj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wlryulkf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rxqlqtlo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jatmhsma.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tpjlvnrg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nurvfjcc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmxxpxxi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nszuevly.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkdksayb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywrzdecd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3razwdslf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmbvtcco.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yazeurbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vxgoyted.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mjarlife.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ndanotdu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xdrljomi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xockjhfr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tkagqqql.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3betlrypg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3flcjwain.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jhrtlurh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cmavccsd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dwpwrtfv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3whqojhlx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ieubrqxg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jstgzajo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3omtxygkt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bgsyfczo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gfccdsge.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3edrffowp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hksvtwqq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmztvpvu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cquyqjqo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rsrxcanu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lslhoypd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yfxrgdsh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kgwnocpi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qezulelb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yhwqppjn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dktaavhy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3idsspfnu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prflfysd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xoqircmf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ldthxnjb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kxzpxrjb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3krocjjgg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vvbktfio.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gndpsbzd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eyyhcfro.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ouhoftmy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rmmkhsgj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mycmmhbp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hbkwardb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nyumgudi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3swqqbuow.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3olmwchgf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hmqvzudm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tzfquohj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xrkiixus.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3comtyqxo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iwifdapc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jhaiucdp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cqdgruvq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dbcpkqel.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zdxdliso.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mjkovncy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fkicxwee.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rbdllvjt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3apfppdmx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dxnbsxey.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qkclcrem.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wczxqhje.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3oqsrtrvu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ozadlfrm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tbvmdiaj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jvvhfoyh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqtubkq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cftcwhgr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swpkbntw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dinaobzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nlfjiumf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pwrobahz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fhaottoe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cuslpphh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jishxyuc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktjkyvos.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcyziqfl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bzcvktkx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pesjzjci.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzvvglnv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mbxlrzgt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dxftkpho.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sfnobhmp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdcjlrdg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gihzblbv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3abutawsq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zxazssop.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fjoolyxd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jvzqysbo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bamzbnew.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vsgwvbvq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3aomykgbr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3upxawpzt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3malxzbuv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lemshtkx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyeztfti.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ibbitlum.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qtpdcdth.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3soazviwi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qduhxuwl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzkqexzp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nynlrolo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qxmroosl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qyybxsuw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kfkyzxxw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3guoscawk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jcxmtfws.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxllbwhd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tultgxze.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nanmyemb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ffkbcypw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yuypybut.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3grdawkzb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3knoguqem.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rxqziyxf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cghdmdeg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3aegntkmi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ekjgyxig.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3bocvkccr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qsyvkbwn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ccekyrrn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wivozhqh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqwfyspz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mqdqogbw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dmbjtjhg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lpjgoruf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyybyqli.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bhzhuzke.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bcnjulin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jturnzbi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hlqxdztb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3htznzlzc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hqeplohu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3smsibyhz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ouyebpnl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3agbfnxjx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vysdngze.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrsywqcx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qwtlbzot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hveilvcy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zupltapw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iutszmiq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pznpvoqe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3beumfqyb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qkrdaekd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjxkbuli.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cpagwoup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xctlfpgw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3schllsjt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ipbproih.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xopeoxwq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3eexwynga.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3obtzqfuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3raivwxqg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qylxophb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugvutsiy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ioykwnwn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ijpeayim.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lslevgkg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kziiimek.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kijfrout.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oexcbrre.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xblhkcia.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfimmptl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vzmrvnww.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kfwauqbq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cegbftcs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xrykqzet.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3moavzmsq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gwcjbzty.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ynigfglv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wamtjeht.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3upwulftl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wcfggcfw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cvltgnzh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqedxuhj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3trylodaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rieaoaxy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lmsjuqxo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wathsdhm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ieejwtiv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ilmoxqoo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ewirfcfs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fqvorhje.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mzuiqufu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ziispdav.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hyzontea.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unumldzr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqeugfxa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wnycjogn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gvlaqesn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usneurwa.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3paduhxkk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtvgsdgi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkszpcsd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3myfdrtsz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuqlpinc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fsirniqc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwusutma.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kevggtwx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nacodqiw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lpjxxzyv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sjoncqql.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zwsuaawb.html


<!-- 参考信息 -->