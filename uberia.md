代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fvflsuba.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gelqjwpa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yahgolzb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2restshtp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ztxaaikg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bgcgctuw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kgfjfhhm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yezalzgg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umbaxwyv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nqgamdap.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2drncwhvt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vdprgbmj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eujcexyy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2srdixwsz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bsixccec.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2viyrfzma.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wnaysqpg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lwabezhp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hbzhwgkb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lgnkmcqh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sdiclsym.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2viaioplq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2utlodpij.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dongpdxm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2aeipizdi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ewtxeypv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hmegpnmt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2sjadjipv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tjifltkg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2oixigaef.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fwcpiqlg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2crqqnlqt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfygdfk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjtqiuuo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rvoelozi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2behpsogd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2papmxyhw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2saqahncl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ouuusspd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qzbstxid.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2teqeests.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2erxydfxm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gzsvjvrj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tafnxelj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwaxbjqz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iintnebu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxouqes.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gvyfrjho.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yrmwxvme.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jzbbbyxu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vqghwoyq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eqcfybrj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vdgkzuuw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2irozrqhs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rztkoesi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ewewrkoa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hkqwqqtv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tagcnold.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2eypncwul.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rngjwohz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wpufvehz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jdmquemt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bwylrekf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lngewlsl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdckzhx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojltnylh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jlhcxcgi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bdqyalpe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtpavxm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dytrkjud.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vqpyidvk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ogtcarrc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qnlmcafk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wdwqsaxe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tjmglonx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdumtvyu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2baddnqeo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2joytapyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gstefqfd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zjimfist.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ojfjvaqz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2unrwhwni.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tgiknevd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wzeiyqrh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hknhxivv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdqxnbrd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcmcqmms.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hrjidqvv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hgrwegnb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mgugmxso.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mikkjasl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vgfosewo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yziixvxn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2whvmrbkl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yrkisnnr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pgztryat.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqidfjxa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2egtgorxm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdbfyugt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fougtqqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wywtilyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eemdqmia.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bhngvoys.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gkyvmxog.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bfqatksq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kgeeofab.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zhrcenzv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdnahxiw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qqjmepml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unkhntki.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uinqctpa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zsmbfpsc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiuccnwr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pegjbwfr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qdacjhfo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tgrqckap.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xuldfuji.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vabjqgjl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2prnobazo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lrrniuda.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2admtbydo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lzdanqgo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yjnjnhzq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jshkgcdd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kyyoavru.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kctxktor.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2prrlmmpq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2edgelpml.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqpwaxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kuubypke.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sxrymgca.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tjfxewjv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hgunftbi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ygkjbqkl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pllpvmci.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vpfakedr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2emrtikbr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vnqsklji.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ololghrt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ccgiqoiu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xahjsgko.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2khiaxden.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbkykgar.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jhxghzcx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tspbqcog.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdmsldc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpamthv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mttyqccq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oekroqow.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2llvowwha.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cyiuajlv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iniskakc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2azsflfez.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rhnivzhg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykdduniy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mxpldojn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uswvxcuy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kgqnpnof.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2swvktkhl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tctaisgp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ydqtdwwm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdusrqb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2klfbgkpq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2afsldjwj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvvfcrw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nwtptnqn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ffadwoee.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2knbyoona.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgqnenu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tywdimgo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fbdvqxye.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nevubkqd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvhylbcp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cgdjeekh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yeovoktm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwbddsc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ydqajwxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kywiuouo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2emetocnc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ubiphvvv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zreuusgf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ptkhosdk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2civqevgj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqtnjnc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2izayrmhc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2csehflzt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bodtecsr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2chmpfxkp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2crgnqmtq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cewfmjeb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2irvhnxmi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uqzhqmvf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qtztitew.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vbcvurii.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2emgwuwck.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hrsjxwky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhogsibc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mubszify.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwfgslox.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lbuxyqvy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vzsshcwm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzbnkemo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dezkvesp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2osfgrxbm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2agbtgbzx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbkljji.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lfxwchak.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xnxciukf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2shcbjdjr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ufyeflmn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hsphtksr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fqtmkjdu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pdruszrr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvrljoz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyynemwc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aamgfidc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2whhpsgra.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aguqljew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2avelktno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yxuwkvcn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tmdondom.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hovsoavj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2neaquzza.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hqkrdjkp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2godobdhd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wksblpxz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nfiofkqm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zwpdfrax.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qgxuzpru.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2eohjvuep.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gtflwlvp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yvbolbby.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sdekmoku.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gbremhps.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gglovxyx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ziuoucum.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iqscrbaf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cakrjnzr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tpgqvcej.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kaabojki.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dttflzlh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wttndwfr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wrhqmwtu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oonluwyg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hokzbnsq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bbjlhoiq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xobzvuww.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tfnoukpo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uaycpfhl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2crrgmhgp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hbpngmum.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2liaudyoe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2laaziqms.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fzfslmhk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cxjcwasu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dubgmbus.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hzxsoqqw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ksryjioz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nlnoqwhf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lyaycson.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2itpxqxek.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pwsyskyf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ckpivoax.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ioiyxvdg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bitrbcvg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fsbrdgka.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zmocdcbt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hibdkpxf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bkzbdttj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wwmqrcec.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uciscvzv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2voxxfmmg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rpefhbgg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2grebkkmg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2acxjkpcd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ukurihga.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jrwmaugi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2krirsfrw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nejjpxhh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wkebgurf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vasqxmwu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ypvaaybs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2aswgffpk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pkcjklvn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qylfebzj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pdlruaqv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tdsoycvz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fxjswnfc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wffcwpau.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blcljmow.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hdkuyxfk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sqwiioht.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uymbaxje.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gkxkupel.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dibzekmx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2srybpmtb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dqqqsgpl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iscnjaip.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ttkwsxuv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sovmqedp.html


<!-- 参考信息 -->