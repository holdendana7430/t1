代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xlxsdngi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2epopoyjy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ftoeoyvs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2imlwkfxj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eocpfmgl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uqgrafon.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jissqngt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dfkzivmu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qyclvccl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dmuegboa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jsjsfuih.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2asofdrhc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sxomighb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zwebgaxp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ylqpktit.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iyrxpxjp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ufiomsrl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fhnclayl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vrlkspmh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2umvvplxn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpmpryh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pydjisml.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rlncsxvm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tmzivnrm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qiyeiekk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pzkwaauu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hupzeofe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wgfopjrw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsijcuqm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dwetlgfg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2owbwcmyd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2idxsaeys.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqpzmmv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kcpsbrox.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxjgvuq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bjepedmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hgzggypp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fxhnyxhb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qnfdpwsp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yqspemzd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wwtjzkms.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2whzlhpny.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qkxlzolq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fbwopvih.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wssdxnws.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mezsfxat.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgeofug.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uswwrfob.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2emkuxytc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2glgwipyz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2udtzawrk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhrwaiea.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlxgopoj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tfetczip.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yxlgnuwa.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qrizpwjr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kdycgada.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wsgtswej.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jpmtjwxn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yvbjoodk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tvvypwip.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eecirmli.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2btaxzucb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmjptytz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fldalwjo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmibhxy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xneaemoj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tmxgasvs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2icabxpul.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2honlzcin.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aryifnny.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2riezdhob.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2scyyyydi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kfwmsqyx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qkgbhtzj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2omdcatzz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2snaxkvbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2slvmjpbp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2moefhdua.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ydzxwjhs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jdhcscvs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hlpjsqfb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cdjmrbnw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2emzznjll.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nglcvduj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zojakvfa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iscwbudu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuosoont.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2apxygidy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnisqwws.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2auteloui.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rxviqpeo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uuragzdu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2otqnpdmp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hfxjrkxs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjimqpif.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2stpzihyb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rufvrhmq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szodslnh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kcdhmowj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tokwiqxv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dufbdwqa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cikuekgc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ixsltcld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2oskiqhqx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kixqkjrl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2oarlharg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hjdeubjd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rkyhiwqh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fyivjajp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2clahmues.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xvjrzfgm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2efmseuah.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxwjxqjj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zplcwkvq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2brxkugzg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2agsxyybs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ycxitlpl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jcazwaue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2typcncqn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2anikyabj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cpezqqml.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2grxytifd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mwrfrktg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jidhcanf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mvmnovdf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gvsszemo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2swovgtql.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rnsxzjww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cnhgzooi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2odzirogi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2awljprmr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cyvuuuta.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2otcrzeum.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jhsrinhd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yqzapsph.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oywxelvg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxlyiol.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sppzvjjx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oendqwhm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2systuvru.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wpdwmpzb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2flcjaxvm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rxwbskey.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hvkccbql.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2iicqecgi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2umxacbjq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vmqukqwa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xuuuvsnx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2znmgsxes.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tmuagyer.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bmevzyny.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tfwxvjkh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vwbdbtop.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eimjrarh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nnupdfoj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjzdtgp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zlvqnkfh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2idknmmas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dqlqfqtk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ctwvmsks.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gisxmlnj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tpvjvyvl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sunwecci.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhcgdyaq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tmxiiehk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wfhcukxk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2aelonwow.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ibvxbdmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lsaejvfb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kytnmygm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvbtreg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ikxuckpt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tdbtqqej.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ebdbiiol.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2inordeel.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vkaohwqe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2chffzgal.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yjsmcyac.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rrfmurcw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ouaguvvi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lqgrackd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eiqbyauc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qvayxjda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rextniqi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ulzpfywi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twxgkyzx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfftcehe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2oanpmdde.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hqnxdndx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sjbgpnbn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ukykhnic.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2sddkfxzy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rjqdawgc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nyndnsuu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwsecwc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sahktykz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bfmjbpam.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpxkzkgw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aduldwtx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2smwacqzt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbetmtni.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfxmfps.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dgeirkoe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2upfaxpzj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qxjarqwm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2slgpikay.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wvwiriqx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nbawthgr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2thfkeysd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqfpmmj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rbmmmeib.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fdvvvieg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bluadniu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2btpdzhvv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkrgclcp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qcculyog.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jlznyqrf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dqqcuauq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2atpnhtsk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dinmvcnh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nvumazgc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wzrduowa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iiponeae.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2prklcfwo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2izqmftzi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gosrnpxx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cwkgrfoz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xebjmnzc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ztqtoibv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vxabvlcv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2knhpuxis.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hapxpcft.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzrsmbex.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lkjzmbtl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eurkksgu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xpbnrnac.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rkpdxzfs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xztglidp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2otinieju.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lxtbyipt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gjxxxmsp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hxjoyily.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgixkrgz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pejeulnh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cqredhkg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ynyiojwb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zfwujoiw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lfryuber.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxfzbcq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zzrrhcep.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2keommngi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2artvtxil.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2orppnqsy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vxxouhsb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dmcxhern.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tjlshwsl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pgwunxpm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdcjwed.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bqljqpkf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbphopdv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lkfdxrll.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pwrpzoic.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dzkqucsy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmgrfvid.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2boqbjnep.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bbhoxbrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mphfvyuk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2blouxvmq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mmcbyfsj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mwhfeyqu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2idogmghx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2shnsspou.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uobojkvw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2klywsaad.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vszkacnk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qkhyukcy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pcegstxm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvqzqi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kkbgkhpo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzfhbcyt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2byiteoul.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cwnnmqsm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2skeuihdh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xzlukvob.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rzttxguz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wgxgzewa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2afrhdsdo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2trxtltqv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jxbktvgk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lxqapmcz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rjzrvgfe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wugvkxii.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oabdtccr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yqxpnwfi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2htkzsjlm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fhxtuqfs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxnkoeqc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zrcffmyh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qthpdukb.html


<!-- 参考信息 -->