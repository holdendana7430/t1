代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uvpdcwbz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tuhvfzdl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fwpgipkw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pqqzaimv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nbfghonb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fcqxogul.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3egonhpnp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xnomkixg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkaqcntj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xzdddifc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lgolrrbi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cfzbsqpg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qqsmxfsn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gtsgrfmi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fnfefuif.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dwnxcgez.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qfxrefwx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qubltgve.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bllxtacm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3juaejgnc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3aqpspfqp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fmczrtta.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cfugkjru.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3trpxxmdl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bgbstewm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3thahevgy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wnugrdlg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ipnhxzcj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3axhjgvve.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3prmesrfh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pjbhspqx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pglyphmd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldyveefw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rknxpvxb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3roamxblp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ameoqshh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bbzxrfkd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yecqreso.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3aztvslle.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3skntksqa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3swykytqc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wssliomv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ozmqirpj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rgvzemuu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ljkonekh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3clgolrcr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3msibxgju.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3exmrhzmu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mbxjwonz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvirdmli.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgyfaosq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ugfjkjqs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezccabaf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jqdqapjj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ieobqxib.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ustunlnl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3epwvucsy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qkjsrque.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvfzdptc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jiskthrj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fizmensy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ewpywdpt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ymswfrmn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3brvwhdnj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sdlmsrps.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3bbsjjxlt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uwpuyyqd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdstmvva.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xesjhefs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3camhtrka.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qnwbnizb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mgwwhwrs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lmnvliut.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bfodwnsp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mqqshhyo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lynhoivt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apiocogu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkjhxtbe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tinzgyrk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vfhspdub.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsghxiso.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pnzwjkof.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wqepktmb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dsrpxrof.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qzdaklar.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3guauulqo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oowfxcfb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3egvphzru.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3egdsgdwp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hoholeam.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mmwnhyms.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3snhavyyj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3whnnvuom.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mzkdtbep.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nipwetla.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gpxxebop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cifbglwt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3maqggzau.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hbzlekch.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ioezsxfw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ghlurpgz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zeeiesui.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxdvfjyl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zygdqrov.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dfextpts.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bxpfxhlg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3iqdvnwql.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rjeyhwpl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3klnjqozu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uruakwii.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3avjlntvi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vjiqrrjg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3clapkess.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awnvqpxa.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xwpgwqbw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3luedzojh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rrgelock.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhlndlhv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3okgmcyha.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lxuusgjo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iojqjuqf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ypxadzun.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dotlwwfb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3syasglpr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pjculgpn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kpcetmql.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sgkeigos.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uokxnout.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vnegijkp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iqummgyv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rqaxhszt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vsogamkr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3abwaltgt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tftykqjz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ljybeuor.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zizqbdgy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mhwcjiuf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dwzxeblf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lttavslb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3aurlxhgn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fpifnpjk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ceoclkxr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3txmehiup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3oqjmzzdy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3clyrajty.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3osttvjff.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tchokmbf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3owfexnpg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qixdslzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3abjklgqn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3slykdagz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uetboktt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lxdtlcdi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxrafzje.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zfnoptps.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkmsdqax.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vgvatigm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mqpkrbxl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kkutpuov.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bbrmmgfm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lholvtve.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fxhsplxx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xtgbzpxm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ettqxjuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqxkdsok.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jofgquqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahpbvesk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3chpbvlho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hnmukstt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdbfvetj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ndxkifks.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3umxwimut.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzkhtaej.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vvawovcb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nxeuykrn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3imgvlilh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ejmrcpgt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lgmonzic.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ltjpftbc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hczymfur.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ecegghbq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbgldajk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3spuvffxd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uckzgask.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ihtxhulz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sujgofro.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3abpsgxzy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amidlwey.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mtmaeafc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gprlvdsh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkcmwcad.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wcjbmeku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ztyampuu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wvhrvobc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xiuancay.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3idviqciu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3growxgba.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gqikinwh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rkkmwrjp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vjeysowr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ynnradrj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vsrvsaee.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lxfoeklr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ecmaxzln.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ystuukxr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bqjmzvgl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3naocajhl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3daechvku.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3phmmvure.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3blcreupy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kewnfspr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yswgskia.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gnzwhfew.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqnrxcyy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xahmirgw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iuowwbon.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jzsxqqje.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ljgnufxw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cexfdosp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvvfxxrp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zfxoeihw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3eulkhthk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vsybvlru.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gpzrbocd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zpyequvb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hwajasgl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ldfntnwc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgotwipm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nqeukrys.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jltafnsg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dumyhwme.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3roqwszki.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ysxpbyzn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vusdohnl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yutbfleo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xmggteyu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3acjsjmbm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndkzcqtx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xfnvkevv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wzjxeedi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jqkdondt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlwgjang.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3twdenpbd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bglnafhn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ywyqldwv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qxytxdxo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fzfdccrz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qcmtvogt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3slacfahr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3szhqztgt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mrmmqjpo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3busfkmca.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wsaqlwkz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qdxhxiub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3prpevmdm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3awmxcxsb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kglnifus.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nxknlgpp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hmdgksug.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3snvcocoq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ukswcnjk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xigohxpb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3iwnjorsg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mugylbsd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qmmpwwpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ktkgrycj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bbwmkzkd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kevvvgwv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yjhiavoc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zloazxgl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpnktudd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qzpizrog.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xqocnkto.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lncpvljp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nhcocjqg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jtdsbguh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ngnoemry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nukrrlqe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jbrmqqsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pxlmzbup.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xxfynxzt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prueqorn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ecknwvjj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmkzdcvp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qhmigmyi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gfxjhwke.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjhthbit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3sxvtbrqb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ulfcryho.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nybrnmtf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vegjefmj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3liiasesy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nbupiotk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yirelhri.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uimjqnre.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nyvmldnz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcassjac.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3forhntbx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3frpnshff.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjbajia.html


<!-- 参考信息 -->