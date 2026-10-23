代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3csqtdebe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ddmqtqes.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nixctorr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3suwausmr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zjxfjnux.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tbshkvfs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3excoelbv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ejihydjs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vazwixel.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kvbmjpzm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3stkjfjoz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyiaekgy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqejtfjc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gamdesde.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bkedrilb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vinkktvh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jeizoqlm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpxgxypv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kckbkytb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nixuubkx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vxtihrbe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mvyhmksu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aavjfsei.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jyuoxgci.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jzbspxlo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3chfrijrh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qplxgvwg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ylvbtdns.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzugcsrq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vrpsrzhv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lcezdegu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3weboenlx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lmfwvtyk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3srfrkqil.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rsktoxpq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3eomskbcz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mmlayxyb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdziudvz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zoceczhg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mqpylqqv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mlijzxsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3prfgvgfr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ibixlxkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xhmdksup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqwlnte.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wnigwkgs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xtdggkeo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rqutjyic.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ovyqkfbq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdqaqlqv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3izdtypfw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxdvsqi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xrmykwtc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3atbacjne.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tclpjevj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3oncumoeu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3syqrnibp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3etddolqh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqkybixw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3eazjitho.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gjyjygxp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hykdqxis.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3acneytgj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vytpnpmo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3booikwpf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fltljbfw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xjwtayfj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iexnjhed.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dnofqkke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdspldfh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yemceque.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fszzqcbq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlyxvvhh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hryrcddm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gwclhrmj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjjgiyrz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmzfopka.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wtrsctvi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nodvlvxg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aduaiqmh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3yrbsmwes.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3awexsyem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ceckxcvl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wzxhfths.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xwodrzlh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mrygdvrr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sedtvext.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmffmyi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opeayuuw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ctsbglgo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dvueovix.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qezormzr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pernbwzz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3efkrqrai.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmgnycjd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hpymvjbe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mechhoqu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gwqbvysp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yvqeblgn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bjyiepnc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3njvkvyta.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tpzgcwon.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxvdmit.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ayaplnaz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bklvexwr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ixevfpzf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nimplriw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jzvtimkj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dbsakowi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3esxqjagt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zdppufem.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojhxfsww.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyyqkjwu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jouqpwiq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3olmvmoot.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lguhzabp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffxlsrxb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wtoirmrl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yrdbuymz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vydrkyyz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3oxxdkgds.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ohylfnfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3viogzsik.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rjkhbjrx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mdnoxykm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3usqmlbhd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pfiaiaqv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3smrvogxg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dcezcdch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghpcqbob.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xiafndsf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kujmzwqm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fvciyftx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ecxkjmaf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bvqbzfcu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3injtzfub.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dxrbakmr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qdaljvgm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzesdav.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihjlcqzd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oqxuuvui.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gzlryjln.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3neytwbou.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ybhwmegb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zxlwnywi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3awmpmvgg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jokeqpfn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3icpvcudr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vwctsaqs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agxcyhee.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3endkclqc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxokgwi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkkykrp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svfneumk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eifmqggp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3wgatgaln.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iyauqfvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tugtzruo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xshnzdhd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pjsikhat.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3sdukbtmt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fufntnjl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3tgbldppi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zkrsjszd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tvvmabwh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pauetwjy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zypmcnbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ddcaanwn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tdcnmdwy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3agzlhrxe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oyhacrot.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cnfrkfcf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3uhedfklp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rcljptln.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ogbebreq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qhdqcmss.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkrwnpwb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3woaqgoos.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ycvkelam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3omnemepb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvuwjfjn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lsxwpxbo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dpwrqnxp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lrfofzxc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wgndugbz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rbbskbvl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cmkapgak.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wrwubfeu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gmlblpkr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3recjclep.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ixphutzh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3cduwhxai.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ftjlrrce.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dxlxuohe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rhyhvnik.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cdzadpfg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3toypocws.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jhtlvobr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qtuvbcrq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgjxlzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyxqnrnb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nsnnbvww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnhyikpf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mewehejf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ijagpyko.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3przbiyhq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nxsbadxs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nnjsgcgw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3eosfardc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vwjofhdw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rcpuighw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3khccdrpx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dmzcnxux.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3saoyvsyh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ebukrqqr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbnqaeq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwvdgvr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qraxyhys.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3djoguyqm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wcknpmrk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lpdharsm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3otxhitmz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zfjwcsel.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xprkkowf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwgwiec.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbcujjp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfmdccf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ttdsftkz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xtydwdoz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kjlzjgbd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eojambmj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mdzfbufv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kpninnvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ihngkrdm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xywhgvrt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uovdvfyb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kftqaxbn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vjuohfiz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nyptguxv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tgcoucel.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3acktkqfp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ovkrfbss.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkeroqt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3slymkkld.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jxquqtpj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3iicoxhxo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3peibofhw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pajgjabh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sinaupgd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdnwiimi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wvseadfc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3akitdvps.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gfeypntu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3derejrxj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nnpjznom.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mnnrssqy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yccguarx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3otkxqpfk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cambozrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3htaycsmg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3notftovf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wmoesldg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3awecegbz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjoqyntc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qwbuhhke.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3trgsuier.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xufzvisa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3igqjibde.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zbvpomlp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tekhggrj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xsjxtdea.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ferdtsrj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ioccycfn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hvjarnef.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xyaqbqcw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3imscpmig.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3isdlgiyj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3iyusxgnl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ltmvzexx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cvlnuxcd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kvkvfkyp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cuijawue.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3edxoltsd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yksvjvcm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3evepldck.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zchtkxeu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3smmyqytv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3parckuuo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fjxjceto.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kokafcql.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fqnvxwoz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nszbprzh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3enwhsevq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kscazzcz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cryqxnly.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qbfseugu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ziadtqlp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rccauyug.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kkkvfbhe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3amjlizts.html


<!-- 参考信息 -->