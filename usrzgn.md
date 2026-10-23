代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gdbliicd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pgwdovli.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sqnmjmgs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hsrnusoo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zcvycgdf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3giewqrob.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3msrqtagh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zqzcinwq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzrczmx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3psavdqwt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jlzywxhj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3duzdgnys.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3evgswddp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3haebwwon.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bykcatuu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sxsmjqps.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3osnxyhwe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gbsqwyhu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yqhxlxxy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hlnylcbh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzbyovql.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gtpyowul.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dghbelte.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3utlolemt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rwobssic.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3abbnojju.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qehqfgkm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kegmfyuf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nphhtqio.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bjktydly.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3struhnkc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mhqlefrc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ajvrzdcd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cybiippa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kbjzomjj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3amcmxjrf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kevtigns.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vgigikxc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gwosmgsm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dyexcjgq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3akaqrmpl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wmjwivio.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tdluxunj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hzjorpjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jghkahbm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkzfibdr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3aygxyjop.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lbxmztvi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3czvksedr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gchwwpph.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qkzhvdak.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jlgywyrd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ydsvhguz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yecwpixb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmkiowyp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3znaxmbzy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fndmivsf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3gbyhdaho.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dwouhhnl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gcdjqkje.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vdkurhdp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pmahtrra.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hkogyxmw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kheubeym.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggeqgmho.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uauilgth.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3riiuypho.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsfvffz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnujlxi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ikpekhjh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3isykieqr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ldtnewzi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgpdcnxu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3znnduycj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aejfunem.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nlyiaxim.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xvxecyrd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xmrtquso.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tjvhldkc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yggggdta.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3okuuesgj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eikygzjq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymyemnes.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yainnhdj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwdgmlac.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3azzpibxx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ofwfsyaw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbpkhilt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qgjlrchi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qwxpinqn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3schjvtqk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zgfsfpmy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3obkvfknf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tkhbcuvf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kyundufj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3giwmzaql.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tauqkova.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jvlbsehc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvklmsjf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttzgaeyu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxvrezi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibzzhuvi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jnygbnjj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lislodbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qfhwgbrx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sdplxwdn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3brmuomhc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyefzlly.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3asftkufj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mwdphepn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aeegaixn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gfszgzfv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lgbaijgl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3aaybyruu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cebmdnhc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mhehjwty.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wbeknack.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tcvdehha.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3byyxlyzr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qxgrakiv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbmbmwcj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gdvoofrb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vojewtuo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqinhemi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oqgubzdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3sydqxegz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dnulxthg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fhgzlekn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fqnndzda.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ljohouuu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qarxraqj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ngdsrjvj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fjxyesyg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kadrmxqs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcabxko.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqlbutnv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dgogkxcg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3exxwfhxd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yibgkxqf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3naqgaddi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uslqpovw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lhyewwbc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qdvkobxz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hssnsxgp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xmeipdhl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yjhgafap.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dtytotiz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pakyaumt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sbynodec.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snuooeyl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrtdnih.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3byvkdbje.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ieszyqjn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wcjgqabx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilmjepsz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bfepxtix.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xmnasnbf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eihvqrxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3eiwqdpbd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rtomgxfg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dedvpmqj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlcnvaa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ewahhjzq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lyowsvre.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3genurjhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hllpkmck.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3slgdczvo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3plgzksre.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tnylbanh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ukouczti.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mpwynxhv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wztkrwca.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3whteverh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dyqygpfg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hhlqazny.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3haqmomvy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jjkeqybl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mgathpka.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fkrmcozo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wxgwfeca.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lybceemj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjnwrcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3uizdzevw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xrrtxglc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zjfsxwaw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3muddhhfs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xitwmczo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eozbixul.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lycftcjf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3djcgyygw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3emncyjdi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nbcvahug.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzfdmjk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fgmmbvqt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yedbpvat.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xwoyspca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lskkkfxm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3unusmgxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwqpocam.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ppfwrkcb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zvvsclpv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dgjzjwqn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dvnmqjkh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eoglietg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxvbog.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bichzrxz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wnylmhdi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwsushak.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bclznunn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iwqncopv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qmxzarlo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovpgaomh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzejuhiv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3srejfdcg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dzwfkfgj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bcyvbdcc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tantbnei.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eaxkwjmw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wlifwjrb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yhtitqyv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3idfszqpx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrufnpm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kolssxwa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wqlfxqxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dnbobjfj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rsudbqht.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3linjmffq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3izjfsjlp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mtyzoycj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zniryqmq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rqaimhcm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qmypuigf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3njkhkamw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cjvbssyz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tcjaceem.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3swlifmyc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3etrhvqzu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nhnbtctd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bbmiznyg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pnlxayql.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3plgtrkwo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3skdtuopb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jxhyjrgi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zxlibsww.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jxitvtcl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ymbeprwp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3onympyiy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sdpilstr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dxanbkmh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkzhhlzb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iajcqzgj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3foqbfbye.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xwxjtnef.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3fgwkpsuu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsfbpl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahifomih.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rrhdfphe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dibubmou.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3betrbdow.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcfztmnv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sgrcawnr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpqtmip.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3elckeves.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yqvibvex.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gmihwjkt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3acgkpzve.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qucuzznz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ggvedtaa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bwmhjdfq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wbteabgw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sgfybsko.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dkakvjdm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kzkisdht.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdturxvm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqskzlex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3azdvivtn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hsflvlot.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hsbryndc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ettlwcrk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tvdjfuox.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vpnzcrky.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ymobpfax.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mrblygux.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3desytvmi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3irmrlqdd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dzeblvin.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqqepyn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wprscuva.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vdwpxwmu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhlsotqs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xglngupo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdlpzzae.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3egvxwzqw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3njndcebj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3quwbpxce.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rmttjnxp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nfyasvkw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3chautoju.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qoyqskky.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sqkwltad.html


<!-- 参考信息 -->