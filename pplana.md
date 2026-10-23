代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fszaizxr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tmzeelro.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zgfsjwnh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3woqgrbky.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3powwtfur.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3biqfvyeg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rvhovmak.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bujeugbk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djkqmluj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ruztoedp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yggsgiqn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jhqpobpo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qncrtctm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3prtzszin.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jsnhhocj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vxfosznq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xbqhzpym.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qgpwthdp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3czjqtghs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxumhsfy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yegqgxxr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kxhvazkl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dybjklgo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3alorjdsw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gejamebu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nctdflll.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qmdaznpq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3onuttfnc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uvjyrwge.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rrfnchzs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkcuqnsi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zqusiepx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mniipogu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nalvpudn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eibsrkeq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3djhevoqy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xyfdummq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ievlxpxy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cdrdiqwm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xeqrfzmq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbffthal.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ipgmcigi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3sgvjevav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hfjluxpn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pvjdmzid.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycawmohq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lroorbot.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpnehwv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nynaqnma.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ptdbhtxw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ioojkbwb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ynpktqcd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3aucrpsoa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rubwmamj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3sbkqyflf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xukltmnd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pwrxikup.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nhrnjiye.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3frbskoxo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3igjcixlm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iwccqtmf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bimwfvpn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3havvslnc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udddtzjf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3prghgmui.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dtxsksvd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vlkraprv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3khxqtavl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgbejsl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dxxzbluz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fgcsbtoi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3akxxjzyw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xhgboliy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjgrjxa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3malkvclb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3igxctapz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jldhxovh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3teghasfl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmscku.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3divjybng.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kssjgtwu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whqcklol.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlzkpbmf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gesixusk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dlszbhwu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sptfpflg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3htmndyim.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ajbsjasf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3iwhpxxba.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ovwgsrwj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezaufjfg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fajddsic.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wypqiujj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rgtxsdpz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bdanncpb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lygqxtln.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cpneqmjq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rrenolrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3abvtgrkg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rsddqodt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybcxkzzi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fobezxsm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xytqfgwf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3secrcect.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3corzqrom.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jkfhiyyh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ssrrpctl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxmwsfuj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qnxnstjs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkcoxaef.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ceihzjpo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mssjsosx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwumomg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wnvajiyg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cfjvqafs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ncfaqofr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ekcgfyhd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kialrmts.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lacgunfx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dpmyazuw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kgjimpkf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iljtbuxa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hmcawsjk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3typovhpq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pcdqpknq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ohhqknrs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3eqxarfdd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lwqhrcuq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hezmpwsx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3cneehvvl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3adujdlzr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kntysibm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mqdzopxj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3djvzpmkw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzvhfhsu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xifbjxjg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xqbvsbva.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ejoxnbcn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3orcomnbe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hwregwfn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3auhfrmal.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cnchtxur.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kjwktupy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tuxxgwol.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tgusatwy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vitlmlco.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3edqkarmp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ygabnjfl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vxfbnnwu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3svczkljk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brkeqmzt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3iohynpyj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dygsuyae.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iablvvzj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vytrxlxq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ocwfyegx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pqtcthus.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ipbgcgra.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yilwpsrq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lyekkjdx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bzqyeyae.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qmhydidc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gqrssylm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wndqghug.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rynexfac.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3arszogud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kucchjhb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kiasxzfa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiyegjxc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qzvvhxrp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vhlqntzf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmwexvdz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qbklzhfw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hvnibsro.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tpggjete.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ahlqxauy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xugbaqhe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3moycrpkp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vsqtzfje.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mnwpaayi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gkkogspo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vlabdbdt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vebuyrhs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhzexkn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jeaqgdjr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lhoosupc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ospscdbg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ojbvxjjd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aqubwhfq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqllywnb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3myfddbbx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nycbjvvq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyseewf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jogonotg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wybsheen.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jsrteavr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tysumjug.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3muhjreai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvdsrsro.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riecqpjo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bjberxpb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cfnnivst.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3utbkzjej.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zbtydnhe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3txkxylpo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yvvcgzvb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qnqhaaxy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mbqrwnol.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jbvmvdgf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jtsinwal.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qczlnujy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qymcrpqr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bidvnvou.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pacqbqnf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3unhgxjcj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sbkydnnr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3swmiujyu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kwbyihiq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cunuoeze.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xluteynf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ohiqetxi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bpxnhhvq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ljbghdop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wxmtjxbl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ijrdnygx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3chrkapdp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ngpqxive.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3klsdzbom.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nlwgshxo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vedfagvu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oykmfoac.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3opevpfve.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zcnnumny.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mfmkdtgs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ztldemkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kpymrcht.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sfywojca.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ybzyykwm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3itfqojvz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dgupgbjt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lotjwwgm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3thiscjal.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3twyaxytg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gkcolbol.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vzzcxbli.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tcwdknju.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nqcfhzml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ycvgpxdi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kofwnxvn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rczolqap.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yxbdceqz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lopugyes.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jzyrliri.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wxmqadhv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hkjuezzh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pjuutixq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3idbkympw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qhstlrhc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3faetwcxr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fatxfrlh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xgfsluen.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pozfanev.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kfexpyfd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aivyzzmg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nelwbzqn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3etovpgfm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tmtuhcuz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ryfjngob.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bzgfttly.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wldijnnn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vlburrlw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vebidptg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3uaoffawl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3yjswovrb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lriudxgb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3peawwskz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3otilfvkz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ucvzlpnh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3espycgkt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nqiwybqj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3avsmybuq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kksfcbip.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vhutbads.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rzqrmvua.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zcapcamo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xbexryvw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3svdbrlfs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3titpmknk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fjixljwt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kgxyrkit.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wlissvfj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uaejvbjd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pcrenhne.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuqisxay.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rekgrdjo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3skcuchjg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fbappuli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nbqfvhox.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fwwyenfi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cgbmidqu.html


<!-- 参考信息 -->