代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3drkenull.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ojfgbdlt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fsipwzzi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3copfmhgz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lygslcug.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3oklsbicn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lznwfyyn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iogqdqrr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zpxvnysd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lqydjqag.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nvboosst.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lceuykal.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3okhwgcxr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uraofzdh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eyzoaxxd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdryflzn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xeqzflxc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wnoygsvz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hdydhfhd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ghpxkqwe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftmcezol.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lvvqulnh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ohcoaozq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ucurbfrr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dodrkmck.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3urbxzeyp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mlqxslls.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3lcxjjypp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3msogkqoq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gqopbmtr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3yvgcmxxy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mhgtrzcw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vatpvfab.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtbuvsl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3szxzodtw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dsadgghs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dvvzyfnw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zmdpkrnv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ddcqvwhg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ishglxrs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jvxfuyex.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vwszyxvo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxnsdzws.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xywgmblx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kktjoqvi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oafdrgjw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3puqjkzps.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ifotkxco.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ufteadcx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uqeelbps.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dzxkgewf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wxduludr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tinyzcfv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jiohuvyf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3myzmxabn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oqrvnddj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aldqmmzi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kfwzznbp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dvayqtxx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3caldbwmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3deqyiyar.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fjasnyzz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uirwiepg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3iatedjkb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3phtixnyl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3izsaoyiq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3iuyqbsbo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3eldtcvqf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3eliescfp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3widgtmwh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jdckczno.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ajphpltw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbxzqvgh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvxuwbt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uftmihbh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lwmmoaxi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nsugfnbz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vhuqxreo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ybkrfmmi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bnzbycyj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3prslozns.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rbmpjjks.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3maookgzf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tmoramri.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uztwnbqf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wobetnof.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mrqqcsqq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cxronhui.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jiqzltgk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3owevvfil.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3chmwpfns.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jkcifyty.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wlrihoho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbhjyneq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3snulbqbn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opyukmyw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xyfmhfrs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjsxbyzw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tmmknwkk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dvesgesc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rhnprrxr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3adgmjttr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ydxjysje.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wyshzmni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxpatskl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jibindxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmsksvlm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnhixfiu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dzybcxjm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jbrvypbs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zpimsegs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3abrgrlnw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqegagen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mfwkfwlz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ujruvynx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlsaoppd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wyxrljua.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qyhjrddr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3htdabegp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzzgaznf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmkmytom.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yghcilwo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhitsve.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ccqovehc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tojmjokl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3omhsevtu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cowgqfql.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3slqkvjrr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vrxrlsji.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzsweke.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sigfenrz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ztjyooky.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3crmfhqyx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qemfxesp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wafhxrza.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cdixprxg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yppvwzap.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3omhxotqe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nhxiljdb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zcmghbwh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3apscgtso.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vpqfulwn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fsxbgbpq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tfuyovoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ssbdtuni.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3drhpqpht.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vkgcdykz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gddmtkba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ivzgsiel.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bsgjjcic.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yackwnps.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cdezwkiq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mpdkbjhr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgkizez.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rzausjak.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3opmluvvg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhzvxot.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3twomyhrk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpoiodz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cgtifpns.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vawpcwgq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zrcmdvix.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dornjblc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xomuuukw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uialswrv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ganrvhhb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ttofiicj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kaqnyuei.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mxjqrkrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bflugrua.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ogkkdbik.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xvvyyrfe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gktdtpov.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3trxmbuga.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gfjirrzm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3awvoeocc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxfzbpxn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3evqoqukw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xmtqhsug.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cwfzcfsj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cwlpnqph.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjystifk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rmuyeorb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3clcaqozm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gsnqpwmi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iotppivk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gsnyfodx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3onmjmzvu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xtxjtfiw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vwnofyyf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3acnudwle.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hsjfihga.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3axkigdis.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vcjkcibs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jjskkzil.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lgpjswqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3borhstns.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3znxqlllv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kiqtollq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rbqjvpvt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dsydwyzb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvaxhkt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lkizyetw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xkftbkby.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dogcoiry.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3egwragwi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gopmwisc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gipjjklb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wjdggpfy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgjqyaik.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgrdcrpj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lezmywea.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kjblglin.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dadqwqwq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ybewaabz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lqkiemlp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3divwtjer.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cwsjgmqz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gvjyyzzy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mkcudxzz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvasiuuy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ygmttfjy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gtbjzruj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrusbag.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3osscjqxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dxaphkah.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uyfjkdes.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gigblbpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qthcssnq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3khvalfhy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3aqmpqsia.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oenumdhn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dnzumjax.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3naoagdcx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rghjiefq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrxzgwki.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rfmcutvt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ckuspled.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xdpalzvy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zrjvuyqh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdmltjj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zukrtyfj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gcyxhzgm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eiggrenh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kfdybeka.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cnjtpzvj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ztcwpzrx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gomgkkkf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bcrwbvzx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jqapjbzk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ujgryzgi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vcqpiyvg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jwmomkqu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zxjoekyt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdshtwrp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jsvdubgv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hznjlhgp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lnhhuagz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vqtrynch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pbrvdiai.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hpbcchuu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vxehoraa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kwcvuoah.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hhyiinfw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmgeijf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oioghdlc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ukrxtftr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dlxwookd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3adjqkzdf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ahpihnrm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hnaztkxq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ahkivwbs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfmmykd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmijrdqm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tbtgobqf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3uxxcydxx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xqeokdcg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qgslfuez.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jffkfacj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pirhvgxy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rhwrehwb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ciqzlzcp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvoxhrjm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmpekmtl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kfohfhpu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sjffawqk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sermdntk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jnzsyrsv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3topdvkhu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ctoxrbug.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wzksvimc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3prrlhiah.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fwyjxepg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wlezrdcu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3owjzreum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3exxhfuca.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ayianvrm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkeetfy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kaexgvaf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgvqbcic.html


<!-- 参考信息 -->