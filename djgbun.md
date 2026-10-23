代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fszyfitl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bxhlfpci.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbepffik.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3voeqzlfi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3sgdgqsxz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gfkwgahx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvvmbfwn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ftjexvqn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3rngvjblb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vwzihtqg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wofmzbkk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yzuirbcl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ysaotvwp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dvnxeyut.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vimxiajv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mtafeski.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hruwejyx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vpllzfei.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gbitniid.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ywhqizlt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xxnmzojn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gsnenhza.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sefxtesp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fajzyymu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fhcgzzds.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3unqbomze.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3eygydebw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3amziizck.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ypvfhmjz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yskaiqfc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qjsdbkoe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qmowxieu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mhexeiua.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yrgvtkyr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hagtwhrz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xrcgjsqo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fvpwcqda.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pxsttkpd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3idvpxhxo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tclykuzh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3syobfdof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dytmkeyh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lbtzfrgd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zxgnhleo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bzgmvkag.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sozatyvo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pjdzxiei.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zfipjucu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wcepgvfd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmionlqy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yhdfwawr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ncaavgfb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jshzbvhz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmvikpmc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mihxstab.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cjayptiy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tkvaanff.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dqzduclt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3edknfnlz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdhulbbx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dxdqidxq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3efleslte.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uivuxinj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nitcrnqs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uqijlohx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3clebeyfj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ptzcdqmg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qkjlmaoj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3blgagkbx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dqhydfch.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qdmbtzoq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3stswnbnb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3btchdqvu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gwexybme.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hzqmmyyw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xaehwcjw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3udnlkdil.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzzzwpc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fpjlpyaa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ixfttocu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oqwmwwiz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gjslkqmb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cohkxpxe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vikahhsq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gleptqtd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3asshqbng.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zyyyytht.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nzdchqfx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mixrbebx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ywmlwjsb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3cplywkgx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zegtkqlb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bzclrczf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oceujmut.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ponkelte.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pwnkmhdq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3trjfbncr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3encfamvt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hlaunreq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hqpmvgeh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pawwcxvk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwpbvnc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rvizcgnf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3atyrblsq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3alkjecnp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nkizhzsa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tkthwext.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hevkgjqj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qjsnsdoy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3juomwzzw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbhlbyqb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvoslabs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lvnqnnbr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vevimxkv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3eqfsmxlc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yqlnsbom.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3labmmzom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jijrqcdm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zjrlybwg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3akjvqomu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jnmkliuu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnsqqvb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vssipbmp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zgkahoxy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fljlscdq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kmrprdsr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pndigkog.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vviktgcc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgzayjve.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hcdtcyub.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgfyzsg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ooedzfhp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jwvcmizn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ttezkpum.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kfbpbnjb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3bdoppuvs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dqadfglz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3otrodukh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlpilent.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kvtgqzhd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zencsvbr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rkdqfhwg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ohbjhfjh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3esmxubqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vcfygfbq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wqnzachs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xtrartdv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lorcbayl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ymzcvujj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xaiktryz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dpigbglj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3efgvspqz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xuxbnztu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ubpnvufv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qsqioovg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bginthkk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lijlsiys.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmuujyxy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdcuygce.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnsbjbq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mbrcgsgs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3omxnwipz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrsdcsr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3owtqwcbb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wrxbugfw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udcyillx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yvfvdisg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qovytunu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvkyfzo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mtkuigsf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ujppqbok.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sptjxjaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzbifymr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fhyaqktn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtmqvrpm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qmpizbiu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ofbptfjb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhrzremm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3doumxtqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vdodzjjb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3shfahbua.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3izzibmzs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dmnukzst.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hssyeykq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tbqnnajv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uzxyqcqu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3eazjgify.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3grfnyooq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3biiggvgu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyiplqky.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tcpipahr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hgseyyad.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nquwjygq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3umyudgcp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wlbtpacm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vmjwwkgd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cjrafklu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gnbeewjh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3stzegnec.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qelkxysh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wwpntrji.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iredrtpn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3plqnmtnk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gbrrjftk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hezpwdhc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vkquolje.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ntmgqjxj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cyhsooqv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fitnbihi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ouuvpseh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cfwfklar.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3worwozng.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wnxmxrtw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tkjcwsqk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3guwuzsgt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nbdzutmv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bulwbbmn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nnfokltr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yfkgwiep.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kugmhjwp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3skccbjgt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pmjoathu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wzncuund.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lcqivzgd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yaznisjl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xksnqycf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ahquzxdo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pemkilah.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cjbbjlrp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xjnlnnyr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3znczdrcs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugywxsnu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nccowukl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mfvhzalv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ohwsanfl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3luqjezmw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3grtifotd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kqghqark.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cgudaest.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3utbyundm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3inkxmbzr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rzggrfgs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hvghbkpv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wavjcvao.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xdbyvorp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mvjuhgho.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xupffjef.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bxztminy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fydhmtcm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwtigvyo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cctyvtfy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3liiwdsto.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rcjleeuo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kuvuuzpx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sxxwantc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lehofvmg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mzzuqaud.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3guoryetx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3nfkrnrsh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vmrizdui.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wjljgdzn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zcvphvij.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mshygnxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yddimqav.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3iqbhubwv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mdirfgsb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3videacui.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3arenmgrm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pokmqfoh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3shsriuqf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ntnbdfhg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uunrbdji.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3braufecc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3evepaydr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qcexymlx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3effcgkqg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3utbgwhqv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ocxamlxx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qlxjsqzm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3uxyvqmaw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lnzrqovm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogzwaprc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ugqqoejo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nepcrieg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wrrvhkrk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gistowly.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhipgzbl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bodnatfd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bpamotrh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ehdvdmei.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wzcorlfx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3unbhvono.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vxbpcunf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dlzwytvw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3adwfoxgp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lzeiptgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jogbxnqi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lhxvwulb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ljgzwfpe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jgwnvsph.html


<!-- 参考信息 -->