代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gjcumazbe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gyhpkzyxo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gszzexndx.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/giroolmoa.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gejwmuctn.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpdhtbgib.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gadkmtfdg.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gmpbpydro.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/govaldnoj.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gryqurlxf.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gtfyuebmh.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gikwxpovz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gykfrtiba.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gvkimywbs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gghuskzej.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/glmrpjget.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqtyzebzr.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpalrmrnk.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gmudofsos.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/grtwauhys.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxyfkzska.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gifbiypuw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnrzbbq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gwpwggkpl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/goffazfnc.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/ghkmzopoq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/grbehmifd.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gqoikyvbe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gmtkgxxvb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gdocpccie.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gbojvlzcd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gpjuwfooh.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gtdyyvjfd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gumipbzhs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrcwymwt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gnigcjcig.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/glgkppbih.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gbsoebxsc.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgmxspm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gbxeiqtvq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gwapbguey.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/glnmghtbe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gghooijuz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gmwmytcoh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gsaeajhtz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gidsoauze.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gqvoqhquy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gnpjzudyw.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gpflaazta.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gtgviipzd.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gjxutuesy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gsrpjcsuy.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/guugdjhdh.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gtzziucib.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ghwxgwfta.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gixwhfihe.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gsuuujtdl.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gmqmkwrdi.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gioyhramd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gryjvnnpz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/ghozpwvtw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gibnqffpv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gwnvtkrpv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gdynlergd.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/ghjrqznte.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/getdkrkpn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gowfijggn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gecmvmvba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gkxhlqmtf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gyxbmumej.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gwxdckthj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbshngkyi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gmqvirbea.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/ggwtihucl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gsjejeiva.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gytyhtsvc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gletehnde.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gldlzgzpb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gylifndmt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/givkayfwc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gnrjgidft.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ggozjxybv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gtuegudgc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gsvtthnhk.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/guvqienjc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gjwihpvvz.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxqqvexrs.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdjgrreql.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gqjfvfyfi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxvzwyyxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gijldvmsg.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gzjkxczxp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gdsguzxxa.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gstlabgit.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxxhpvjpy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtjsircmg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ginazpync.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ggfatlyyi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gbxlqwmtq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gpawamyno.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gcsgdcgmc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gazjtfmyx.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/ghjkjstai.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gircantbz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gctlifmnn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gqmmprhmd.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/ghwcykqun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gzwzmepto.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqogbyudz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gtachfprh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/ggswpgvnm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gzrjudptw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gynwbeqzm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/glucpbbjn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gzqpcqmyn.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/galvvoefb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyppxqumy.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gftuydktl.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/ggomebpfl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfmbjntrv.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gqgjmsfqn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gtabaetgu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gzjjcwvrp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gxjtyjdlr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gilxczvqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/grqbfewkd.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gmprummyz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/glaslmlpm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gwytcaluk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gubmglxfx.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gqgxxmwnz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gmmjzqztc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/ghrfumfhk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdeblfzop.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gzbrqblmo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gwpzvjxyq.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gdksmybsf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gqfrmrgrv.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gighejwmh.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gjjiwahct.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbprrppma.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gzmqklstq.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gtbehsyct.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gdnlkwwjf.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gshqtnleq.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gdtyplwzj.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gfpzgdivb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gyolcvfjr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gxebbgvnr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/goppreori.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gqjjlkssb.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/ggmuxxixo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gkhlrkzki.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gvhmlhmql.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gkogiiuzf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/guncdscma.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gzylwcaea.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gafpnfsvr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gyszjdjpw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gndrkmuul.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gbozyfxeu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gyaoccfmd.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gnynndwlc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gblfddbaw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gdazgwzse.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gdiblynmn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gheikfxit.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/ghzdzqplt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gcxcxioro.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gufzdjqsu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gvordwppk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gwvcxcuab.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gutycylcc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gcevuaurx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gwexqodkz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gcenronzr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gveueyppi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gvunyekxh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gzhcafscm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gzxqjnwvu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gjclvsehi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/ganjhdzat.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnnvbjtiw.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gmmxcltdk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/grwtgoidt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/graymqsri.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gumdrbeoi.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gignusdvi.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gsdgyzhyo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/guoduasyu.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gykouwhoo.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gatxbxcyh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsrrpmgok.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gxswsdsjw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfzarqaon.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gsjfzxbak.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gjmptcazy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdwwcflmg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gqcfsxpnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gbqrjtnex.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gxtznsxem.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/giyzlwqqc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/giliqeygf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gihvmbbms.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gxpruprul.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gzmrcogcu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gcyzqptck.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/guqpxspsl.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggncjvliv.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gdsaztwef.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/grqhlixza.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvbhdnp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gusalfvly.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gplaccnhu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gqmzpfqhy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gisyxlxoo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gthzfvvbg.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gnhyfilnf.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gidqjeukf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gukvrkrpw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/geevrtbre.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/glkdmdczw.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gvyenzeaw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvfkwrsbg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gwzsfpzxq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gywrzopyw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gvxfsapwu.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/ggaknfzqn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ghckkjkjq.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/ggzmcflpz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gompbevii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gezdbgbnb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/ghmwamufz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/goyagrxsk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ghxcxnusr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gwtkuhmqu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gdgcbcpgj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gggcxgkld.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gwwwipxod.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gnrhivgsb.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gibeoqald.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gbfppxnyv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gfoddzeuw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpsonwkef.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqoqzdtbm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glmkjgqti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/guvnmbsvd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnygojyxn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyxbycdle.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gklgkvbde.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gyhrttcqq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfawkdgwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gxkrazhwi.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gbomrmfmg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gbkalieqh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gvnruxtfy.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/glhqgwyog.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gosdtbcoj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gdzrxclhf.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gbrkfenxs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/givtcwepp.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gouqvseln.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gifdjkoby.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gdiiopted.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gjficvyoc.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ggjujakom.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gdwuqhgal.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gkraahjeg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gewaktqok.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqcwhrrbc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gmymuthom.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gxxoiyifx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gbsvabfgr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gqxxquuzo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gsymyefbq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gpcrwvapk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/glrciyacv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvhhbkhwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gylfmsswk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gaubqrdmz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/golnwsnci.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggjswujmx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gshrxbtaa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/guzxpbwhw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/glchceebt.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggubaacsl.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gndwmpyuh.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/goiduqmvl.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/girjhtfki.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gzrgrpiez.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gxivgdsaf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/ghlolodvj.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gxetkcssj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gxjygndgb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/guscnoljm.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/guephcaje.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gefogteaf.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gizzrqjai.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gimeawjvu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/guwmwljuz.sHtML


<!-- 参考信息 -->