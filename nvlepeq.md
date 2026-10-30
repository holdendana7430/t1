代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghdfvuqhe.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/guuoyjtgo.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gvwqtbbrg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gtychxjcy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkbkjtfuj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gfhslmhrc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gvkvxmboj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gugqwdkca.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gazmdjadm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/glaaggnfo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjrkxdp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gqlspiovt.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gzouybwhi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gbddrwcft.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gfqokveof.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gimyvwrmv.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gynhagucd.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gooczzwgh.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gaqvtvyau.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/grzjydwnt.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gwnfvltie.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/geqdlrvdn.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/givpoxlna.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwzldwm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkqbutmvm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gsezstzvx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gtmxrpjav.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghnlwoptt.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gczblrohe.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gqxbsipny.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gvffihnnz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gnasappkn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gpquoudct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gyeskulpk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjnrktyhk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gejidzzei.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gvrntgdme.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gkyujjjps.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gngiejbmw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gtnyruffm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmcmdfmhh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gmmnwoefj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/glzjcbgte.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gnpqdptwz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gtmoqzdkj.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gnxykbkmh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gytuejryt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gzrrbbhws.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gbdywfeff.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gigviojne.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gwjvfgwry.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gbhlhocvy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gkehodhte.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gxefvebbc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnrwifz.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gunaxulam.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzpsmhcle.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/grcdjgrxz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gudqyaotr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/grmfbafsf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gpaiamqhf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/guhysklpe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gfnnccqjx.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gaqvbhyns.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/giskwtgfw.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/geebylqan.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gyfiqhjuu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggsdpjpvy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gsoyodbnz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gftoclaaa.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gjzsrjzjh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/glzsbqwsc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/guztatpif.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gfmgodpul.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gbnvnganb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gorjgiqck.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gjjqnruah.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gfqqoinuv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gyywcepgn.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gxxxpmjht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gdtolejpw.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gokcqrbtx.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gwtmifbbw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gxabmphgi.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gkherpjmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gkhwvffin.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gzytqastf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gdkpwwzut.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gmxpxvzak.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/grzuhyfrj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gpssisjgb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gzrpnzccf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gqlmxmofy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gebmzslrg.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvieseugz.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/ggvjtemvt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gjhqogtco.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gifwpyldr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ghzessjco.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gltxxomyh.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/ghlnyopjm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gzockjbav.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gboofkyuc.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gmhdufapp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxhdizleo.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gyiadhmrc.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ggfaeieyt.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/giozjamno.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gidgzmxpi.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gujrptgcb.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gwyazzfqi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gwnikmeub.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gaiwidgnf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gncswdash.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggwzzwyza.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gnyblgnri.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gdhdddbnz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gzukfwkgh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gxfgzivgl.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gbigmwmyo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gwsqofntl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmrvvcrek.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gkapbnepr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/grbkmqcrs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/goazygwxw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gpcwdtuda.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gtrydotsv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gccevwzsh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmrzykan.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gxkuhwely.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gwelburka.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gyksmsyyw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnpyymqdo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvfvoawjk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gtlivukgs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gnndydkbt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gsofijyti.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gnlbofypy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gljmtotzc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gobrxiqpr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gzvydudbs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gjesiruiz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/giqsczuxj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gznkjipsa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/ggttybyrt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gogyvtdcn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gavroxxzk.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gvuvqcggp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gdsspfykh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/givvyskdy.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gaywtjenn.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gyihqcckv.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gjtiiyxgi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gyypkypfe.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/goezqyaal.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gtybplhqg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnohqfadv.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gjzicqmnl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwjzdajkr.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/goljwregr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gbvaaweuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/ghtcqcasr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gmozupccz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gifpwnvoh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gbvjzdcuv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gbqnsbhco.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gaqpaamlu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gyjoqqygs.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gwmwsipfz.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/getsvspvn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gbkqjayqi.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/giodmqmhv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqvlwmqyy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/goyqyagyq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/glmajhxzw.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gzpjrjdik.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gnaoyswsk.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gwnipvocu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/ggtykceox.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guzxjdgod.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvxdybsdr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gnzvmzyag.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gclswzdlx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gldfrqejf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gcidjmlht.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/garnmyqwm.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gmftyuehf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/grdphkyup.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gufedcibb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gcxyxodgh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glzzwbvrc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gufhuccck.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gnriyoioo.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/giajyrktd.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gxsbkchre.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gzaahvkxw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gmdkhlbip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/glntxgjup.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/getxhtcab.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gnrvbazbb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxeyflbyx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/ghngfkgcs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gtnxnwyyv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/grryxxksq.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gllemljeu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/ggrhdbsnb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gbjedajvp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkfvxwpig.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gydtvsqpv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grerbusai.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gomyazund.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpblnjjxr.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmzunwlew.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gqdpivioc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gjykjkwjx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggkbidsxo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gtyieurdw.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/galjlnnxn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/grlbeprbb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gjfvbwvbg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gfreqdsjs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ghphdxpie.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gmqbjmulo.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/glihbqtsx.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gokyxiqvc.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gpncdmtkf.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gqgknjtyg.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/ggyebukas.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gkzktwyti.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwzmoirww.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gkiitlrfh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gwsxbrkxr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gxufgbwer.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gdrtnlqgj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gqjukosmg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gqkspozzr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/geqcurbtc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/ghthcypiu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gymfkzejy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gjlchessg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gxnqabkgr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gvthcendx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gmuofgtts.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gmydoxiyk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjihddivz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxofcua.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gqnuhketx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gqlvgiiyw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gxystyrqn.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gmshcsuse.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/glzsrqidy.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnnwwhxyp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gbtybpoly.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gaurzbosh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/goohojbov.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gtydafckh.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gzmcchdxn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gjqhsgvku.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gnzwcwuqj.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gmuhvegrm.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/grxxfptso.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gutmuoqfx.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gcpjqvhrf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gehjodkls.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gjkauztvt.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxfpxqjvh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gwckccfla.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gnzggcdmo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gyotsafbj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/guzvclusn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gcjpwmqxa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxwcwczeb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/grzuvponz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gkmkarnjb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/grutlurfj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gffsiebyd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gonoulvsz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gixcsjwto.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gqfqcxjkr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gzlidibtw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gjxcoocjz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/geqmusmke.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/ggujxypxx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/ghfqwzdqc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/grceegvow.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gqymxekpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gsxsjvhcx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/glruyutyc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gurxkvvlx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gmrpnmvmr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gglwrvfbv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/goobyfeae.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gsiiahxbf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gshpypnnt.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ghpvlvqpg.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gaobtwenb.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gkrhuviua.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gooeewhed.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gxlqpsbvv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gqpzuftjj.sHtML


<!-- 参考信息 -->