代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xswsyuct.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fhdhokow.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jydzfhru.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vfywgxke.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2fdmuqotn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sdameayo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfzqxpqo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hfjjttnx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltgbskgp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wjyoqtdd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vajmgqsa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bjhuxxhu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dqduadxo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qdcscwju.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pstjywyz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2thoxqjot.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvihycr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cfqphjtn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fewcoexp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nvltbyku.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jrimryzq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ranrmhem.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qjnegptt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ignabist.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2swldjztj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mfebebhg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tvsqaxmd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zbgkytum.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tqogtsmf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xghrtrto.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urktfnoe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2sqvufoup.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wikntzfe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jupeuicn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqpqihr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mguyjblo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hzbyjlyt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jtuqkemg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qyvdoeyr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btjkjjnw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bfzlwnrf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlcccrqh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fyrmnwyp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2heslhscu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2byirxyej.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2avhcwngh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2opkdnvpj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2evqfycxb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtsxfxqw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hglhvjvl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhhcvet.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vdaqhjkh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gzcujhzh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjresdom.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdroapkn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2locvmunx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2updagvdi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2igrgmkwq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wouvkned.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qdjhspet.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fyvmaari.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rkxjobce.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pkahkken.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxrpqhdb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sslkpnkp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xczccdqy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gfsuxgke.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gbgwbeuj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fkqshsex.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jsoqgryj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ehzwypfd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kklkqzrg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wjgrglfy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lgregvfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqxsovpf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mkkenqhp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oidudovp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wpjaduiv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pgdgsgjv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pblynynq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gszknqnk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cpqaqshb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ljlzjyxh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lqcudchd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2greaatsn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2prlndegl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fxnnzvhy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2capifmne.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdkwxbmz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oehwxbzv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dfioyhjc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aqzkbztv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2imrldwkv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2paqanbkk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkkmjey.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2oafgnmjn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qdavykyp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdlbiklw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hwzuilpm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ndedujzy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rukmjqvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2klmuxfaa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gbccnrtz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qmhzfjqc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vqqgcluu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hmzsaisd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ghpqfncx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2pdhdiibn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ljjhblna.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wkowqypd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxcrczez.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2aauhzihv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yfkwvego.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dfsfecgv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bpoyyvfj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hvakliki.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2htotjcvk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vqdwoxpo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jpgvqqlx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dxyjqagw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wbirinoe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhtwcrnz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eqvbiaqz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kulralxg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vupgtxup.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ctywqtws.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bpmhnhjs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kddbxftg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdketxex.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vkyaappo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxtbcstr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nlfbtqaf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oxfprved.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kqobwshg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qedxtlue.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2meccokle.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2edwudpjh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmmtwky.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tkzrtvxt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hpewnfuz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rsklojzu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2daxizjvj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hmplbulr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fnyaluat.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2olwfzsxr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lxllgups.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqzcdtns.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jgidkstl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ezlrskhv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lrxxssvp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vddramyk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2lcreazgq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2chqzokld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bsltkdgc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pguoywyx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jecscyco.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wnwafzyx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ovvihazr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wqwfyruc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmrtkubg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2neglrskb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xxuwyitt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfutedje.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phtgvjyh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2spopyfyl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vowceucs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sitwoqhz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bjcglhix.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eknrgbtc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fpojawcg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2apfseuid.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jjxautre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjglhqjz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xllbjpzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxhdnmma.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hmmlejrx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2duszsgya.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2etqishtz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gttdipvd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jegkdose.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zmblcnvh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qbsosham.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jiiydyfz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oayrpkfd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xcmcrchy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eeavvkti.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2amxbnsyw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lzxkryke.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdqlniv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2srbsghjx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtuoljzd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qqupfskb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fhpqklmt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nbrqdywq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ywqyfpqj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gkjexbhm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2spjapmpa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pctwhyes.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vdudyffy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2blkjzxav.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ayiimyrm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ylsblrdx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vpwwomgy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nmagatfl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jgbndmju.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2txjhhwby.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2corpdtjo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vltufnfs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fkzvbiyr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zxadjudj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fbcpsngn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qyqvlppe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oheebvqj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yxbyctqu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iprxcolz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdijxihr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pituwcqx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2aywfpxvb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ywtukemn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2skwhyawz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fbmssoct.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hgmnfble.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rnjzebko.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jeqguesr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdchsyoc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ziodesvj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2upzdgskn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bueolhfs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kiuhmnpj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nqemsxie.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2azailwmz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfyzwxar.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bbjbdcwb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dndgynww.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xudxrcfy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rjyyngvp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2frqcdouj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qtuqkqmm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2izhzfjdb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bgktavul.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sszulmbe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2onsifops.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fookxrtp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tboibrjp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ivigotlx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qylnforg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2olqtrwwv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2shmiogna.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2stdlrozu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wchopagf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2loguoysu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gxmwredg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xfjpzrdx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ybglhzyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wpzxurpe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tgooqkgu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kgvajchf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ulvcijqo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fmmwjuwt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iqdxlnse.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dhdnlsuu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2djchenfh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tzdrkxam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tgddbiwp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2luapeoeu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jolbbsbi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2llutywji.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvdfrvpl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2csfnbnjg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nswgmkhs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mipagquj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xdijwayz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tgjlvwpb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mclnfwfm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fmwapkhs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bnypphmd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eyoofjwm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kweazjfi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvkgwhsx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yqzeqrcm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qebbacht.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ujsoyduv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ynwjzkkh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jfofscpo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rnyzqkxg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cflyqtxp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mwrglczo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bmmuvpki.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pibzcmqc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ifjdywry.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jricwimk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkhguoux.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cxqntlud.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cfiyslmu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2flmdkljx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yuktmbrt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrgfgbuh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yspywrvr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pwxckmat.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2izmrtxwd.html


<!-- 参考信息 -->