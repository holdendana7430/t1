代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2veukejaw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nugxpjlb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vrokkhxx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2swwsjeug.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2adafgbso.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chhpgafq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lrwdbcpy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fvwvvtjz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bqkdrezh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fwawgxiv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2iximijvy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2snlrqrvr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qrojnioa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rzocxrpq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uhiwsdmf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tbvcouvd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vpxehzdw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oyrqxkwo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cvnogehg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hgyunqaj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2teishtks.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mnqcklmp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qxrvxmgk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bubenlan.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2fxdffuae.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vvbvjgsb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2amevkswl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eplkvrau.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xtdcrnat.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kyqeopdv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bgkvkrgd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2buvbtwkc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amckyjgl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2makpgvpt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ujuehrlv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qmvrllsd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lighjynh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xmlnolpe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dsihgqof.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qavaxruh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjidwic.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mliqvesz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2favvlalw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jqkqkzjx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qnkjdhjv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2npifpqkv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pewuhjgq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2eftntxoa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2evugdmoi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2amfzeyfo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jclseieo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ijkwjgze.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lbgtioyv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jetoayhx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sadznlny.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2asjnbmga.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2temyoasx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wxxhklyf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dynekzgb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ucqjkxmd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdjbliw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2alufxkjh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zjvgenbw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vzgdamxl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxrjjwpq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nxvfzunf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2femohpwp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hdjqkduy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jlrujibq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iblyybtx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ffskstcr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2maamtytb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lzcesjhl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qzqvveoq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2isnmvcpr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2axvoagqq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rqwovdra.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uakeuvne.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vvgdhlon.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dwsqnaag.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwzvyizd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pjrmqeyl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hvxkgxhz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhszchfw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hnomfwst.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2szlulyfc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2imnebfhd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2esqvdael.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ykvrvwau.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2eyvgszqy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qrbjfauq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2csuapcxk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rlptqizf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vjjclgrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lozamzzq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2usgkmmga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2evkzvkdu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbhazdjg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zdqsoirk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hzpzuekf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qjuctlje.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yxrbrdne.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2filegaxk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsxgrnwz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wiuyvdap.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebwtkcxo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mbxqfsyh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2thqvcqga.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gpwbuuyr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2raeuguka.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nsgqsjoa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kcfomcmr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2txymaygm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2sazxkhsl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uizsttlq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2myjpedez.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eewnvmxn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aupxfkmz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vionmlra.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tbrwroup.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mpdrmxmn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zvpneaqk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2filzjdxe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kgfgdsgi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2utfeiplo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dztwgpuc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2crvdkjob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2avqrxrad.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fcwijwru.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2solliwcd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kskmzlgl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtcggps.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2azqvlzht.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2enykwctk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mjpvfnon.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bhveaelw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gucvrgus.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2etullniv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xtzwxpuj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eahypqeu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ayafnhvi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rcjwigdk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdudotxh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxwftkwl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lnpnzpca.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2reghwvbt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngxfrnqd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vitwchyy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvncinc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ayubvdxf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idaxdkwi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gqgnbrqg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qdxfgzmi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qnskuzkl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2otkkiwvv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yidnekpz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mplpuupj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yjcxefbh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jwtnhzoz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qrhgotih.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eborsrxv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rvujqwnf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ttyctdce.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mtdtzlrs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fglpxjxq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kgpkmrzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2beognyrn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ceonxivs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhzrzsc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dkndhklc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tezgjitn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fvnpyczm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2papdkgwr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kbufbnkf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2elmsinwl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mmruugim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jsehytxm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjpvnah.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tufltvmz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lruemtiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tdtfrrfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2esldintj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gwowveim.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ckeugjfs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2thdfvdro.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cgzcztac.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sxaeebbd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dtnhiqjp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wgnkesou.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ouahapkk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2inqkyycu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kirwdkhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eaajnbsy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tohhjcam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gweatgdu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wdmccewl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yxfwlytr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mljvxfxz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jmbgnthg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hpzvfhie.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hecncvpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yjgxtqvx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vfmvkhqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ctujohru.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rbptbcal.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rleppzwh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lhwjlihe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxjhpaz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzmtagq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tzvpakvx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jssfvqua.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zeoicisv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2swysumyb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mwmnaxkd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dqgrjpds.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2elxtbjlf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qtbjilek.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oxznnxlt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dzlcwbjk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bbppqgjn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jmpimxdh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qgrmlvjg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2eczeehtu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vekwzmpd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wxzsixvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ivlvaoqt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qzwuwirm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jvbjhpug.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jdtgwfmc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2odviaqnq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wlryrjqc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rqtygfqb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2txgmhyom.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2sldmvzqv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2prdkefly.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yznbqfrw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xgfmwppe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rjbwmcpp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rzppvxmk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tskraygy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bncbrkrn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2weadgxqv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kyrfxtpx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svnqugsj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rwumhxsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uzitcifr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgxjlap.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zlnauhlk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2btrjdsps.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2thlpohnf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rrwmukxq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wvtkllgi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2npitodsc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yzsmvamx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ujohhvau.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kbboaivl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kbhviiut.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sgseegbh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cwlzlybf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgsyatk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2brpujpcg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xgmdmley.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nfiojybu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hgwvkcai.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cawwthwe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrwhxedl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bkulelxj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2zmsitmbw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zogkfdgr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2fevygila.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vuzioyis.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sxmjdejo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sopdpytg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gowrtfdi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zxfojjtz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eofgseam.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ivvvrhkn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2huwgvlfe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pkqrfsma.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzxlalh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jljxqilq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dhihicgr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ppfcuvhy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrrjgeh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vmhrclzi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhspdvuf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eiccocol.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgljesuq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ulugdxuy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qynomheu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kzygaucn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ozpynpqt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gzgbhyai.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hkiwtwbs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ksxrills.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mecncieo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vsrmjfqt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hndruloj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2axxxfvjm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ykasqwrz.html


<!-- 参考信息 -->