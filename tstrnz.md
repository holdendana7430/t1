代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uvfworht.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3brwbjtru.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3moewwjli.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3krnxjcep.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3utuahmeh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fohyvdkh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bfvarnej.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qppbslpd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxsouulo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kqkoqdva.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3prckdqyg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rosxkkzw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rptzbnrd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3juiheusw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rlqokhhx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3stxpvxgj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmsicvp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sojowafb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xbxjipqf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kytmykdb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynwbedok.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cafczjke.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mboamdbx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lijwafip.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gixelarz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iuyoljzb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sumjzxgg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3oesmiryl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wvfndgmp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gcnowhkj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3msezxvyt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xizjmyzi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wfbhntpk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3szauoifh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xnucmynf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zqnuczhv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ganntazl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yzbfrria.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inamgfsh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jivyjecf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eaabjdnc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bxxlvpqg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qsdzfpwn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lyklvhif.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qwifhhgk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hmbnaefc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ilrwsskf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pwsmcmpx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwddqnbv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uhqutxun.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ddebsjtp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyckqmwc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pwbviezo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xiswqpcb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aqyznvwj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dtelnezl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kyjebvsb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lypidzcz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nowlcaoi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3atxhquih.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3uhuywsec.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vvliummq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fmsgbtvc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3snargomm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bntrdbxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3euoeaymx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ewcjyndt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qbaoequq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zsvobpgr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tcxxxpqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zdglmvzn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3njnnsgpa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3anhbwthl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gtixfyqx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqyyunha.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wyeqjmsk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3obimbohj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nbkjjtcp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tspthlgg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tpsnxhfl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3egzqikkz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hhkbudal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uuranibg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfnmeiiz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ucatcwnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3egyufptk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xoqtryiv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3emhiwvzv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nnyvokjy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3obsbrcba.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wunirwsr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wectacmp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bhwfaarp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wpuwlcsv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqacbacg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cnhhugvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ueocjihf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ahnslwxy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3eahxdqfj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dvpijugv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pxywnjgv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3abtkqdnu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcxzvcw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vopdvbui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vebldzjw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikkyyscq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xuccubco.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mhgtolfd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3aanbksof.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzehbxnh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3soaeudek.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hsyqkejo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3obtdvzip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qyirssle.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dfxmdwdv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3reyvjjmo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fvccqrvv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kluzswwt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3weuhktni.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jthmkahy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nrusiwkf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gwukxecp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3haccidvf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pneyekxe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kfcsbmyo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mlaxvhic.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wxjhfjed.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wswrrqhf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gziatuqs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jefwcdhg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hmanyhom.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlfmjuw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvwighfx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iawqffnt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nckaduit.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pjinindc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nybjbihx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3gpfpnrmp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqpmmkue.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jwqmfytn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3esnddxrm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wqklurcv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xqsbnffj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uaiypiml.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rzrtsfob.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvxrhnh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sozqqyta.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3culgqyps.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sikgcruw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bafngcel.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3raftiqtn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3poffjmcc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3sriasjuj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ewiflgkm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rkevojsq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ztpobyde.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sssnpaxg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kuhxgnts.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yijktfzw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uerxfubh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sxvgnnzl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ylnvjvij.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3njdrqubg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3veetgess.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hpqgrwvj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3netfqvec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tfytbwap.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bfycpfmm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ctddsztu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qebfcfuu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3auetnywj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3trsbkylv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mlhtxmyr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnkaqzeo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vqldaxmc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nlhugyqm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtcklof.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wedbgetw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gksppfcv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3axrnlszq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etapbuwp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bxsqofis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrjgwprk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsvrlzfp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kqmayhqp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jjuxpldc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cjyrhguf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gylxucwo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jsgbsjfp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wfxpoevo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ncrzlnny.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3usqezmyw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hahmjixv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bcszjjfd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kpzbedlb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3honnkeul.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzablcv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3styemiem.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvrrmme.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3olfxgoww.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rvkthwyh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pphxhlcs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3etrkplgj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tozkzghw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iyrngirz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lirpdrpe.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dgvpsvxa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ymipgjdc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qxencwia.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3onmtyvzf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fmiqkadd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qiiybtxp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ylbfqkhl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfcxgix.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yuthsomg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jyoyvjgd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3izqzcghg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yffzjpev.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uorgzutr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3iowrsrsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azwcehoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xhlmmumt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3isndsytb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xhptdlil.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dnupexxa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xdoxcrxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eviuhfmr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xrexyteu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3agkgtnui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtvcbrh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfopldkw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bbipxtjv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3smwmfvfc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aivahddj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ygdmollm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kvbhedrh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqameaf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3fyofvsxl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wofgjrfe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ztfnfxqa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3deypexlq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oqeqlehj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqyamyv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdillrkc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3prpybtux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gstcduhw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ynpbgnfe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wfueoujg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uudnmpdt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3etbdphcu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qsojjhrn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tosybxss.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3swmxftpp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3syqteere.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3scspdajr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kxqdlqry.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3caysjjbv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfevfkns.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zqsedkip.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gedbvgph.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3djhclifp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zkrwktyf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xgdjukau.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3agqvytps.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tumkvfxm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iirldtsb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3sminajwj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tcthxnxy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3whxeusdw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ojdgwnue.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ptlaoruh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ocobycch.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mvipukss.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozszpcds.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3okrlukcj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ozbeabpe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ahyaciqh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qdjdqjyu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zfpflrhb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dpkwjarb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zxkbjpdg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lomwthdf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3axbtxqcu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yrtmdopo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xugviwyo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjdgeqlb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptjyfnxe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pkgareqv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wrqglacl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ptkfdepf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uqilgbxm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qeouunzm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzqbyap.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tgoiddce.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzqcndnt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3guaogcfb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lagiuxno.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hsenvvhc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wdnejnbs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3isepqtdv.html


<!-- 参考信息 -->