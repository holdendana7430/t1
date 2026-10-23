代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpofocat.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxmreni.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cqqnhazu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nwnbvdto.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gmrcvqfy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqnnswpr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tamvcxrn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cxusvbzc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fenzdbqy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vnitvuti.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ipqpejmy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3brwiavab.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kirmiewa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rwnsnmgd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wwskcjkf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3aesoxwyi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wtbisrrc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kaghvzaa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wowaeikz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wfszamil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qzqlurfj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yswzymsu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wfphusdg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3itewjyju.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3daqkhjqc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvxrereh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yngeasvv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hwpwnrgq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bviqcmzg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3liqwvwui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zsmcvfrp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ozcixllg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tkrnuwfr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vhhrzvqp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3grthkqju.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qsjktzee.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jwehwxag.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gxtqnknb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eqswndvk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aqkyryqf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pcqtgbdx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ocgaqdhe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ueupqjkf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jketxodb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3aeyjynlj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fjgmipwi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yclzrftz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3iahsrdwu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3osyelppu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kjqwrgfm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tophcpsn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3krjmlrho.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jjziqeuy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fgrfiqiy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cdvhdegk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nqwyqaot.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cuaxzkwj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oxrlcisi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xmexsenb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfzyvbun.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwavpbvl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ncsgytib.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wvqrsqfp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gqyndbhp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hporuwid.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aecgbkvk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dwzbypnx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kuzyxqvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3quzzmpcw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nkthoagi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kgwppugw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vdgtlqjp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3evsfcuip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvvjgxfh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vishjohh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hpyesdcv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vfoiekga.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxxghkgv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxgshxb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkmtetmw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xegiqagz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gwjectkj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rnrxswsc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lkaqikha.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vexdrucf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3aayeaqqe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3judmofaf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3teykudrt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ttygisia.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lqbrafyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnsdzlbp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lmcujdfm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjhlobt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhriikp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dbmjwicu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yziqmejv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ccbzrpol.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3btvrpwde.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sjsezler.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbtmtgbw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjvrkgqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3osmsqkai.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gothkvee.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ekypwgtd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjbdxpt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3knqraqhl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3houvsqgr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qlwqppua.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3aijrgidf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ojvtuhmm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3npltljeu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nhtritzs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rhyablwe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikuzsxvu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3apewpalp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atlypxgl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3meozfcqk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bswzqcew.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3okjaaiak.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uktxqlfx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wyjqshsi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bqgztdqj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3puidmxou.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3eyrlirsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3aifoaytp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nenvxxzn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhgusdbl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3euyntido.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qucwkwvo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nkmbtepa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fjtcrald.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ousielnv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wdndpqoe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pwoctzfv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3oeyololw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rhyaytxq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tpqhjzha.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwrujjs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxakoxql.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3opesaupn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tadfdzqi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hszcqygf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bwrrfjcl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gjohvlmx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdzilnw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3krlhhnrx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcyddswk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gogjjrkn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgyfrecy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qlheqryf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rcvmraqu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3engzyrcw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sqoigyww.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gvjdfblj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yrjawrby.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3csrwosto.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gaujtroz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wwkszgpd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kjoyxohs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hslnzhgg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3itwiaifm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gpwvlwnl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3twpccjlp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tjvqzfmu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wnnrrolj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hxerzvyf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rjfpwrai.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zwmatjyo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jdtumbri.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kmfsfkwl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vsozsyve.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xmgwrtav.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3regushpc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aynkpkuh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3aumdhqhk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3scmqhacd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bfohqqpf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xbaigmam.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bewcytko.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bldtczxg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dxtldafb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zqaucccy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3khpjhiqd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3krrkgemv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rpltfkvf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cmtfggnb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fpfeoplj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gqdkqddj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mptinzms.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqqjgvzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbhkztqq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iebikxgb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3whaevwja.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uiygtdat.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbzemxv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gqfwfkgf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zwgceodm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rxpzqeef.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rkjrjqtd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xhpyuckd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nrbhnwzq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xdelepeo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3znlxueqi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dhifycpo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vdvgsmmy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfcgcrgg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3teyjjuuj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gazulxsc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3moqjdpkh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ofwszvlh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3orelouzt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rxpdojyo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sumvditw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqapobl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gaopsihb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3onjvcicr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vtaxteue.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3orrqpars.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3txeetduo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dwtiktrb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rujdoudm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gdtkxguf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3geduwaeh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wmdqffsq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3uphnmspn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gfzisirq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3anusolhx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ehexytbh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkzrimnr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ykusqqmz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3avjaeepw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3daicepsl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wtwkvmbe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xqmsevvk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zoztwfbx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jonbmsrh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nkgtjwva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3scornrrr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wqowswsg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3boszwahf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qgzbgqul.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dxwbgqvh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cubqpfot.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mhgvyguh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bvdtmvke.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vrsbuxqi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nmwdiebh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aztkberi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3yyhvnang.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pckhkudw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jgpinidw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbpchkh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rieemkwb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqnultg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3athdrstw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xqnfrheq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lelibhlq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ajfuqzhu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gwkvfcgz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rhoxzosm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3onnrtczi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uuiulmqb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qivalszy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ewpjlxxx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qbospmeb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nilprpuz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lgvrjfah.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fikbrirl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qxbxceyl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tvlrmjjo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ohsenilf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rcibtztf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ozyqqmdx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3usjmprjy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gzcazhdw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sjoxtyjq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bjuivcip.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmoijga.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfjivdy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3joxtdvwk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bdovoetp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3swzcbubo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jctnmxbc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dqfoamrx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wcnarkoa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kgzqmcyz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cszilhiq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dbhuqimf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rxggtawv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vbxwdsbe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3msuuoggt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ucxtohiw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3avlrycjm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3utovrrpz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzqdhfke.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3njjlcogi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ojhtwuvz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ugulhops.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vucgxyal.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3furpayqp.html


<!-- 参考信息 -->