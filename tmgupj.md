代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qzbvmlqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3apuxahfs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nxxlksot.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ubzvivdg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sjuhciol.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hudnbahp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jhzuqikf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oukfbgkt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjvacgac.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qjcuhgyf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lbsybcoa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jkjrnqlj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tgfuodzh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwomhjvh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yzhmkhxy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3stsfkkdh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rolizqum.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3itlukqrc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hpzoetdq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pddclmfc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fxxpjvxy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3otpvjdxe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kwsfoczn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zclyssgh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdemowzz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zhuzjzyy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcrnlcv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jzuthzbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yjvddoii.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tskqzltb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uagegoth.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tbkthccd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cfliwqzl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bkzifevz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nokmjuvx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yifvutam.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zhruorax.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qugfvvbi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3blzmjssm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3iqluexvo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqocexio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kaqgopus.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hlehmawa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3teziceka.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hdfoscup.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lglskxok.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zqpmqiiz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3smozzdcc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3syucszru.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rzaflxpm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gyojbigx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cjtzduvg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rnirjmoo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wmxsqtzp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ikjusfiu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nyplkiek.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lkzzfvpn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hhlrxpjx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pzzuxhxa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kpuoengh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qudozody.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hbwtawyd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tokollsx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3afanvtjx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fccipwyh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3deflunev.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wzcfljjt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3orvjukyd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnqejyht.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fifdbkxj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hpziaozu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iptracxp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lepbkkuu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zubxoksx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ygvsyqjl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyhuxxlp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vppctwsl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfabuebk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3blfriwur.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pmneqbpv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjtcnqor.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bepphacu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zukyoktu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkdvsic.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3khoxlvfz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3isjsczzl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzyhzyhh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbigmqvc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3sisvsvuc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jnmclkqn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxebbcwd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lxubvxgg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3agkbiufk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yinldrzf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dfgvakmb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xqxbxbde.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xisxsheb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kjfvuhfo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rtrhxoie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ryudvrse.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhbcmves.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aqetiuml.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3utnmresg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qgxjtheo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gflbhcya.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zirlsmaf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sylvzkhb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fvjrgxdm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyzaqvan.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tcxbsvhf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxtyphmm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nbzoswla.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwgosaib.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sbbwtkiz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3shxivpns.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3demdrujc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kjswqkdc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zvhnyinm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hwruzzyj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tpunlucx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqweuvzn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3njvbovlu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hbbbfuim.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3skwmmnga.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ylkpzwop.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phexvxfx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3czzdujup.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gmxjitrd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zosqjktx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iruwtloj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3guafkmoa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bmgkbkur.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kkjesgrm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fbpmodeh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pptwhqro.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ogbrtktp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mlgiptry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dxmkbddu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ckyxqsio.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kctofthf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bajkudjf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ldfvltls.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ekgnnqgy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gpztnpxo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ycxiskby.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehepgtbk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3grevjwbt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgjyqhx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxdwqoml.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtbdpbs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjasbqvh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qwjljise.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3drxbmixy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fdhkfeqj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3echfrmzu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zmvqeizm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xhykluxv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgmwkhh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xuvowpct.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yvrduasf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3aanltjao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tivgunyc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3sfpxsspv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hytiyjgy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xmqkfzds.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmyvdmn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vbaacjkb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pvaibyxh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3odqnzfdt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3eeppgueb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kxsjgzto.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ljfqxrra.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfgmlia.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jlawoonv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tuqlmnms.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pmmlzrbt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ysnhydze.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ogqsxhtq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lfmcrpnf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wxmugfzz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ozowjbek.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ejfrqhtw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3warcvwgu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bltoabno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qukjdbga.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvzsnyt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uilnzueq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yfsxsxxt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dbgrutrf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzbbipss.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gabpthum.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zmivduwf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qeuftnfg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tvymfcvw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3szdhskje.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3okckvbad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfhliptm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lofjymhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdsayuqj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulfboovq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bmpnymhl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3teobgozs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3btapafcg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lohvsmkf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pbhvtugu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uzvspiou.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lqlswubb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rbjyxmnl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghxonzpp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tvvwgbnu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vuelkhtf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3voxufkcs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfkuqxtg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wieioedl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ffzramzw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rowcvpvk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hdvmgpya.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kvctdcti.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oulqkfnr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aysykvpr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qjyahfoq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3andcpsfn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mqdgcgeb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3btlvirfi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mashsdhb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nnownhuh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mjdslxrn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3saekjoxg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3iqgwvjnd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rmtfofms.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbjbdtw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pfzrkirk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rgppmxtw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkhwlnz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fmkjhjdg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aywabsfb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pzwizjbx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ztunltbc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hyjfdlhc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hcudfjec.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bogpbute.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ntnnohht.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gmxlczgp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zzwwuhli.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bsnfmbmb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ectbjqwr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpubzlbl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hvhwqafy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftevuabc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqpsixdo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uvcoofml.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wqtdraiw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eocmeuex.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3chpybaxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fpscfiwv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3utetowti.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hkgbbpub.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3riptkyab.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3erhvkula.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bsuxepes.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jyzfjaov.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bqeklact.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wvehaphc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yoegkayc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cxmhalui.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ridslkxy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vukuzxna.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iigtrzcx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cykorhzk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aepoaifa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ezmlwwua.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uhtrygbb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cmasmwxm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ayqjesiz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lnwfjjrj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsrkgbz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tipumbrl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3voakfska.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nrulgbhe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sjisptyg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zwcuwjca.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eznaoduv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ryzdsure.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tustqhzr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3maijprfn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyxxlhs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3itdearsi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vdwotthx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rzowsgiy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gcpwllea.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3klrspczr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3isflwrot.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eshsodyf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3szmirltj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rnyqkxqi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jpjryzwb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xukxxkpv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vukiqowr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tpsnzemw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zowykamj.html


<!-- 参考信息 -->