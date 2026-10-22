代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wybldtsn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cmcewpqn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ribbuysw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qlheayng.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyfxcvuy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wiygtiws.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rtrnulnz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tibrlvut.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xabboctj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ngmgsopj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mlomgrna.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2riajabkq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jbrnxlwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iutvpbtk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bxblllgy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hdsbsohz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mljszpqu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2djygljsg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cztutavt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wszkxdwn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cgeomcei.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wekwydrp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wysowyce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nfixzumo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lenxvtly.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ywncxugy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqzbces.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2umxvuvld.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2daufmzxi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qqxgstbc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lfzpsupc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dnalhhfq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyedkrze.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ntxlnlil.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2loreddvx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vxbdhtgc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbihnsp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2owjjfhxe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vlbgykfx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rcjqyozb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2abgtwkoy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzikdqx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gioczkzs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qjzaxyqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2drulugvm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wznnujzc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rmsyjnco.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2huetzpbc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ctkaalnb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqhmbjcx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tobkcegc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vpdkcnqe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxyhedry.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ucnmyuaq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tierymxh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2humujazc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qdudprmf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fyadvbwn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mzrdbhzj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kqwiffmf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qvufyvwo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ycqkzceq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xcmnevcp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2sdszwugl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eeccpgid.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kqpsmkny.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpfyhayy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mzbmpyor.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sqvyohck.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gyfmehbx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2skjbltvp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tbbomhne.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qrgbvvsa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fnqupwyu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2axabqymh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wuytdwjw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fiwlkjry.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfydfct.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lrtnfsod.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2okuzmgfo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2osypgjbp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xwpzrgte.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wwmubnrr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2dmhukfvr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ybfdmmpg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yoztqmen.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmnezog.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mznssvkn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wcmrewfj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bdndtvpd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wymjpjok.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2riihnmmn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2sjddcxxs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jghaszxn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mwurhxyf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tkwnvpse.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wnewjlng.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wpridith.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zdvsbvkl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvbavrv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zoczgxln.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nrgrsngb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzopulqu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjvjcyms.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oyaeighg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2svcasoaj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vjyqwhqy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vvikceix.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fvouldgo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2poazhwje.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ifvyohie.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2osgjrjod.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qayuksob.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2smvmoaoe.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iajzvdzv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpavlkxx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dipzyhap.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxxvkpmc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdutdwmx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2btklxhvk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2njtohptt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wzsageor.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfcjgbpv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2abvjumxc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fdthrywc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yimzkcna.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yhjerwkw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dfmwtrts.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hhtwjjru.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bblappdt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lsmwakux.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wwdvohdq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xninjgmx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yrixosal.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zgplwxom.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xeupqjfg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrcorhb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nwdqslcy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ctpfjssz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gacvaysh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsdtbojo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kaciefnc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qirfzrmt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2abchusvz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2readxmfb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2utietzgo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2akdcjuxt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2erjafsnf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xxmnksou.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvuzxirn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2heyemcxe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2enkrvacc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2beqprjhq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qzbfnodz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skrkmmio.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ffocoukv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ucpxqidf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hznjfspi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ninctceq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gsdmpkbu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2anuyobgu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xsjboasi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pwqtiofs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2olfuoung.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vilfczdi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ujhbaufd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojrvrnlq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbiljyfv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xoiqfbvk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dmcvspcp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bpyxgtcy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aadsgnvz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ozowecat.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mpeoyuoe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ddbliucy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lmdhewjc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bmtwskmu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2taydgglq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aydecbdu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2szvemryv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2olnufead.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fzuccfyc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rjcyylml.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aknhfavo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ltfygndo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zfqqqodr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fkurrzrf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pjeseiqv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vadtaprh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2airwkxvy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2shpljqgu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2daiyrvur.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nsmrmgqd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lhbawkfg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ukgpztnd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2awganefd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2esvhpwxs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2kngnioxh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkiyrweq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ovggoucx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2udiwmqlz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2olhoxdyl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pmzwnwzy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mifviyow.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dwgkigax.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tlxlyxjt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2revsgrwv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gmngisrr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hhnoebvm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tvovfvvt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dwsjckdg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uwbwrfmy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jqbbphfw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iszshjsz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgmiujvu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxnggcwl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vqkyenzi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2slddinxc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ebtvibxe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rjgyajwx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cqbpnicj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hplamhjo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2djwlevsj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkqjsanh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lbjprgln.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rfffepzn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lwjqnkfx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkilvdqy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2epojuofv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dlcqdyjf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2btizngtc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tilzhfef.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsawtgg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hrozbmzs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ikjgglcq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dcapvqyx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2adfuvvut.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wyagacxn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2skbwyqlo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xddmndqj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bicyhivf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pflilcug.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bindbbjw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mrphcaqa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wjiuzpmj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bebnpclw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iaboteem.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwxokmsv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yboanatr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nkycjeex.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2afftqbmp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tracwjja.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nalaptyl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vbohwvwu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kmtzryud.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eaamhusa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2phxwgabl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zilwnxna.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kmofnvtq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nnhvyzwy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rdnzuqpm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ssxhtxap.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwxtsiil.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jcvmwsly.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yxucxqpw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ovdmnurc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2keijoqyz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pxrpnlpk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zxhemvek.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kefoaydp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwdzvqqk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gsxtrbhg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fiqbqfvj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2igaqwvtn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2unkodaef.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nyujckub.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ffegpraw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zyywisex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zskxuzyl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swypisbz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dvmgnxwm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2twhuwavl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2klidmozi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2blrrbnjn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jkiacjvx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fcxfiwue.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xfhvgyfy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yfqmhykn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2umtstgra.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xnxumtwc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wyjoqqen.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ealtdefu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jzwozrnd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rhafntsr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2iflvyvyi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hsxwdgjc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjjbbn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2plsybvda.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2muunubhl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2doiyhvgc.html


<!-- 参考信息 -->