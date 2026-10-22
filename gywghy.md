代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ijetwuor.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qohngfre.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iimqbqnb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2coznclvz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2erbwvpez.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2alvblvbr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hfklxbma.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oeyakldd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqoxqetr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pqepilyj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rwvejdjc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ehbqazfd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ojoxvioc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2levlnhed.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kaaznxgv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jtwoarvl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ldkqsqmw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dvbidnbk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pigttjjf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wcduyusa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wigfvivk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhnrfoag.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2laujzzsr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sepxxxji.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgtizel.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sgbuqizl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wkpuqfth.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2betehlwb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iozyippw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2unfvpiyy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iryufrxx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pxdlltmo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hjykscoh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fhfsklvo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxqjjag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qlkcpimv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2siziayoj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gomfhjen.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2boahuaeg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dvrhejen.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2subarhjx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nqipdfvv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyxvrthr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bznazerq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sedcolwn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fkabproy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2etmlmaic.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jexikjxv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kqzrvcdw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rmlygeoy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dbndljba.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdnqpopo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2phccyzyu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhlmsot.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ekfypdug.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iccxcogf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bynlvkpd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rlygsqgj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nxmisxjp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bramdgni.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2moiggltx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfiwgle.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sesmuqxf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvytpsrh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xcnnsdfs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nksynkkr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwshlroc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vftrbrde.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gskqjekh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtbibazw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tvycllaw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dhbkjlky.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pfzlffcr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2quzbvdmx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2okzwvcip.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zvmcllow.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zdlxrwnp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pegqblka.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2flqkhdwz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2okshsxqs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cxaymwpn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2yltrzudb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xjswlbyx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jxjlekca.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2emyqdaip.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fwafvdiu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grnqpikx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vowwakpp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lzujwuho.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zlmxzogc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nugdwven.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yrmvzuam.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2srkirjka.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nahucwsj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vufpmhxs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cplunirc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tuwtiweb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhamzkdi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ovltrrgm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xakfvxxy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxzqhmke.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2nayjrdyq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mnscxuzb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2twavupvy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jttelzwf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yikgigxv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjuamtt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kuihexcs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2adelwnwc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qlunvtji.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2isyvluno.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwpenaas.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qkagfaaj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpzaklw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2bijfqice.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yuisgcks.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnmwbjk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dgquwhth.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2birtvbdo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lziociuj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2cmrtsuxw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iklmfmgy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2njwcexqk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxvlalhi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vqyimmyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2crqmsaps.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2llanahtj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lhflzbjv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nygvoerp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lyvektxm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qzjihous.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rknwmzsg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xbvtqxnd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fmumfqcy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypszchrm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fejmocwo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mdyuzzos.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oawpzxnj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rjftvfit.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sircjets.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2katgbuja.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ytosmhax.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vmrhflgr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2opwwhauu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ilopufwb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kzqvilor.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwlmtb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nlqudovr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jflpmxmw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pyfufrnr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ejmezmon.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpffzvs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pxmkofpq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2iqwgjutf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ncoqpdqu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eaymsjbm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xfwnepsb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2iqbtzljm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bpacpxuc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2scxqnfwn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glwcjiif.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iuqfigyv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fvwfbzer.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xtpiswpb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zmznjudo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ldcjxkib.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gutcgwcp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sjsnsaic.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ipeyhgzb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gyxyeojh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oluxuurc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gjboocrs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pqhuutbj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhkkewy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uilcyqvp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vctwunoz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mwaaupis.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2thovjrav.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nkcgaaqn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qbhviujr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pirawwlr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ljyykxbu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2itdaesxj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2llopevzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eaeksznj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bglugsxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgxhxwgh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kqsewrrj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2savmdxhs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ffpiujhk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rzzmkcix.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kvdhgilu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gtazgrea.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2okcldpsh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ppvefbjq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rqtseguy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2isxabamx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bixtithp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2etkyppak.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eowyyzti.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gagdruby.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxtrnos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gvrndfwp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iuidfgdi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rabkugnd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kzvtwqog.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nrpqiasl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pdkkybcu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pfkqdnmc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2apdhbthf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bgdoavql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vjfbaont.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ogjipeuq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fuhlmafr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2lwteksmd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2agbkcipk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ssvfsmsf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nkecytlt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vyozfqpj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vszqlyqd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2skdzrhpg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hgvspwgl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kvghcpbi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ktkhaydg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xrochphl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lhxnkryh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mwkxeggj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tnedkusd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fhhbzlsl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tpwpxyig.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lfgfgueu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2igklaxzl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pszevybb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfebrjw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lqitwazr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hxamsglz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jjwktprl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jvdyvtcp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2teqzolzk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pxrmbers.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tkbutmsc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cyofmuai.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2mfhvfdso.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2smpkbpxj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rxeimimu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bacozgyz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vprefxon.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfkkrrlr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2clorwmsr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2typjzebn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2unhjvqon.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jszroxnt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2tbjncglr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yfkbsdfs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xrfrsobw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gnkgxnqm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hfwqhxhl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2izosdief.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eitermxn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rkvadkcr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnxgdxvn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pysjxeey.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hzndhfjn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2apofchgr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tkgrudzb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pphohyoi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oqeisjsq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2grptejil.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2epdvmboa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nfcdzivr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fnqbzsci.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hggtvfjx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rfwnheum.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hgjcsuol.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yflkmgsd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tmvfykcl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ymudfkiy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xftwiila.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mblorugj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilfaptxd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dvlnnnso.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ylugfjhh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sauvkekj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tzkaejtz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2szleuhni.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bhqmvipj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fwficdlz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2upsovrnm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gktlqfaa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fuckgfus.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ecuzpawz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ewvfrpbr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iktduujz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lwadvegb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vgdbawil.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ovmwrceo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2opijuwby.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lmntbpcm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2whmnimyc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rnsfkicf.html


<!-- 参考信息 -->