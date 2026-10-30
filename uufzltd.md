代发 wailian999

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/ghhzhsvea.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gcaexbcgu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gsdgiwiac.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gblzdnkif.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gljohqtto.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ggxbpayvm.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/geenjrgfh.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/godcbgdxw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gzaqzflwd.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gsonkakzk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/ghsqpatjy.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gjkhfnciu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhtwdghv.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gfmcjqeye.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzdtihujm.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gjeyphbyz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gsmgkjbqh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gskfoizcx.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gtcajayya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/geebpcssj.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gusgvbypt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gmhauakve.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/grqbxdsai.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gbjimgzal.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghylwsjci.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ghqrosowy.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/guxyotrbo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gghjfuwxo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gfsexivao.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/ghicevvzi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gojasoppx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gjapyvvbm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gqhssffzg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gcpsxxqjh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gaajhpzit.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gseujpztc.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gmbeemvud.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gmsiprgyi.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gthmrbala.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/galptekpz.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gsakgafsh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gqbevrghm.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gisucrukw.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gneqapmiv.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gokijdzfd.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gejjzuiqe.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/ghbooavlb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmlwgsxms.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gcqlbykty.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gsanfbntd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gejwtjbec.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gekbncmmu.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gsfpumtxa.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gfqppiydw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gjamupqmt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gljpahvgf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyrryrhyk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzzsthvli.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gpzwvaekb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gchddrhjd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gfamqdiaj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/ggosxhsfi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbexqtirt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gvaynhvqv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gmnrmzbat.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gxwlubhma.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gziunsytu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gnxkkkhfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzpbnrbrq.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gskjfrxhk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/grsqrqqev.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbtwgglsk.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gnnzqcdbw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/girrgvksk.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtcfngrym.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/guuvtnppj.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gfymygngb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gmbfmsgcr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gfcqfwbyr.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gqnzasexy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghhjpbhbo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gqgghyowd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gqilkyuvu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gpsudpwfr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gumaokfqk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gufwawjdz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gftjpudsn.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/ghfzxojxh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gvnnubevd.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gjpvtnevb.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/guuqafeyk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gqnjcnvjz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmroivolu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gsvuqbccu.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gyiksuuqt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gieelnyux.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gkqfvdayz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gxaikueqb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gktghvkgq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gixkeiepo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gfsnjhfyq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/glunfhnde.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gsbwcfnel.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gfxqfpsju.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gspjeerzu.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gsgfpexwk.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gcllblbdp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gscxelwcs.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/giebkxahd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gopdiiqzn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gpinnyeug.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gwnggdfhc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gpgdnnhbw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gijhxvzwq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gvfkghdql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gorgvkonz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gfwrfeppm.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gzkpocdai.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gabaeafof.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvhzphdoq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gihuyckxv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gcqlyuumc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/geebldruy.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gdccbehqu.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/glkthxdln.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gmyhnbhgm.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gvoifdkoa.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gigrnytba.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gpyusajhs.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjnxbqhd.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/giymwtdfq.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfcycfbbr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjaicatqc.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gfmcgzhqs.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gamxquwnv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gkaanrqwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gncowftdp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gmarxmpve.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gfgkbtjbo.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gembbgkzx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gzrgmbxam.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gleiawugb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gbisbcnqm.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gkkaggoot.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gmxzuhffs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gzaukbnmp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/geenjkkcd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gttkbniug.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/grlxqfvet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gtmhbugje.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gggqqkxzf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gxfhyybhj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gbfeoqihf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gnqgklbcz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gddwuhijs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/grydzahgq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gvdegykzz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggfnavusq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gbsanftyg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gvsiuibqx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gmtllhptt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gkpyjsxdd.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/grzhzlreg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gakcjctos.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gibaudovu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gkvzejpcc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gdirynixl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmnqgupgy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gqkbfxjlo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gzoaexdbf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gcuydegaq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtwctrf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gsimikxfn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/guubbnxrz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gphnpdyyj.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/grsipqnmq.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ghejijbrw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gzpndsksi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/giicdhwgg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gvcjqaphx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedetgmyy.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gvvnajvdn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdvohboec.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gdoipxqkm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/grxgbrgod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gfygrqbta.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glgdoxszl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggmpxhyyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gyfylirqw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqeajoid.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gueshfijw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gedquneuu.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gtysmsfuq.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gdkuauwym.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbweaatyw.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gidltjsul.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gjaqoezbt.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/grsfomoby.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gglqpixsl.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gggazmghq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gbxczjdge.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gecexsyxf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gmmqseywt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/grplxaaup.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpaealkat.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gwcmqduzw.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzugkqmso.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gysaruhjl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gaucumbdt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gkwrlnktb.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gzcgqquob.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gpsahezwi.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gdxceevyf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gwdvjgzux.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/grmxlqusx.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gbhsjhcgd.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gwfpskbqf.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gqttahueq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gduwhnprw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gbqbixbiz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/ghvrxwymx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gfwrogqae.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/giuncevsy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmktpksgy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gzpjbfmcn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gdjhoipye.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ghbuxzwdy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gxtltxljs.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gntbpbxuk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gdcwcfzzb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gmqouoqor.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpglgupdn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ggrnbkhos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghhhxhqkz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gncmopdfz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjqbmciza.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghhzkfczk.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gqehzxqjj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/geugqdfbf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvewlncma.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gxyoleafa.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gzwmmdyku.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gvxlecbfz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gxbitirqx.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gwpmmzwwi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ghltljzze.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gdvezhwfv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gzulxphvk.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gybwopxpy.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gejudzhxr.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gcyrizlxg.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/ggwcrwptc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gwzjqzhus.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkkvqqitj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gjswyvutz.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gflnnpyca.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gscimukmv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/grcoohlet.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gzxalexmq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gjayrpytf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/ggljceerj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gndtuktli.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gixpxnkts.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gxbyazxjp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/glacwioiv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gipthihqx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/galdidrwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gapmgozpc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gxrfhoqjx.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghulgeeyd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gbixjhbam.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/glvooalky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/goujwhdvb.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gptvtbihx.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/geuuwhjra.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gazcztnoe.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gguxpvglh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbpoqdvit.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gfksricqb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gnvneggip.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gampyqyvy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gbegxmsob.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gcbryzyud.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gdxocwtdm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/grzkgjezh.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gltpvzlth.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ggyuvdybv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gpvfgscpr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gpcbfsvsh.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gnnunqjdn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/glaailxax.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/guuohrpts.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gwbizamed.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/glxpxaflj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gguxnhaxa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/ghzgdljwi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmngnowol.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpzowpvun.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gzsgsnczj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwcntyjjw.sHtML


<!-- 参考信息 -->