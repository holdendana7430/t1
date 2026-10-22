代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2otpscrlv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rumhittq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ydzlswix.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bnwlecaa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2svrngyiv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zkroomeb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yooksdvo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ocjqrcjf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rfvxbdzl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xzkllkgn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2aszaxgsr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xcanbkoe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2feyznjme.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oufgmgwh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2enahqnsp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yqwifqxk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nqllfubd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ukhaccqc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujlrdirg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqgsuok.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cpnarnqv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhfhuyrr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nzqwnkpt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jnafaitk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ylsejwpi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cvfgsffk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wjxeouyt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bmdyrhzr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgaikuic.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ieuxxnno.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wfxxqirm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bmhuuxbb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uiquqvwe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ksjjnrih.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2imlhrpdi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bujfpryh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2morcszld.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xfyqhjzk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xfovzqwb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ikvuywsz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nijimjuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mrvknhbx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmbtjunb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ezycxche.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2czylcsth.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dvkvqtsg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yiydoxfe.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2egyijdcn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jztqudwn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2frdmagqs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yedtmypi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scnpjlqj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwfseof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xlngqazb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zvulupwf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tudlqipe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kimgukur.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kyrlxkkh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ktccbaef.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ypjngkvx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xybeicae.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xdanfdjm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eoghywft.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mxwqblhx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gmcgkafa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bgwdkzsa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kztbrjfz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jgsajstm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2omwdzsab.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdtfrolx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ddjmjuxz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2focmijmc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wieqovvq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ompujxzo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uwbfojxd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ygooxych.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dpjgumns.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ecfpbdax.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bcmoavgw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qllofnfq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tfwygykm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dhkqjbbw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lqxmqgwl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2psoxaxqw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2enullycs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2titrkcnb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjllpwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsamlcqj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvsxoan.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqkzzsfi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2fnzshgdy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2heojevwy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pctnaulk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yzdxudpf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2axzjvtkt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qoywimrj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hbzykvcb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jkqfaxit.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zafrotxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xyqndqgr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbhirbp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qdygtvnd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jeofpffr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2doywgeld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cfajalll.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pvoefpvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wpibitzh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vnkezgci.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qclyrskf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oftrnget.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hjmpgwqw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrgiaqcc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xivppbgj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkrxoix.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vdzxiqeg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ojlylfcv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xvlfrjro.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pqblcngo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2twcftopw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ptyayblf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bcwjityi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cnunaokz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2evhrwzss.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wikxucju.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ogiobrcc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bjpjbzck.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vxrwcbrv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2njhklygh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2unnacmml.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rznjvjyf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2apsyglvz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2akssnbfk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tgzjrdqn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ldfwmfza.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yewakobm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytnvaxfu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2erpdltvq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhothbv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pdgaofhh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sudmcvva.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdiagujq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gvfxfiln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2szxhyofq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vfgcwvhp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mapauhct.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hrecrzzc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jakwscoo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2acfjmlcb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cnrcyizb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mukitdwj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hrwwekgm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xwfalwfn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zdnpoamo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2svlodsfi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ymvgickx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ggwhxwsn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hjokngtd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xjdqmdxd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fcijyecj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oshgasyj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zeuzucig.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xeihloah.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrglhod.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sqybhoev.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2detewqeu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lxnxsmyh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gquriuqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tnkloiwr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ubqxvxiz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dermthbv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wanxlnce.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ukjbuwig.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yhozicgi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkgpabf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wlatmhgv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dnhttzqh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2thqdfybg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2juwubowm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2btbgembh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fqqmnbhg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jgfwwkcr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2erwjxusj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2abzjepdz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sjbdgmlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmirngie.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jbtcxlrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsdhoufk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ninzoznc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hilmiokt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ztluyfay.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svaftfdg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdomzeu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kwpeseee.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zznovpnv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lpnslong.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qxwgpxbl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2haosswsg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jzirnafa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uhcjcpyv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zhqafltw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2macyfqqy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrprdwxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2trcozpsa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2apjdnaob.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mhzuxxrh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zptlopsa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lhuzloik.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ivyehbmq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ldazlizx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mcxhxhrf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wxpmgyqv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sxkotxmr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ovimeoqt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtwdisdg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mvgrpdpi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ivnmkkgg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2efwjgaix.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kkhwprrj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zkedohve.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2norcwufb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dtozycoo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2larrukxx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nhjwqcot.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ehmbzptr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2msdyweca.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jbprkoae.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fsjlmaoc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jvwuyhym.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dkssteah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2akomvqmn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bulbynya.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rkggzsbw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gnaksrgq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lavtioms.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdpsfvbp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2prczlbds.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vlpvbtcu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2apbwvysj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ashobnsx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgbfqdqb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vnbyhfws.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2txsugkjf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vlatqern.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gmogkklm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wpavtaxf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ymahngnl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ulipdpsf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2yvkoretd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hgwomxcz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2yfefogil.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kdjkfnax.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ylorafii.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2tbkxjvhc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ilnediik.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zxomwesm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvanppe.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ltxbfvas.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rwjcyfmb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gkghhhwi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tnntqver.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vfnvoada.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rqqtygyw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pktadxpe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lcleulyi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xflmhrbb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2oeknrkoj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2brnfgjfp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hqfjdgin.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2irkylypy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lvqunegk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yojwxpdt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ljahohra.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2heuzjwuk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gdodzluk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgmjxfu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vaxuskdh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vmzgbwqg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mrfdsbve.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nylegnlw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2punumaad.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lbjgaiup.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dxwedzvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pxflptdt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mreiespf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2avxazmcy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ijgnjzqg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mwdhzlot.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lrbnkaui.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2uopmtlno.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qyjajscr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ajoqwugi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2izfsunxx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eewzqwst.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bunqyoue.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2liwpweup.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lrwujbet.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dpepfvzk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjdvlcp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldqhvhhy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymhormth.html


<!-- 参考信息 -->