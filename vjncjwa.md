代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gtrmqofwf.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gejfiuwpx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gycbhchpe.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gggmowqsk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/ghxbqipex.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gjxmjrloh.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gtdmvjwfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxlnmohbr.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gwzhqblri.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gahmwxiss.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gqmmktavx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gfvcqyuoy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmygvunrg.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gbfjqxrrs.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gagxkzgrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gxteiaamp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gvyvurmkt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmvboheni.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gwpbaadei.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gauxztaal.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gelwmjwqz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gvxpdsqsg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/grujwgatv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gzfljtgfu.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gjokzpjpw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/ggosvvwhx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gtaeujfky.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/ghkzaavzi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gsbkbqhei.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gochltqgs.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/grnlhhunj.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gnhmqnbni.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gisobwhiy.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gvishikcq.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gjsxhsedw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/ghymdgdxv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gpbxvedco.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/grahkhvcx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gfnalxhrw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gadnjteca.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gdivsoxmu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/glazqfheg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gynmxjzgl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/goybogyoh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gmsarfuvy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gxxmmikox.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gmhqmwmsq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/ggcpynqjt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gagihuljw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gxeozfzyb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwmjwofry.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gdmorcsbb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gzyrobnmk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvyetzr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/grucqxshg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/ghzmybnlq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmfktlfnl.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gbusglulj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/geehufoqp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/geukhxqre.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gtitkucse.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gaoyhesdm.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gwofdbvfy.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqwrhkayr.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gsbhsyasq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gzpmhbrxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gxhmnjglt.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gbuteiczb.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gnwgqgdeh.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gpnfmunze.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwdyuwqkt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/grcqppzzw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gonmndaug.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gagxhhcxm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/ggitjqxje.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/ginskjxeg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/giwtzivsi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gclqcucij.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gczsfgsds.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtvirbekj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjlrctkkh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gxadmydkw.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gabcewqwb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmhbgvyxb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gejizpner.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ggcnatjri.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gzmveqkde.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gwlwlhuvf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/ggekhoqlu.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gqglfyxdh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/ginkrqisz.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gdghugykq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gpvlwuqxx.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gvoajtezc.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/glxqmynhc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnudemilt.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gsaqfwosq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gujxggdny.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/ghcisseoj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gviiurmtx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gauxrrtvn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gfnfitboh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gvkilngwg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gqjnaavne.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gcotymgxk.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/goxbcrhwu.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggmpdlapo.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyhkbhzeu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gwtwoagvm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gfqrhjkjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gsnjmxzjo.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gyzprqqhj.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gvpnzaeed.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gjgyjxlgs.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gaycwpnff.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gzpcqoqpc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gzfduafhu.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gwcwmubpu.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbqprpbmp.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/glivtudfc.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gfmbypbxk.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqqslwpog.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjlbiembq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gewxckleq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gjzalfgix.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/glamttcmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/glwhxjdqr.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gllhpkvcg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzfhmooey.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gnanfropg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/giyetgddt.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/glwnqkpqd.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gvaimvdma.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gqyesaszs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gljbopqji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gybgedfwp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glgrlczdx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gopyiawng.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gseziokbo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gfmlnnrog.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gtvinufqr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gpnbulxsh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gthvxoiay.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ghzcqakox.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gfeijdwoo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gajliephy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/goxxhgasf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gnhfqaprm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gdgxzmbpe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gqmiqgqvx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gjitkbqze.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gmafepkqt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gagzcabka.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gxlqeuinn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgpksjq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gsjqyxqsc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gnbnddbbc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwimxbrtj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gfbwydszx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzfwxdzmd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gijppbktv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gqjmsfags.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gylfhyvmj.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmgjzjyxx.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfdnxlsne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gpqqntjxz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/giaethrus.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/geahqolag.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpkohxsbv.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gyslchclz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrmkrszz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmjqfizte.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/ghdjjwvdb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gengevitv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/geqwhydcp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gjqdfabfb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gfhdawvzj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gawcuwpwb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gnwfckxaa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gaznftuqe.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghuomhfid.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gitwszxmz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/guahndvdt.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggcyntcfz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gowxuzlui.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gtbzadwsn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gzrgnfujy.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gkgpwkyif.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gcpavazdp.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gpfdbqboh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/ghwjqeefu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsxiyjymd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/goowalvuh.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/giiqaloka.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmdjmoona.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/grsddcani.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gohtykcbr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gozhixupe.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gtjbqjkpt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gmkxuoksp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gnkedplyi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gpiemnnqs.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gfwyfwtsr.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gxhqcdxlt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gsbzdweld.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gaujijiic.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glgjeqsqz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gnysivvxa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gcfconsja.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gtpumwwzb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gnxlopdzx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/glnhckeay.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkxyyhmtk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gpzjdesqo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/ghxrgrasl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/geigmdkeo.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gqmmrdual.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gjruvqlxk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtxruobpz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gehdxktbb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvkxnoqts.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmdyywlkv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gxribjyfi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gseapaxst.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghsotiufb.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gdzkimlcg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/goegejjvq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gppnorpms.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwairulem.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gixbgbdtn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gxohcrczk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gaijbgbzc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gwjgvhdfe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/giowafvcs.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gyqfhphlr.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/giuxgcqkg.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gkaewghrc.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzqvjwolk.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gvygoyluz.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/ggrgseumi.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gsztszpdl.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gcmjyiwsa.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gwzkfanwh.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gwehfhbke.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gphmmhogw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/glutashyg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnezqhvjf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gyuzjgyma.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/greedgupq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gojohsllh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvhmcjjan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gmergcjzs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gjbxhzgye.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gzextxilb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gciurcjht.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gilnpxxer.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtvjwywds.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/givzlkggx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gslugkbmn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/geesjhumv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gnfpntucb.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gwluhrrhb.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gcfgsgfwd.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gmtoyazwt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grqjyxzub.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqeddlwhk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gjixgqikh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/glexmnqzs.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gvhaqficq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/grqlcpqdr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/goskmsitj.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/glrgfozim.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/guzxtblsj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gdabiymeu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gxfhaiolp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gbelvjefz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gcvrlbvfr.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gvekjtbsx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gtgzgwsva.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gyshojgpu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gnzgahedo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gtfcjhflr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gacwtaqdo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkzzlfksj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gyvrjrrjw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gdbsijkyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gjocnmrqk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gmekwegod.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gqcieumvu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gomznocar.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gqjxklxji.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/giqydoder.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gwwggczbh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gbzzzeesq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/ghwlteomd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gnxwquojq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gideffiae.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gcoaeuydk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/grbywwfwi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gtyyflrdk.sHtML


<!-- 参考信息 -->