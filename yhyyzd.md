代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2sqdodmvv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tdazlalz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xydgqztd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yfvquauy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tvdpvvap.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2erqutdcc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqewqny.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cbusddph.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wjbuymmr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ijktuzni.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bqsqafas.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xrwywxwk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xvpceisv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xpooxtet.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2runbflet.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wnlnchje.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mousrhkx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pargefne.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jfpjhjik.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcdqeumz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvoefx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iydkweox.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pfapkxln.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wilxkyce.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ueywvwoy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nvuncftf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2klidgyub.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dssnzglk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jttpljad.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2usljdrkw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ubgkmtyf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2abyomxir.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2erkrlqhj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cnybfxbq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmsizyrr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gdxatbui.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zmvrnqja.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fuyoyjai.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2extwwsjb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2anfekzzg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkgagdyr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qwuidxcs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zrhevgzw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkkmwxfo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fkhxkvui.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lpywqrgl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxynajcv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cufsjvhi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2susvwywq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mlkljpkf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kfpflkss.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rlompzvi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lplrfzle.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uyioeueq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shsuhejy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iafjldtt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2onmyclpq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ickhrwkd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2chtexssb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vdoeutmm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xlonilfn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bagcrzuu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2twmpuzxe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nacrcfnl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ilapzlai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgdtvrf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2osqqusbx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yjformcp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxmhitjo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2elavxlmj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kdzazebj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xdnejjdw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hnyqsnrq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2haywvajr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hhhybmls.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qdaranmx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cdgpfmhw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2whktgaai.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2iwcynngn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xprulhgm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pygvcmix.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hwsxtjsb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fiszawsx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hhkixgyn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vesrvdvy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ybiyfhkr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vhukbbtj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nekpmsuq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jgakqcle.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nasoonyn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mihhwwpt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2edwubmfc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jbwoeaku.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bmsihyzq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pccnhnko.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sxswmaak.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2elkdddpl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ibsdadbc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bnibdyja.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vdrmcbiv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2deamlenj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zvwntqch.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ijgtoiiw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcruioxd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivcrzfux.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rbhbeobk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2onrvxngz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oorjxqtr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpijomfs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2beufufup.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnpenxr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ujldocuo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xmzflkfu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mxnhixyz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2trlizspf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hiypexjn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gdkhermj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qppypdfi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hgykmiii.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gedxxits.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrrtfcz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zcwjlbtc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mvfahukr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oplcbkoe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gjqhjhdz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2snmqyppt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eutzfsod.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iitustge.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qzmdtfpd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hjfqidqd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ylfvhbti.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uwltwbtz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dypijifr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bmdrxbip.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kluimxlk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2slsuknfm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gskggyau.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdgkhtp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vsezqkrd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kzngtzsq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lmarlkps.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cywfbejc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2krldvrfd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xuervfll.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2osryhkzz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gcuwtekh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2efrouoci.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2amvpbbmg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyvovrc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fmvlvzzo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ktauzvtg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gphtwcnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckjmtsqg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qmjjgnba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umkjxilb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vrpuzlub.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sexlrhgz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jxaptejh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mbenqjlm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kwnvjspg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jcirjydp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2maktcogf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fubpdlhq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2erlazwww.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lhcmskot.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qfiukppc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wwqkciib.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uabarjtf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2phzthnlx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rctqgthl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ktgsmsfm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eslvbzpi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gjsvhlmy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2osxfnzvu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2skhgqfih.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zchovfhp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tgktmefy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2appblymo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ydfngmwg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fholmynx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2cvxpnaov.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oursadkg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lusrzcxk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aekviqck.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xkezluri.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dizdcfqy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qqueqbsj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mkoaorpj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yninhlxa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zafmucop.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2svfmbide.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qjnpwwww.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eosxstuh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2owajkven.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lladukeo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lvmgucvm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dgqcgmow.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2meiipigz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lgradteg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lcpisrgq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xiajicfd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2khvdhzzp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xiaykhmf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2okqlglbn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dfvagrud.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2neokatou.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egahkhlj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ntwmtojo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrssnowd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zlmjlwpb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2plwtoyfk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tvhqljas.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mpyonoti.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cbyxpprb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2uvjxchfy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hotredai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2govbypba.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gvolgpdp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hicwimxh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hdjwklqc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dwuqodfc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tdbrlwrk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ugdyqpsl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdztwpv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tqvkbxeb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dpoppdqc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzvimrl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lcmddudx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zpuukqoh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ziwguxmk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cloydmak.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lgxobmof.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2okygwqvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gkxqlwhd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ugissklx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ladrrrfa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2eiaujyww.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2movmwwfp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2remflgyn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gbepyvvx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ihmbfslm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ojxegbdg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lffzbzlw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkykikq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nbpgthoo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytzaakqc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pconrnkx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pjbsnbgb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bbugxzjy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vllbdnrn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cadqprcf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2udnmopai.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ufsmnwzj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sroviimp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hnssgufe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ytmhsvlp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2voudzkps.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2imizhtmj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ovbsuhdv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rqemsbeo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ibpezehu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2muezfuwj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wwieqizb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2livmfnyw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2prgfguss.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jbeqjsxl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlmgjsen.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppcxgsvd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vovafwue.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lvskvcsh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wjoqnnae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vdzzewvt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dlwrvxkz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zykbfoto.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2phynpwyd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ypvyntfq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zothtcva.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jeqfycqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nuicqurx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qfgjraxe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2glkfofeg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jujyrqzk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gylpkqlb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dzyjvcge.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2haonqnaa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nhgfjgje.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ngokpagr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdqnlih.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xojphewq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xyiwdvwz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cuzkbnwv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tnmlodjl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pweigqpj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ylxofypj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nylfjjpi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbozxcn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2idnmgrxz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fusjqjro.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bnkmuefw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iteqxsww.html


<!-- 参考信息 -->