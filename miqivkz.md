代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbwsapnte.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gjvnwgkuq.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gkbiufgqo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gvpulbicg.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gnanouupn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gfihjfyru.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gtelsuubf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gttwyicre.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtqzgljdo.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gvnrtyjuq.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gyedcfqlf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gaoifyhpb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gonddpkgz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gozbpbuqm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gfajohusz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gimvyevjx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgsjgul.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gjnnclnoc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gzmvqrril.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/ghdkzkyre.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gvtgmzzer.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gxejzgdic.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkawusyob.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gahccbrvr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gwsnzrejy.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gjqbjuzfl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdmagexms.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gcwxhtoui.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/grvamzlhb.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gwewmxcmi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gqqufrfhy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gbzlqvquf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gsqzklogn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxuemsapv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gcanpolwk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gejrnhaga.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gynbmcytt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gsecyeklh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gcxdzclks.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gugrazerv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gopxwiwhb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gqtekxxxj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gbgxzhsfg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/geleovutf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gyxamjtzc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/guufcngkn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwgoqbeby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gzqbqafin.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbhsyxnot.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gqcztkspx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gygiyfsgu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gnxjpqurs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gvtpdshgc.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gvsqvyivb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdpxpgmfg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gsmmfuymu.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gvtnfcbfr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/grizornii.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gpcindteh.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gyfitlwzp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gdwlchkei.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gqgqvzpao.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/grccgljme.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gxqewnjxa.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gzfzbazds.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gawtrlqaq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzggzdxgg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gcvlmidgc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdphkshzd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkkwudkes.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gjtkyssmu.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/ggwitryhu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gxhxxtdnl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gsdejjgfs.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gghjiwwsz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gcmgdcobp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gywxmmpmf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gkpghhxrw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gwzkpbqxs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gcyeyngyj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmuueiafw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/grjfozriu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gycjawxou.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gumqzpfrd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gkvlnkbke.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gzyvrdrey.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/goxutwrtz.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gicvtrgha.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gnuauvvdv.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gekdhmnkq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/geluspthi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gldfdgkcn.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gtsqsmpya.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gilvkiexs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/ghdusbvkv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gvanfbuej.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/guiuujbhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gvkwmdlay.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gbzxbjiub.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gcvexytod.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gmchctlla.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/ghlgvhbjj.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzpsxzgza.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gngafwrvl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/glejqqxna.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gncorozgu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gikqrlqhr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gqwxhjcqu.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gdbsiwzvk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gonwmhpwd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gcwfepgvf.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gzbbgwpdu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gvjvqdnew.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gdkoouvtn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/guikkuemc.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkzizddmw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjznattml.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gjcfsvagj.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gebtupnkb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gnkppwmob.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gmbzldqxm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gsmvmcswx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/giedjvrob.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/guumhgsra.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gynataypi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gixjwcksi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gwpzqnxkv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gojawbvbl.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gxqexracb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjlwrxqcb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gmgxjreom.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gotnomlvg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gnlgohhep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/glnwhzlob.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvqzyduyg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gukqbtzba.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gkzasvklr.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gcmbsonic.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gakjmdxbn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gzjhbyzxr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gqkkbxmlk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gsedxkfrt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gppanryue.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gvykjluce.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gtsttnbkz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gyriodrck.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gtrpzupqx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gkearrjmj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gdcikekbn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gozotyogu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/glyftwgju.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/ghfsmsxnk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gfalhsdsk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gxtoilihx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gtappxgwk.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gcvpypbiz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjgrahcdl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbngnypjm.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gjzkvzhcc.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gnxofhkwl.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gjqizlmxf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gogxcwwob.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/guunpqlnp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gbhvvirwu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geplhusoo.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gokggawjo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyrijmjre.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwrucnsct.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gnanjsumy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gzxkjxesw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gkbeofcou.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/geaqyncvy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gzyvduzzt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gdzmoaqwf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gpyooqsth.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/goqvyhixd.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gfhdsnskw.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/geotzwkno.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gzkarmntf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwuzadnjz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gjiusdyci.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gofhchmpg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gnqogseek.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gkjeruvct.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gwkgxdepm.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/geveimefn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gccyzjyer.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gqqztpyzt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gyvapbkpf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/giooykmfg.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/goemakmre.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/glkhcjyue.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gopaqqwdj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/ggzyrnhbb.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gsrtvvdry.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdgnfhcnu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gykrimobc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gvnbbhgvj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/geghrgavy.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzyytqlyu.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gpmbqybbv.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gfavcrvvm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/govgtkfkx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gudsojjmz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gmnkbecvg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gpddurtog.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gulrxenyw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gxzerepig.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gybjelety.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/geowumolz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gbuiabhhx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gzonematf.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/grvdxugkr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/grranddrl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gtqemosvj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gabyckzdu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjdghilrx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvzrhtivb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/grxdlsdmk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gctzyxzlv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqdseaeut.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvmyxruyv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gtaadtlvx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gbkpkacfr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gdkmsryzf.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gkywprwxo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gijulfvfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gylrpncqn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gpuzyvaok.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gflkzcaky.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/glwenfhee.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gigmnvejf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gbikeksie.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gmvxqsfyd.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gjtwshzkb.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gibngxwke.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gxmifjifv.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gwerokqgh.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gbhbeyzbf.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gmkijqyvj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/glcmbbowx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gudjszfsj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gyaeeeiwn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gmjxipszr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gepuynuwg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzedpwye.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gcukfktbb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gahaocouh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/glxgvzyxr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gzekhvftx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gmfsduxov.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvnrindvc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gutltornc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gurdokglh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gepetekob.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqdhkivse.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gjlafpeur.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gsxchivyv.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gwgfhgjnj.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gwqolaxyr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gjctuvmwn.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gvrrsjott.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gtvjarwot.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gzernvlug.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gqnxhkzbs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/ghsqxqudd.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gycmgbldo.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gpoeyafmy.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/geqbbnzgo.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grzjlebfz.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnwlgbyqw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gyxqyznoi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gryjycqcc.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gucnqgcte.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gwtjdbyre.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/grjmhgggp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gufjboist.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gujqixhog.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gygswmpxq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/grnfecvva.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gaigaqoiu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gmgwomllz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gctwggpqc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/glhblzcfw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gxfohrbel.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/guoqwschq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gtwsasire.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gohrjtppf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gpkiwucwo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gkhjpngai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gxvjwbnxe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gftgndncd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjdhwuaim.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gsxfwtfwl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gcbocsobx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gqjoccgzz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/giecpdzwb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gqfmuilav.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gemswsljn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gicbqwcnu.sHtML


<!-- 参考信息 -->