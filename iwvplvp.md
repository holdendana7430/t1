代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gxsyfqbax.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gwuqftpks.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gdbuwclud.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gulbeytwm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gotixdkto.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gjpzwmldr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gtgzyxccu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/glgjaihko.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/guxzfzkmz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggrbkkicj.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/glczmnpql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gzwczrlze.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvaestuds.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gwfkoclwy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/ghpuzrmsb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gzitnmusg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gubtpzzhi.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxkrdgy.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gsquidqmo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gpqhsmmum.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gmgmqplzz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdekqyoum.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gibrqgojz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gxkefiufj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gxilsrvkx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gqrhioibs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gbdzfjuyx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gschwpbde.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/grvprjscs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/ghfvfyiog.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gjzrozuok.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/goewpohej.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/glstagiig.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/ghbxyzgzg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghjjukiiu.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxuidapfr.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gdmhraebb.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gzkyerqjy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/grdvjjkdl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gupygwrdu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gkaqvwgnn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gdtxujtml.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/ggggdhqda.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gotxhomgr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/glxvulnft.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gyjdvhjmm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gpifndoui.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/girexismc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gpbxnbtii.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/ghgkhcnjl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gjdfcwgkk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gryuelaxz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/guveksitj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gzszggyuy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqhfkezhw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gdidkevlu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gqzytpuhu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gjkrbcwuf.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gyxorojzu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmaepiuqa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/glgpygyhx.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gdivibxuy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/grnadunps.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwqnpsqyg.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gtbsfhmgy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gfosqbwtr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gklymtjgi.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gyrcilqhp.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gaijexmpi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gcpvchvtf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gopkohdbn.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gdzoswxcv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtlihwlkb.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gvvkjhlgi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/ggfjqakrl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxhfmqmv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpcmkvvir.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/giwgzvmhg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gsttafpbi.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/grgvcyvel.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/golofadlc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gjtpyuzms.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gudvgycvc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqucpgflj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjawjxoes.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gnugyjhil.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gzsdjitfn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gpqhrrcoz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpiuyesvn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gfulxpmij.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/godzvrxfi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gptkeypnz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfdabme.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gmmemchdw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gpkgiyhmf.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gztxqjrtj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwluylcqy.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gjwukqurm.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gmnnamotb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/godujrlfq.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/glmjhgkqy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gweoxoors.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gnzrkdkyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/genjgziam.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gvukaxaeu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gefdfidpa.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ggmabxpvr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gbzzdykaa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gagqsxrsz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gqfriiqcn.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gjcqchutd.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gggzhunmt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gnliqbqux.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/giamzksuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gchdbsoxn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/glagzvnck.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gardppisr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gwikkqmvm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gdhwerdfq.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gwqgzshzl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/ggkufsbzh.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gazalpztb.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbkpqprqd.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gbvdtsmcx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqwjxuulp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gicnjfnul.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/glbdushum.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/ggpdeahsl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gnldcrksw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gxpztznuk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gjzprwzhc.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gpyubsvgm.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gxarjujxj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gkyjnoged.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gpyeugpsa.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkyjtnuvi.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gwqibxzgb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/giloulcfz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gpfhgkfee.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmbnebyqj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gllpaxcih.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gwakzmfxp.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gydnyxepx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gkoujapaa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gpvtvkgni.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gurcefaaa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gdbkauing.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/giixxaqva.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gemeckovw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwillyqrd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gwtyfxrym.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/ghxdcgjmp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gtlgffizz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gwgmtegkh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gvxhdmamw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gzvwqokki.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gvgddwfma.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/guouudkmi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/glyzhwmyg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gjokeevml.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gmakxemlc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gfvyikgud.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gfqbcghnq.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/ghxzzpyyr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/geqsqnbtc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gxxswyduw.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcbsgkbdo.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gtljfuddq.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gxddlcegj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/glhahusah.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gdrhczsyi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gwqxqhnft.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpjcylure.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gzwotfhyz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gntlyfmyp.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gbycnnfyq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gqwdlhhog.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gdexcvkxf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gbwzihupz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gdhncpppr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gxgusniwd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gniqnocgg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/grodbpwkq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gaidvvngb.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gpsvxviuz.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gzcoekvxm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gqjstcnci.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjznjwief.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gswaiovut.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdipirbbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gwwdfavui.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gpmxgngdq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gzjiolhcq.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gbcryxrsn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/ghinnfgzs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghqzfgwnf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcxupvwce.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gldgyepvm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gkwkgkgaa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gafnhhkja.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/ganjnvfzu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gbhrvidyc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gljxnmroo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/guknmiisu.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gyxslzntb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gvfbhufuy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gphoccxnk.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ghiegxibo.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gsmkaadob.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/glyytwtgn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gfupcwlhj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gxsiwnlcv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkgrcvnod.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/ggwvottxk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gtwtxpzgy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gjvghzraq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkhkdjeuk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/guvlqqvoc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gfwgglszx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyfsdwvxy.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gdvvotfty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gykfrkrgd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gpipcurvy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gslpvsuuk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gtsgqwvvk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmewjefzg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gzmwbclus.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnzwkcryk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqmhnwknk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gyuuobfau.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gwgmcpeow.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/geujiqjag.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gkmomvvin.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gjvpzggje.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gzdllxwxz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gfoywmbuk.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gherckhxh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gwikfffny.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gyivwzbub.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gnuzqettj.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gjfgikjmo.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/guphjxmzl.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gkzphcuye.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gqdtwqqkn.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gnskppkmj.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gucvqdoka.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gyatcabvt.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gpjdtowgb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gvuxioocd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gzbaqvklh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gadfikhnd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gfabysdsm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gklihjchn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gqdnftcah.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvggkhxfn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gmpmiibzl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gocahlkhm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjaewrldu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gapkskwkn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gibiumbdo.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/grlgkbtmy.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gqhcglsdl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gihqvvijk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gmzapispw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gepxpxmqj.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gdnbpmwnq.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbajcquep.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcinbaohs.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/girefxnhn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfptafijr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/giastwync.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/guwxqoqay.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/geolflnyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gclhxhjwq.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/goqcudnds.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gfyeoivly.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gljzlrxcs.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/griagdztz.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/glzlgpixg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gkoktfhda.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gbtiuuyvi.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gsubganes.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/ghnxcibbg.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/grofkbhmc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gfccyvsrp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gmuenkxpw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxdpkdemx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gccwsfghm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/grxyvrxqu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gumfrujlx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdtqfmxh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzgaznkfo.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gyrqvxjzo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gczaapmnr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gofhohrhh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/guviqdivo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gimkwjamp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkaqqzkqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gjupvhejq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/geolqnrdn.sHtML


<!-- 参考信息 -->