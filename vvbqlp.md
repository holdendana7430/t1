代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wyrfckpv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hbmaizfl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nhbgjzpt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3besqrlsi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhxlhkg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zclqvobz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3phjegndj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jtvfdyuj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cokbxclq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wrnhyicb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zceotuxh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trxkqjok.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ibwqpkmx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vtukftdi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gdvjhsva.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fudgwxib.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hnoxawoj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vvzivsqv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gmwfavxh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aparhchi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mnmfjwgc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vethythi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbmzygx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iozittxq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cuzbewwb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ljendqrb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrmddxsg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uoiwvmrn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgorgxrc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mjnywtzy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwkjawug.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3srztffrj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fzcxeszi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3leqpvamd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yrysagrp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qxrgexfe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pbyurnyw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pmdquwqs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3neolgojp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbivgrb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tdkeoppq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gmbapvgw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gnxqpumw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dmaljaen.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmtriccj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lbfwesbf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pxnwgnyk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dyantnpr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3eygxgvad.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vlkdkwto.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mmiftusk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ythoglim.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ozbqtcnh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tejcwhgv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lthridog.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kozglxjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3txcguhlo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkxleqs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3idmubgds.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3syddyohb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3otvhzgyh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xfdugtrt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obvuwnzd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yjlgpvvd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pnczuotr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tixissuk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ceyswnxq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bbxurgcw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zmboekfk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3euzwdbfp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3avihakbh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ofpqlstj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxwjsnmj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yqlgtqzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oeirulyo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wlxjmgtu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nfvmqvnw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wbrfruzo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sddjbbov.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bjlkzwkf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcxspakf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yqllcvuu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wabgodnz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rrpqmwaq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njyhdqzl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rotituzn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pspahgyb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zhpfzzuv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hxotjtqy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ucskuhkm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbjmqipg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zjxwqsaa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3khbckwlz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jirbmoub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tuztmlip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kvgvzunf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3shvsldfs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3unacofmw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fsnpnhbh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rthogica.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rsbgmrjg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xizckmox.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3diawrbiq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jpuptzlf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zrsadsum.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nfsqchvs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nzzvyxlq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tfcghnhg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gqqrzzhz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mgsjbkvr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3niqqbqdn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ojgwknzt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3parnahtd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qtylyfma.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nvigyioa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3udfscbin.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pdrgvako.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mpazqcdw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tncmyauk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tivheueu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3msvuecrx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hytkboxf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ghuqbjga.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rkzvzrfo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gotdryvb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wezjnbzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ajawabjv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eyxohuey.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3acyoghyj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zcecwfit.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ksincmnr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dtuvemai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ntxneyoy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ggrrkleq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ntdpvuzj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oduileua.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3daamnoss.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvkcmjs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cznsmvxs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrippbn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fpiuprlx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iglopiqi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kafielbf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gahdxmdy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zdoqixur.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mhtlohii.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pmhjuivn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cnmrnbfj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvgkkar.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3maadicti.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ghiniapc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txsgvjrq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vixqiwvn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3inqezwym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nrtlatbc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3stythzoc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3deeizmiu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3otgpsmer.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3udhhsooh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jqclqubj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fqyebcpe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnouhjc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zkuqbseq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkaehhp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bxgshqzx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mebtrjcc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkwknwyp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ykxoejoz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nznpsxbg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3erspxqpz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qrqzrazv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vbnjbacy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pwawmavn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xtexktgo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vmhvetfh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mcujbkku.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3exaxpzfp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vefeudxo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ivqljvlx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3eeqctfuk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fowxpbuu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ilmxdrhr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3axdqrxac.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ydlexnit.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3osaoflfg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3finzcjzq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rfvkmuod.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjthins.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qapslxcc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jhnporkq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hhepklni.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yumfrvot.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cimplsdo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qswjpbyz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mtnvpxpr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3iudyciha.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxwsvbij.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mshqdaaj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vpgnmaoc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3snxcdcmn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3siycxnij.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uunrpowu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gckqkpsw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qzysysib.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lytufmww.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rgzedeou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ewpfhngp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jbuwuvuu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrccncd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nwylikkp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xgvxiykt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqtrsusk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jrqcdvyv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jqxhmcji.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mtmwifmz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iscitrqz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3imjtcokw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3iaxurauj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zglpdydx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gyetetqi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hgfmcale.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rivasdov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypyhvwkt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxtkbxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jqdqeghv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pcnxnlws.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cpivqetw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zyuinshq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3oxxtpprx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3udfnfmqd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mvznsteg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3flkmsfbf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zyutltom.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xhkvioab.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfdjuwa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aqyabqap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eratezpe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yrnlqjxl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zgmetdti.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfdewywl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zhukyjlb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jjwsdaov.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuldzlwj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3znskuhuf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jtpyqhwq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mcfzzugk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3elgpjmtk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mnxgmkep.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xhcppqgp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaosfqsw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3akukntoy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vulyqyes.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwnoqlhm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tsdazpxc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjhbugzy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lnoaybxq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vkimidsv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yrbedcyl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kkmajbfl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ftdppciw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bbuhdbyp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tgaxqabn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tyhfhxmc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3anvimtoo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hpldcnkx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nybzhzhp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3knnvzsox.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3calxnici.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qoowlxea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tacwxipw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hqqmxapc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ybfcewlu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fcxhmjve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmbsmoaj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wrtqfvyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pambusaw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zazxlnhz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lyxspuca.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vvlekyqz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vigfzakq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ipzffgua.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tvszpjqo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rirzzqoj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytpzzvwv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nooppwie.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nvwcrtxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gdpzcsus.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wqklgybr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnhlrfzj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mzzwxxmw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3snxggppt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ovysebbf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sckskdjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pavhmefa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ypwtoywn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3elkvopch.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qofrgtpq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3blhzqfop.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qjoydwdb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qwcavajp.html


<!-- 参考信息 -->