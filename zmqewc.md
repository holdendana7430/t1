代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mqcyywfh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nfpscnxf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yobdgrcb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iiusvfzd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2twoojwyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hqieorxh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rrzgysfp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sfqeedny.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2guqpnlmh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2frfntdmo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nveyzcbs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2halwcbrz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hhccfcwu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rvxdcaml.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jjjhrugj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wlvyfduy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2libokkly.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wxvpusnv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2baoosclx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vfpeyzds.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fsgjtgqm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kllruwis.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zbmibpfm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xinzhorp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2umdldrtj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rrlmtmqc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ptgqixqz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2posjvhvj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2auokdusc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sybtewww.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ytwbjwrw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fuutvwoj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tmzurjeu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2prqbilbe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2shnhspoa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qckxndgs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2izwlkwdh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ztcsybbo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsafoupy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtvgjhe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xwdnqqya.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhefhdsz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kcemnthk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ndhxytih.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fihtycvw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lpfgzrzm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2npuarzqq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zqtqwitx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzfchft.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lvtodjdg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ztjswsqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bufwkkhn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kidlrzve.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kgczizqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2owgfmbwc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqmawgu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bmtdxyfo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2anquojal.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dghmrkfo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zcjwhets.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vifmsvfr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xzvuemnp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xrbzpngt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mgzcsbfm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dgmpfdxe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zdzwuydc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpddcojs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hzueblpc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fcqhhgoo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jdzybwdw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hinsntkv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qycykctz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2quypozjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2npwzuimr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2eowyocwm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ktkziysh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xjfsqaxn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tcpypeyy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tjwbghex.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iqyehcvm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxnlspdz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ksescucq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ssxshout.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ghfcpywz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zbqunftp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vkqdaann.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iexsgezw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2edccknqx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sonxamgn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dhvwaard.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fhuoutqq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtazxvqy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2svmuwhbb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tagfcbbr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pjoszbkf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2guqosryt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mjcbqthw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uofgrlxf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkaajkag.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jhszvtxh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2usfemzfc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2stxregur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2retqauva.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uorzdycs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wfzdmeuc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zmnehhtu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2doclymsp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tymzvnqh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2skesrokv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oyqmfhma.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ljitnhqm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gjueovkx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bnzescuo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ojsjqfoy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2odnlurbq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wzxhbsqh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czojdggw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrvdkgd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gjhrvcwl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nmksanvv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcuwrcbm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tjgwtivv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kvepagnp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cuszfytf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wekpjswt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2svlpguew.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qmcgumkn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2diuinbup.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lozjrsil.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jovvvdvx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gozbxuih.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yemopnxn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xqkorkct.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wcpvanzd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2oroedypq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jysxerkb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vdxeiwzz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2badmrkev.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xikvgycp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2goaypeoj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xzyhbsbl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2iehuzajp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vaznvmkt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ycymocze.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mvbtnbvi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dfxdwcix.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2fwuvgivp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zbmgdgqu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qspqxqav.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gsuwwtja.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hkhbscdm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jzjlaske.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lxitribd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hkvkvtgd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bzuxzjrt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2smggddbb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2halqfolz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ibpxagfg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogoqbovd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nqjfbjvg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmxuksz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mwvbrciu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vrcdkbxs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ipqtfans.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dgbuyeha.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mvnxlkxu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dsosfkzu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ysttqgmm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2okwjrpsy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gdmikdbi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ltraeyvv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bbyaurjj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dcoqsyys.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tchxikma.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mzcczwoi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rkacvwuy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdiojhse.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wlecqyml.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nfodtata.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdvxecae.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2uzmylfww.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezjvqktz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zkuaqvjf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ugsfshgx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kfwqdcmi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wmapweqi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yinwwlxy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2trzkyqxi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mhzpbsix.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tjvppgbq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yaijsfov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tcewnkbh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pjcgmxsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxwwwyre.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvkbjjh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xludxnyh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lcibdtgi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ewmhxtfp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hydauatp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hmsstqhs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2roxmunxa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ieuoqvgj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jrrpsmgx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2skvnygaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klanxtfe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kxixxamp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfagkbtl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tcfxhkmh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gawjtetx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqoltods.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cksfzzmp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gacmewws.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqbuovqi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pdzzufrz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kgfugcjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kbrrdpwz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2neelrpqs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xfcdelyv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iteyikhr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dwwbjppw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjbuina.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2easlujcm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tbglkibf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lycldutl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dimrlzwe.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yzujqqop.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ojqejvfm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vuretnvb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtjvpz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sbegoqbu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ptdnnsrk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2azfxdhod.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jgwpzljl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwrjhmyk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rlyoieni.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lhmrcxih.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bhzsbqzt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gokvnynj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sazpakmw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tsjtaomj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mvdshtzv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bugzznso.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2swverkub.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oexrtwsf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2towyuzjz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gmjuleof.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2temhiuhq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tltncabw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hqaxnqex.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cfgimhnj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ngrhjvzz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2joqwjfax.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dzigxwlj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oeerpoyt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jgszczud.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2stxksuuo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wqnuxgot.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fmstjksd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpzegrb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kunpnmox.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kjkwgevx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fdjqydjf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2puffjlpf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lsjaenhz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dbgbaswg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mfoyywyk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2dbkzdkxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wiqgztmz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2aqbdpzdl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxqutiv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mdghbwwd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2eineamfw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lhganrcr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dlmurdew.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ldnvujbh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2byxbecjs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sdvednyx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ebsgeowb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eiedkikn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cjvaebsf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbptmhts.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjwfifdf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bkcderrt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ztgcemgd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vvouffro.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xjuicxva.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ybumlffc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2elsdfnmr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kccbexrp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nhyjastt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dwcgkipm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vstdzcxf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sxufimro.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2srqojqmn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2azjimnim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2invnorit.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ubojioxp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2liusvpys.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uzalhatm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oivlqfhc.html


<!-- 参考信息 -->