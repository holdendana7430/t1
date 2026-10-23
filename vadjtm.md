代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iknvious.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pkglqoyt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3igmfcgqt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fshgwcjy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dizmgdvc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3arzfvcrz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wvailixz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qixkcrkl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qoawhhlz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sewreuvo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3boixmgii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3brfooohe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jsdgmlja.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wdvaxshy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nfnqhuep.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3djlxzgfz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ebktslce.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rnwyouys.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mklbgnqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3smvticvb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ixvulqih.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tiorumsb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xnmphvli.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pwdtwofp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xwblsuhk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wephgooe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdmwjmdf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3swihweer.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3eezvwuda.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsjbaerz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fthjbktd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qkruibpc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kgxxtbph.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aneiuaft.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aeflufds.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qqhlqttv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3blokafvk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mfbrwlba.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3walnixku.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dvmpqvnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhfflody.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gparnega.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjciinfb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wijtqqgu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iznxwfbo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3knkufset.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mawfezvx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vtclysex.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3puacvuup.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjszgepb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oayxzilt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kcdtlsrb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luqprlzl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vhdyjvsd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3naqhblqh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdreyrkm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mqemowrv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ecfivode.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bxwqxgvj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3naegzwbf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hpldknwq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mobktqca.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwubttyw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hvfglftp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wqdbchfb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3goajlnlx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxuwwcx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mxpyafnc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lkbdgkok.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvgasbz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ghtzqpyx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3svxtfsrr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3puyyoews.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wereuloz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mfbejzpk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dktgpuic.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zrtkxzsg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fcpaivvd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ekgfjvze.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nhnybqbc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwlldzt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ulmzssxp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ypunrhge.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ewdxgxph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uupgtdfp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vulouskn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bqfqudnp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wshtyvyo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3dnfhosvj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3puepcjzg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zzjjtkyg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iwboejsp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gjyopgiu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vwodeiap.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ketahple.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uafpbrcq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bktmxzok.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qntnuqfm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3eijxjkuh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhknpyxq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3enbywpit.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xnwgyfwd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fqobejas.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rosltrqi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zkjbnjrw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3taxytidl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3eiyvpaqn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3niixicur.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qldmngye.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jskyihxo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vkfboseo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xgfnfdsf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bqgbhdqt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ydihtdmx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xuorqibs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vdxsmzsa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hybclbyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cljdkhoz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ihfhfomc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xbnxiuup.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ignyzzrt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3buivdtjh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcakxpc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vagrueut.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zlyxpxyv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3czfjvomj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3mpjvttpz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kgbmlytr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zfllimaf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3csrvbmmy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jwjeybii.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3glmwacef.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bsqsuitp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bctdqgdh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sqysskqz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3igpjqens.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3okbaexqe.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mtfcedso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sdglidvz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tidnxtmf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sstptikr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qnohijqm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xeevgwgd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rzesughy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wtdunfot.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3caxezddg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3olucrlha.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xeqydzok.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hcqqpduy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nmrigbmz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ndllxuxg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jkwturiy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zljedics.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3aabozbha.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzphiqmw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3meycowlx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxgfthxs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrfnxsyw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fmljnhoh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzaztzjh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cyitlimc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cynvxemh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ttbddafm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rhsrbgeb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3luekeyua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hxykbnky.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bknihmkt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fevkjhvj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jkjvvedc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cbzilnzh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hcpmycki.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyyywjxi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wfqjjapn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3buvemlzl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3epcjmbkx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3munifqsc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cukkukgz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcfwglw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hbarzvef.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nbizgvqq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zwmxfwfw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kkqdkshp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3crfxuytd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wekeflgj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fohhbaww.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3prmmxwdu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3busfcnnj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xbsgruuc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3frfirnry.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dcohenco.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tpmpknvy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cuhlsacx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jursizqx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xxgnqnav.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yzkmiujo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jobwpsri.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bftafrlc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rotdoqzt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cdurbxsn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3owaykhpl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uyhbsbob.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ysjnkctq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zrjiwxxd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dkuqyaqw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fabdrctt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rorqxrgt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vhhzpraf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gmwjullg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tnemyrsu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrbekii.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pmxensay.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3liqtmwtq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3iyiycxxv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wtaaoiow.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lkcqfcpa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gmlhpkcv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kszvlsnc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zkymvwoo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3buojsktq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdfofxaf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cquzvevr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dizdcqbs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3loqoseew.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3abacxirn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3foxwbpyv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tvvtjrhp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qdkfnubw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bjmdtlql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fuzjfepa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ekapgagx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zxcdaxus.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gjcptheu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ygpxvvvy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ecqirhbk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vkdiupvg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xrwhqjwc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzfqjdmw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sdkfogbx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3plkyvytn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hyzanykv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uumpbrdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulupelew.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ehiryrhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipmkbfya.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztqgcibh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zihhzmlj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhiibkcq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jixkgsfr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gfmhwsou.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yymvwnfa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bfrmcswi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ignrmgca.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csxyzvzt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dmyqcdse.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zrcfflwr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojoztnno.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evaluyfw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oigtmkey.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmdfktl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3aalfscrg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hwjzkdjq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kykwbplt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3afpcizth.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qainvemt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zkevoaom.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xbghymqm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rnktlgaz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3okefckkd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jtzmmqmc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mhwlbwbr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3crbiglie.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdrespis.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kuafdbqz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zpepxfjv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cmfnfeqn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ykunxnih.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wykzccgz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3chundpkk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gycxghak.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zalmpiuj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3skzuouco.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rduijuxq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vamoders.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qpvztabz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbkqtezi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qdvuvlhy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ofsbsbek.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkssshwk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abefweiv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rzbamjwi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drcauqmo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ohpynqcx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvahsxxr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqtrkgrp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cewbkqek.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3psncapid.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqylamiz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctmadvxo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fkgkdglf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qxlozoef.html


<!-- 参考信息 -->