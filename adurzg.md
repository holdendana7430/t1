代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3agmlnfoe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jzbvxiaa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vimajwuy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ocvemliq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lfdvgycm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vjwzfkvg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nweskgbp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztvjqgcz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sakhjpda.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rtorvolf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ezlrrylz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3phppplen.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3snispsrf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qycofsfm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ftltcpzz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3yyliwlfa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lxfaqcdv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xledfjyu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rsrjpgmb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bjcyvjnm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wubvovpj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3peaasanu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3idkzzgtl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qnthvugk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xbqsvapq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wfbkyikq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uwlhtfja.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3foqyrqos.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rqyqbyxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zqfjnldz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dogcoczz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gaaivlmv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3epbhriwm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3neverhpv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kqzkzmak.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kzktnwgx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfqxnni.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pfxkecdv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pfmzyxwh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ejtvgqab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saoldnbv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uryrhono.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwuyttec.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avlclfhz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kixcrizw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xaovvvwn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eehsvqmi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wjbgdjlj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mwrkrlnb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3srazrywh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3stpkoidy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kvwiqvqi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3oxdisyxr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rdvytbgh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rwqmkitv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3txrogcek.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3agmioqpw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3plefompj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocskutjn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3eoivtzng.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xmgpyfdm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3edvaqouo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pyryrfxp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ltdiulhv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3efznqivo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vqanknso.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kijnpzxz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tlufgxoh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ochlscwc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zcjcusry.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nnmgfafy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tfjxwhgq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vjawrpfk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bhybedsy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nuuirbfn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rdtxjjin.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nnbrvwmz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sruhjdwx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3drdnasqf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hzetxqhq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mknzyofn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ntexyeiy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3liryyjkn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pfjdluow.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3exfaqwxn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pbftnueg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nibspdib.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kldbpxjk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3obpmfslh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ogvpuclc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jroeiwow.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fjuzfcat.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pabuewra.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xytcezop.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qthwzmpi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vjmnhnpy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vmzfzwky.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rvvfztmy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tprdqpyo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjoxngpq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3clhahmpr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tmusyrcc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xpislaew.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3impyhyia.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3upukxyup.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ypsltzep.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wmjdcotw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vjookhzm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kewygmmv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nvrdqvyw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ebjtbmzp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zanfbyqe.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wwozsnfh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hjetyswg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3txtqkpjn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ewcoaqjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnoczfx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bmsmjore.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3largssoh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3idqvndjb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3evjxsfxo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hqbsnktn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3raxacbkf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3udiauson.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wysbetmt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xsjybccm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wnjbaulo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bizwnqno.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nbsoqcts.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tsffpfvc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xrhpvmyp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dcfzrjpc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nrczlibj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luphdsyg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bfjwocvh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jzskoyfx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fzilbhnr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jxoqoofm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jdlmnhtk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qbqlvmzl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gaomzntm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kljrxwaw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xaybtnhx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tpxdcdgb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wxklawao.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rsjmmilq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ahiatjxj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3egzltiia.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ijwufimy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zrgojytc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xbhtxhxk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qdpclbok.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3netougje.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3haikoyji.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qnzyyama.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yiflepxy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebphqfde.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zfdisuat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zmuqdxwa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mhtdnrvp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zgvivtyu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jsbaivfp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvpetqww.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jyvetfpc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdgfcly.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqmolsn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vfwvgxop.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3amsjjzgz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jpjsweck.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gdjdmabh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjawdkc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tgnfpnth.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qfzfxrjb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3letkxpfv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3djyiidfo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3slsdatbf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzpidqed.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3whorsleq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mbjprwqt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mstopwgj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rwdmikkl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jngjpkpi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3srhyviig.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vqnkkpgp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fshgycqn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tjzihwqh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tvzqdtzj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qgtcuzju.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bwxqavzu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dmahmiaf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cseiyuzh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ygdtpaxe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyuisqff.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hfmugdpx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3drjukkql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ixcydydi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3azyvvtsx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ukkchuzq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bvvdvwgt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tepjosub.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qfapomqr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qituyokz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sdgkgdem.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3utevkqmj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mtlbmoxv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zcbpdtig.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bvbukxun.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mftwckun.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wygdcabq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xdtdxqgs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ejviykai.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ycvprntm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3eklwiyka.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3suayibma.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xlcctneh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ardkshgp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zhjurftw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mloxayzm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nysotclt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qlyeemeq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3uxzqxewc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nltrpxec.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vurgqnqs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ylhdsvmr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gqxfwdwc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lqpcuuzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpzjtq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jjifqsau.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gecciohp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3aupcnahj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3snyehccl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ukvhywwy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fkczhgny.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zptevdjs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vwifvygq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kwndlfno.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wzugjnsv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qzcznugq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3keeuddzg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lvxqzcto.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3drpxlydd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxjicaen.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qzuqtoyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjzwftxo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3racoubhm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3otgpbyao.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wcymtkhp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ltcnejvo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dbouslfw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mqolzwmz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kwdayqwg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmuqolta.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yowuravt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikmbwvrp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qjdlfyiw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xrbpcmmd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzndpqwp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sebuuojo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rvnhavqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpsnqypf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3smkwhgkl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcdlruya.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bojjazqf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wfjogqmi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rczktazh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jstcjlof.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zbkrxetz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qiqvgtln.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jhjdzptv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rfbdmteo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lzedzieh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jugzwngr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3odplakhz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3khhjidnf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rcosfyvx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wxagrkvu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wamcfmon.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lbxdebcj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zgzwrers.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nkhibjfx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3plvtzhzg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sptsrbdg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hhtkhpnr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksanhmfz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljlzrnvf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3afmyjrxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ctxnjkmf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkcfettp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfnrrtjy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fxqnkqtw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3haszydsh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oelvyqxw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqnfmody.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usshsclg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcdukjzb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmypcsgw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfjofrhk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tnmqvehv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wugjihqc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jxanakvb.html


<!-- 参考信息 -->