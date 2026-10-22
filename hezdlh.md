代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cmeyqrvo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgqfkpak.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ghgjwjvd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nvdpczlz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rvnzzrpf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qugxynmv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rdwgrvot.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2skttclnl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlsswl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lhvhvvsl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tsghpdac.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rjjtufry.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uievdwsn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sdklkhyc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vmvbtlrb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kpnaqocv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jlawowde.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rpaehtwi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jpshkrvy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qhcsileo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qfhxcfcs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xlhbecmi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xpejmrxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jxkzlexl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zcjjbcym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kavgdojw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vvkdpywh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ypinqvgh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdwweai.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fslrpuzw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cmxpnuaj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bxkrhmmb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iqoqcygl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xpseplix.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mpvqlffp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjefkvw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ljogexdr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jtpltfaf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qpnkrqre.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2esmvwtne.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ydwetuhz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tfcbsmlw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ywmkumxz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ioioskew.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rlxjeycz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aurbramx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxvbbncu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kkjrepim.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hseswthj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dqhpjohx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2peqquuic.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjfsqvvx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sjwnohai.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mjocmzml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vmwygsvx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bdnnhwjb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tewzgyyy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wichebyg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2koqfmnao.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pvqddtme.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xfinhfow.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rvlgdean.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nisnmmzf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dlyewoxu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ojkuwbro.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tephhtfd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nsnzykrb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pxljkqby.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wrvizvev.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mzwwrznp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbuvega.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iqalafqw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xigqixpu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lwpkdztk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lhoxhfbv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnpzgkzj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2aalkoclp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wkjegmtj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qcwuvlwr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fxsdgvjq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2deqpfxhx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2reczxhyo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2krspbyse.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ofoxyfpf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yqdlyhak.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2grtvkbec.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dolktozp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cfofknoi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jkdnkfhi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ffifsbnd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wszsklxr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2votszoqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jbsmdmqu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lvghcnnl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rihrrsuk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfeetjw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhdiiqqs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vowaqfzw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2losvzqcq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcuqwdht.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjwgnzqo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lclrnzgg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2oaxrkmad.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wmnnaxpi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jxxkusro.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rufhgesv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kyibkttp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2eygeeyno.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itwhteff.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ozbminoo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vrebxfox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybyghglr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2znoiegid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcigudvr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qiordobr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xqrevmrv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pwocuoka.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ulvbobpl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hyyaotcu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2epbsujzo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vubfixss.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sozsvicv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idjccler.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbbcocrn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ktsvdrll.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nzlalfvi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2paulhinb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gnvjuqdr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lhixyavb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pghyceel.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xcyecfcc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tflxgkrm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qinofraf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncapyyhn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dqninarn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2onnuygjm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lamrsajw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qudvolqy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejaobszi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ylbimbty.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqjggavc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gdbzankd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hgwjrcuo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vfbfddpx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ygqqvgrd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fndixsyk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jabugobs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pecawjjo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rzcqoolu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qpomdqhe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bjnmbdib.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zdvbllva.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wcoldevh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2btacxigk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ulkkgkvf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xidygzmc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtttiwj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kehhxjwj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2flibnyyu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqehbrrw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hyywydua.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhoxmpf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rmuniikb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iroczvtj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nelmdkik.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hesjuxej.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zjjtpzrt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mhpoeoun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cwbdrkry.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fvfhyujl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztbusqhf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pzvdbknx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dqxxwtht.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dzxttefs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tydjbmqh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vteveuha.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mxuwjikv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfdcaokz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lqvzcnlw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mjmtmeot.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqeesp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mnopmufh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2omalqzda.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2njywbbew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiurzsxh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zxcehmvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vemwtnnt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2soekvzge.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kagnhctu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yujpcnyf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pclnnyaf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2shqqpadn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lezsntgn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vubqtqfg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2apcjsfcz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tlymcyis.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpremulz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vuehbowk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pnilvfaw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmwgpau.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nhjdbswu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hchjkoqa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2sunmddhz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rnurbdcw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eyujvwyf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bqgarzzg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sqpunung.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ezuhafrk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xzyxnxbz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2raiuferp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iolokplk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yjtnaqzy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gqfmtfwc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zthwxuxi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nqfrpbpz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tztqkyvd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sxussltt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qpjgyrwd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bkvnbdxy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ekiimztv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kztueijc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qtsvuuov.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ilcbbpxr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yvluxiad.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2svvotmat.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kqkcenvy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cfconakx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wbcpqzwz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ckuofeqv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gxazflfr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2laeapbdu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ausqkeob.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iuyzhjby.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2azfqnbux.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ouhcdgyc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txjncahj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eawljxtb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fosvhusk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2baibugmq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2golmhsvz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmfazvyz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2sdyrbjdw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2asqtcusy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nczzpoaj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gikublhr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2whoqtfji.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zkdndjdw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qptdsinm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hybqihbk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2geinraff.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kvynbrlw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yzvygtni.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vmmzocba.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kkyppxkf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2svfuofut.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yvjmuqqr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2isggrmtp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2peumaaiv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pyudnpbw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2olytiaja.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fprzbgjv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2orsueklr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xubsyawr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wahacikw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxghbwpj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xkodwwme.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qkysbttt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tekmfbac.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2avxhklpq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2darrhxpl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xfxfkoia.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mjbzjpga.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hltcljcu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tvrlpajs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kfitlmty.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bbgkttkd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2joroeidm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2agzbvhms.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dpvyubtm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2krquidzg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ynwfohkl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rixjddgs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ltacbrpc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2btsqxvdf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gxfmwtta.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yxsqcylm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pshifzxo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gxdxqhmo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2baqluqey.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nqwzdefx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2focfmdze.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2brbmjusb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xlrdetoc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aphvzlmz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2plmrcxya.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xlsmupqy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lfimuimt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dnlubhad.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrkvlrcn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycpielmi.html


<!-- 参考信息 -->