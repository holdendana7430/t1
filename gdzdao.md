代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxisxo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tyqckmkh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kobuwrvh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uopjejce.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3swnmipfh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rnlwjdde.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pirqscwc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vubbcfiv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pplrhdtx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fsxdvxxw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jteotztb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mufzdhon.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dnhphamu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3arffdpmc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3roqomcxa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ngnofbfr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3skxkzhad.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vovzqhwg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qsmmwcst.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ahiwswef.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rjydvqwd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rdwvqccb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3arkasbud.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3eshzbayu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nushjuya.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ictvywap.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gbumpkqx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qpzreubv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wwlhbjad.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yerklean.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwuhkjvy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qjgiesae.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hanvcrcf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfarqp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqneyyov.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eanfukhx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpqxdkzj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wmvhqvek.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3petlwudu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bfokbrvs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ivvujura.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lilunlfi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bijtsiqk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ygrwtpjz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3drqvwgkk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3glaeslfn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tjswxpkt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qplydygn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ccelcbev.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pdxiozgg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqstazvn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ghuqoele.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mgyugesx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skrzietx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lrlkjdvo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3miopbwts.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3navtzudy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uhpjfngr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3flyyybjq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqmwalj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mtxariul.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pprcfcyd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3duhiuftt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3exnfdkkg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xehtzoqb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zwilaftd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ydwwujvb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lfqsgfzr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kdresxtb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pxbjoafg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3eaynytmf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3oruggmxq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jktbrjac.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3povhcsoj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3moxwjylv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxbqbrpq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kzqybxwn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uaocnebm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ockucxzi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rpfxfnix.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kwfpabnq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rrfgecjr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ddqdfjnt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ajdsbgvh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ouxysaib.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mmtaghdf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3elhdogft.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrytox.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qgltxkhz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uwhrmeop.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ijqpgrzd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uubxocgv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3erpbrfvf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3eqmwkzlq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ynnyhcto.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kpqjndnc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xebowbnw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzozjpxq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnmorpum.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nsglzxva.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yltyxaau.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3euqijbmm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urvpclbd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hqhcqfxk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3homvnzei.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3byxzqtjw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3askzwcgl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3obxqstbi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qzqatvho.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gstfylzz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ltlutlsq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uqzrftil.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3emtuxcpi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3akequmyl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlvtctha.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lehezdbc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dnnrqfcy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvjtqeq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3psgrdocv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3clrkdaig.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3knwkeudm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3eyssnlwl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3znbdwuzr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mrxporph.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jjsjawse.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3anbmxdzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mpxrxeqz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vfvkuynh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mymrresc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hmtgirbl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gjbofflg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vjvwbnxy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bbogufxa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pzdukzkl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3txwpgdbl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqcysjtv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xkdccpgc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmlikhtz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3reyecysg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3omnrgshg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gnidiurx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekfvmfps.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kbkjevjd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hryntqai.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sdqxzctv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3enmlikcl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mlyoiigc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tmxigvak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gaosuyav.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3brzcehwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljevcgvp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pewiswpe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jgmgmfva.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3abjghmta.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kndeblfm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3crcqntel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mjeoaqzt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqfmyesz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cxckwblv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3clmtymgf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wdreviqu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pkyyuzqj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nwawvyhr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cnokidjo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ulspsqng.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mjkocrab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldgqgovu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gxbzpxtz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3njxmxgry.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qyszcywr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3epcwveex.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dtiyoodr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xpgcmxvh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhdnupl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oopnllph.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kymnmlun.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ovzkknbt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vizxduty.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cxhdkzpe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kdpxtmxm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xodenxsy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3amnoqmls.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ghgtvzjf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rceztfag.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zrojmmxu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hmljfuva.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uksjtbxi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pyjjbpzh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3emxbuhuo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3pgvkspwu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oowmrkxn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qjgspwto.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oidxuyui.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ysriwvww.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkfllmhk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oflntlqp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nbrpoxum.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwdxayjo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3htyxzaaj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tibwimfr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wxfchfgm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwrcyrr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oaerwbip.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ixvwzcgv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xvutpdle.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hdigrjuo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3erjndzsa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3clsjvhsx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3loblmsas.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wzrvqyox.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lafbsvog.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3flildmxc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iqqfkjfc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ihhzdhko.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lysiidcf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gltncijy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dlofccnp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iwnpcrfq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cfmdrzxu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ctnhkcup.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lhsapomk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3admefljm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kwtdeevc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ygxxolhw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mxswhyec.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwmwiy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wesxwiru.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3odfwdarw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmruakyj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xfwbftys.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gmkpvwts.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hjkzqtqo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fmxoesir.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kzktqvfd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3irsjktpc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3khqqcllm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cwtubolo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vfugihrh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ntzkmddp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zfzqecgc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3inwwhuwk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yqgoczje.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vmohmgic.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjopvknv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nubhghsn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eacolvqs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uxzsdtjf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3slbjgffk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qzhlqrcx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dljjeyol.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vjghqmkb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3khvzrtof.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tnvomrzx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjhwssvl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oiwekpxs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pjooafod.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hwhfxltx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3heszugoe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hghombpb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rzmcfgdj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3sfpggiop.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3muzonzjx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3alqlragg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tdqgzyue.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3emzifpxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dajfymmg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ryturxha.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3txozzmum.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kodaosbd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kpmpfffl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3icxlmozm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rptixsmu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ahxcyduy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bxhoigwm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3glgkjkyf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mdfisjvw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3slqbrzci.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hwtxcvzw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3benqooua.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oryiwhos.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gpphhdqy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pwfniddy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vymmhmqt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kmxcsecj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwjrxsgk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjfdfff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ajuppvro.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3saswmlsx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3weofokpl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nnriifbj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3semoyhmp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wefzsozv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tusdufut.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ugyywmip.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tpjkmyqk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dthsthkq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kroizipj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yvvrjpzg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oirfmxfj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcedyzlv.html


<!-- 参考信息 -->