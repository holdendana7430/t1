代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pryjlcuk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bsxwries.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2huqwnphq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uubzexzu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rpnzpyke.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjuhyipn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hsewacob.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zosfodlm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2optyympt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2knkfzmaj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ynngznmb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2krtrlmhv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gikbwuxx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qajtftus.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bfwqjnqb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eyqjldrs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aaskwice.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vvbdeqnq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bqdngyza.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ioqnzors.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2uzxmhasd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vsyuwcgc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tmxlzdyz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2midjdzsu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dcyhezqa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbjhsbnf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fhnpqlqs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kelcqhtm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uxwdulgy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ixyfxsjl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2croifnxq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vxjhqnbb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijzcowhn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vkdpmdfj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sofjfiqz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fncckcus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ywbybhmp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fvtbxuhk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2puoipojf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsdfjsp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tvcntbwb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2akhixosf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2iiybvabk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cczjzboo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fuedotcf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ucoratgg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cgjvarpt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dzymkabq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2exwudhnp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aidsudsh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obxdglad.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2diqhiook.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xfetwiqs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qvvnkpco.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ppuyalyc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hsjgvccj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sxizibuw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hffbjnub.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2autkbeou.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nquhmcil.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cddnuoog.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zioihkrb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rnwofmwi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pfwitogq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxglvjfe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vftpkthe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2soaxqvve.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bkmbxiyh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qwepuocz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gsfrqder.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lozacsbn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cicksrly.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2auivpgwh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plqvskhe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qlugwohk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2squuyfbp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ocphexoe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nkpvlslp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbhjjjc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mycbkglx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2armtvpcs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ikwvkvfp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrfoaprc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sspxctey.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yhloxkog.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jansnzpp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dyhzyyxp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ofwhmrlr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aonmdvhm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2twfnacxv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cekarvmh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pvuctgte.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ajxlzgxn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2exyvwsib.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jqxvhefu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pplnagke.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mkzhqwdi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2puadjuwa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2spnqapwt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kehxqfof.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vszzwtfu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whpzrvdl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zjshcmbh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uoqfyfer.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yopdaqpw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2goraxjhg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nnvjtevq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fxqgrkrk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2iujqmuws.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dekzhwfx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjtcpku.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uhaswpax.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2frgporok.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vmfzlwll.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mmelpisw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qaspgjhr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ijakxqgh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2drrknnky.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ocqgfnfh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vkknvjtm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2korszmmn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2iwolxoui.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2msbdksur.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mlwyqewk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qiweomxh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xihsvihz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2urqopeth.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjxlotnq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eabvjfwt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iynrmfaw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2oelobanr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2awlysuad.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qypdepju.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bnftqsuh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fjuwrnbv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bugdinav.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vxkyhdaz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oubzmoch.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jttefjct.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyduaxcq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rfvqcvys.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2juqqtala.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tbeanvqy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gtcwkmqz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvaezfi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tukqptbe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndailtee.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bhylgijk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qdhsgcym.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vwsdcqlv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cenrsnfs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hcfakxcl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fqiyfbzo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mjkydpqf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gejuccul.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dwbhohus.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbundgyc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbersgf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yembkeyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2epwecqao.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxyalfdh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2gochrykk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uzpbglzi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sxmlncnx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ejdwuakb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pictjeoy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gzvgaxle.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bjuqpdoi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rnqqewfm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rgtsjrae.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hcqqcanf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zkjzyauy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lummaypd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyrfohfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cibktwtt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yoebdlqv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qrqscuku.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urezcbex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrmldlkb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efguepzw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aleniuqs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vcxzyjkx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pogkoysw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2grctobdv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hdwpgllh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zlunsrfn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cmvatqmt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnlyscd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvjiqeim.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jjaurmry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwshlsbk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cuqkamjc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qgdxvdhb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xempwfhs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcpdjbcs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fzyplbqc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2sdekvkpf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ipxxmgwe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2gmcpuxlo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lmnzthzf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2loyeezga.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kpwwoklc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mtdjcnja.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2crluptvg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2paeobawy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kywfoygh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vtxkoiij.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xgwhqfik.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2subnsjen.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nzgfjmit.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rjgfymdq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tcaodvgc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dfcpents.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2eqswygef.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlpqpon.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rcmfovvk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ywuzxyxc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqkrrrez.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2uawhehzu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2anxdpzhs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2etqokqao.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2najysnpf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bznwojiy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fdxwlhto.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrequyok.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vxjqkrpa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yekahsta.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wlrwgned.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xdawxynz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gejbqwmj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jbydfygm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iysqdncb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wxdnwyao.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ftvxsufe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2aelccqmo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kqjgudhf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ebqtwaob.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kabeglul.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2auuunzhi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jgotxtzv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hicbsmjy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qyyfrhvo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmkocahi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aahnmsye.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tqqfqugm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2oaqosaus.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zyjcldaa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jtizymny.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ewquakrx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wrkbjblt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2csdjneym.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pzsbmtsc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wbjamvib.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tvlnhayw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ojwlupzq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wfjnhrye.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cvdqbslu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ckzzdsdq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ovvirjac.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2drplygra.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2pkoaendj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kkhpboxr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eiuijiae.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2pznkrbnh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzwhemip.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qvsetcay.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2msbiczgb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2olgczoyh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rzbarpnj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hsdxwkoz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fqvsbawh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dlfplutd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xcsdpcka.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2snwmyjim.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gtwumydh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2diehhxzu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jbqopsuh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qknymzip.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uvdmyqot.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pqgzoqzw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2alsuujzo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2haibxbrz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vrypjgtd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmgydso.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dbopwdev.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jqmlisol.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uvywxvtf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xkrvlxfr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mqowrdft.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jgqynlst.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kacqaxoz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2eucjpbtu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dkkrsrqd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzwgajfw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkzyjuuj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wqfqenwh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdyrwhh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yhvnqbyv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gpcvbwrc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iijafdrw.html


<!-- 参考信息 -->