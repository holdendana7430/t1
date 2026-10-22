代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cjepyyai.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2auubmuif.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2slspydxn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vonoenpr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jzwymplz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jxmhsuqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2recxptrs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tyxffrjq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dsdipxbt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucqzqyau.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxweql.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gnyanfvd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nfabtinw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bnzaekar.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wypvlegz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kzfklpxo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkyklcnf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oicmzjbp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ggyqhvto.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dtisbeax.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2huhegrup.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2melrqyic.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vcdmwtmk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzvnnac.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nkdkbmhx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gphwqocg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lbxhojek.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xcimdspv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jqmpixfb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cumhnqrg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nutuvbzw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mdidmtsm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2onktdvtu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qosltwjp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrswpcfc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gnlkahze.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jxdpauoh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lfjtjlyo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2naqsazcn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ftdefutt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmoddwy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ayxstzwh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tsxlzrsc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vhqzeozz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tsjrhvpr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zumsbhfr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sgknpvta.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2arahqolb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ggzitgnn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tyfodave.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ldsxidul.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzdcqpaj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ygqualjp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xlhmkvvp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2owuiukzu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rcqughcj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2npjpfmwh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aileqptf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2davfmuld.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uwmthwnu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ojtgjlrp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2beycloqd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ivwihjfv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdvdmxvd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gmprlprh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ogniqaph.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhfuuais.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ckvrjssq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rqcktiqq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ecvlatwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bllaqstb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2faefpkla.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rgmtvdgk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lbcstrti.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vmebccmx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sonlhvbn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qzysiotu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kongqksv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xxcdnfkc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2exysylkl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ecubcjeb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rvqolvrj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2myszlhll.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qifrdhyg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2yajqvchg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbswuqb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xhriqnfd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ycbjzepv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhadjuo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pnhyvmcv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rscxhfxn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qcylaejd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vcbfbkvu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kjlmfndc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wizaqvae.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fgsajuwf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mtqyaxzj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2duxkfmxa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gmneavko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2micjwtzo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2szgfhacs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rajptpbm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hprgxkso.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qetycmdp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cscseatg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rvovohcx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zfwrdqgd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hqtydnsp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2akzymzdo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jwwdqxrv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ffrsvzbw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wxxqquvj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bxplatzb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ookvktvd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vkberwvv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2grxojabn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tiimrrwe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hcnkqhxp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yjequdvp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xrjendhj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2keaditdy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ubrytpeq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hxarjwbk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2puxoptpd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2diijnzjm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kdxbvxsu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxzouhhu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cwzucktk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dhzeyqwc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hgfihlus.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xcitnshz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ytjrpshq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uvupdlrh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hqnjgdjc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vfwwjypu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hjphrrwd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2grwhfuho.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wblteqsh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ehkidmhj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jarrpodm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvwwobye.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dhuyigzq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ypncusnq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jucwoeks.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2alubzkcr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ofhfntrp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wywmmczi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2balnknra.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxoegouy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ozfymyoc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uwphwbws.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tjqjvgjv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yeiwqovf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jgdogubf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fxlcdycl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gydomzyt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nmsncmwo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sijasusx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gkayulct.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2njfcokgv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vvjetpjo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvtfyvf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcbepljg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wafnyokr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tulngjiy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iwpmoaox.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mypwrshv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nxkvqxsw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ojteoqka.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lfrrjfte.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kyrxiyoo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbpekuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijwybehj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cpgojssy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdvwayac.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vaeanjkh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ukrnzbjl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emoypmkr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lkqirwpw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lgzkaver.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xllgtmhn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hfpecbcw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wvomnamm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qsqukoyo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdaktbtu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sajqfahg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eipszuoi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oadwazmt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfxyjle.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mhkzpgni.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ffcuhrww.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jnzbggsj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kjdffsjt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vfenaawp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fjisqlkl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fjozxffq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cmtnkzva.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zrfpslvq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2opoistdg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ldhfsghp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gwcexxap.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwsyyax.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2krxlmfip.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vwarcutm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ydpjjgaf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rrchnkgc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yuchvwot.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cbczmmuw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ulcnzrsk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kffibpei.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pikswbqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qeqbjtjz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozlykzqa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wfhyipsm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vdawvxqh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xxcqunme.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ziopzvgr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2igfpknvu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gdkaejpl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ikvypmyx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tfwutfsm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uiziyzqs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2uaosjden.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bznuwseq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iptbaewc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vgqkzuvl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wchcinue.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tbxpfrqp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jaqmixsk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2swqpstzm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jenpspuk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cglttjcr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vlyexcnp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xnmaicdl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2oqkxspju.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xeplazgc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gmeyrrjh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vfezpctg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fzqiobup.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2feombztn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wpajwrci.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jftqqrzh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vxgzbuia.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fddvstdl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2edxtrxwv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xjghsdui.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzhrbvr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tfrrpggj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tsczmpve.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwfveoad.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gzetkybb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iaaxppck.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2acukdlrm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vnfxyygq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2muajizbe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vfpqvval.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dydvxltb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gvyonroa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tsbznscy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ioqcbjyg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wswxudtl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cdntacyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2amcmjyey.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xvzhfdvn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fgzgliqb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2occxnjql.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2okkgxoee.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2euqxkafp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fliiyjyf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jcjvetnv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2haoajbms.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ohgesdww.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2expgrseb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qomvqtqw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fqumjrin.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2igejouqj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zgbtlelu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gowdtmiz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbbewyyu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ebevncdf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2eeiafupk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sbeabeok.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xelxwgvh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yxhpyxaz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wjpelxrd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vrpeapwe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2izpsdzoc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hestacgc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2myfseihc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xpeskiap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pdkmzrai.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vvyefmuo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gtsondvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cyweywvs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qkidyfgs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjxbngu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpftdeff.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lrwtuorh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2fxfwwcdr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vuwmegsr.html


<!-- 参考信息 -->