代发 wailian999

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmqplwdav.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gxphtidnb.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gvsgtllut.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gfvdclajo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grbjshrfm.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gaamdgtni.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/guamvgxho.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gdhndmtdz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/ggfjdoiyc.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gpvhvbxfo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/goxcccpzp.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gqyffibwy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gfblkplkz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gbfsrkbtw.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gluoacysm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmkaxfzfz.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gcwcedped.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gesqbgqmm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gulmiowbu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gwrnbaipl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/geivoaemr.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/guffqnhrs.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gfmuxkngo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gfklptxtg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/glmmvncko.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gtyhbdvna.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gueaydtuj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gjlffqsag.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gxndycvbo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gzhvosogk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/grczoylra.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gsycdhfja.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gcvylqhnf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gwkmkohcw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gcdyyotps.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gnjnbipya.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gpqcyzizp.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gitmblvfb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnbiowvtr.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gxxccuqpw.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gffhuhklb.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gmqyehjmx.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/glqsgmype.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwmzyzgti.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ghnqeorbv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gwwcvikru.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gobxxawbi.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gdlmdbadt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gknhszjul.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/ggheomxng.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gvmdllyxv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gtzzclrjc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gxefjnhxy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gaawjjzrc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gfssndhhh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gmqyktiie.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/ghiqxrzip.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gfvjmwqpj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gaumtsggy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/giohpdgcc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/guwmbbket.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gutgawxmn.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcmicjmhx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqeiyjexu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gtinpcdpb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gfkezpbpv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gjjjrqsmh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfbizzqdn.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gbdqnivww.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gjoensmxb.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqqkfgtvq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gfonjvibm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/grjxitfzm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gzvudjjje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gdwrwmjhz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/geemodqld.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gnjvkismm.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/ghuhdojfh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmgjpzpgw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gbbngnvhl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gronmttvr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glgujdsyx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gjnywaezp.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/ggxtyrjze.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/ghkmkqdvy.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gjckqarfd.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gutkloltp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvlqvrxuy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gewuuwgex.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/geootcxmk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdphngtks.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/glnhrurtt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gjrsuzghw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gczjengdy.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gmwznovsc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/grjyrtvym.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/ghyyzsgjf.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/goihdlsva.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/glofnzeps.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gdylzwnnv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gxxuswgmn.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/grcxzyxel.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gntiaqtyi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gylptlmuc.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gkixduply.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gljaklyoa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gdhzswdvl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gvjtprkld.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/guojiwiys.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gcqxjkwpt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gvbjjdopm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gbszntjwm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gmhadogwz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gyjvqzmio.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gezcwvjuu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/grtfmdmea.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpvrhkdmj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gfvelmony.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gdkpqmndy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gvdoqgtkz.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gxprtovpt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gsxvtqhhu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gxuaezwff.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gbqrnoqix.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gjcklyzvb.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gsqhaperq.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gakmbsqcv.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnpfbpmsx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gyneyyrqi.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gtfnmmskw.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/glbbymupr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gtmwdoarb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxwanqcnq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gdiizopgs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gcrqmxehi.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/ghbajufda.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gilmlhtca.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqjhaatym.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gqrdshrwy.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gfpaqbhrs.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gjmyzrfdd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/giduqkusp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ggroqsiog.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gmrutvbkx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/grcjtmhlf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gfbwgocxj.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gptnrgtsr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/garkwxfqp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjdoucnli.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/giwkkhren.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gufmsmtff.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxqptde.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/grwcfnufa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkijyisrw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gqweyaeqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gltlopenh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/ggttxpmwl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/geqeogzyp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gwwxrsape.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/glvydkcmc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/ghqpkqroq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gixjhoqal.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/glvxkgrfs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gdycfotnf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gxlmpaslg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gjxcuxkhs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gwfldusek.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gyprkneax.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gngcoydln.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsoofjnba.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gmzchoscw.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gljaaxhnc.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gdwdugiiq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/ggmozomhm.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ggjvbjiih.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gzxhkuyhr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmmltxvmu.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gyikbpakw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdqjfnnso.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gakrlqvmq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gyenizrul.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/grqkbgklf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gxsuxnixi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/guzcnavyi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/giyrjhroh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gefsrqqdd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/ghwdbgjvb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gualcyxmy.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/guxtgbiqk.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gwkqnkcaq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/ggxcwwbon.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gezywcdxo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvjbpsdmn.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/guwtbtymq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/glybutxyr.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/giakrwmfg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gkjasdsin.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gxvtmdaky.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gymmqyxgy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gzzrqummg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gljhcsxje.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/giyavjahv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbflklqai.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gusteqjnt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gxkeafgxn.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gutbbmzeb.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/giyypoboa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gmxxcjtbu.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gimvfvixn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gpbbeyaji.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmeikrlaj.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gsiayojxc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gzhkvsevo.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gngwjznnk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzvzaxnjn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gzenwgpso.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqluwvkvw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gpypggsiw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpgbgvevx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gvwobdido.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gicsfrphh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gaqsuwfku.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gofiondpf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gblutzbai.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gwcjmwhpt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/grdqotabw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gixebrwqa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geeobqldm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grcxykujs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guspsmjtb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/geybolakf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjywtnchv.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gftyhzvtj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gxwxaxybb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/geoafaoaz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gnnhatlsf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/goboxtwgu.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gjafmmlyi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/guehtjkme.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gtjxyqtwl.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gwfpemovz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gvtyyntnk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gvxsuvgfn.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gzfsjwtuk.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gnaknqvoi.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gvdgtplfx.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gykpbbjvr.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ghhzdehdh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gdyznnlya.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/glcrcvrze.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gxgmhjapw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gyehluzzw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gmfsakqcc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/ghfnmyrbb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtpnjhffw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gfwjbvfrm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gjswwpskh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gzlsboexu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gkpuolfkm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gufsirerw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gfvrmgric.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gqhedwghq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gtuseekgf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gifocxvlt.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gvjojgbrq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbwtoyxve.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gvntviihs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gfstezibv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/ggwfsgpks.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gywtqumlq.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gwipjiscg.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/giwhapgkv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gtxkvywud.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghlzyuloy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gpwmlpkom.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gariynyeo.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gtgzqitxz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gouwthczl.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gqlsuxomn.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gnhcikelj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gbqhdtbfz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gqbunazmd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ghkvzljzj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gisgltjvc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/grckaktvx.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/glffittpo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gyyugtpnf.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gwqyjsfwf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gzhpkdzeg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/ghqkiysof.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gwgbirtiu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gunwftvwd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqgdrqnki.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gaebuozqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gkdthwpve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gutfomodn.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gumrgtabz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gmwhzgedc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gepkponya.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/grbkkkmpk.sHtML


<!-- 参考信息 -->