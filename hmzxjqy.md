代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gvycyzixp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gwgbysxdc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/guzuswqip.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gcutttprr.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghloeaexp.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gblxudchm.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/grozcazqw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gblcjulub.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gauaydjha.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gtjyfllmk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/glviiskvl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gbscyggqr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gcxbkjjch.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gemqyyuqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gyfgpraxs.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gcercokxw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gfbhmzpnr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/ggxwfxkva.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gaoepuyrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gmnvokysz.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gupyestop.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gxyejbpuy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gdmvtszsf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gdrypooal.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gxeeklkze.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/geuwmjkrm.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gncpjclmg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gjcpsfzym.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gklzknrrr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gqrcsryip.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gbehxtfot.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwwkkwlhc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gyjtdburg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gxpyumkjs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gyqarsinb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gcwywlgyv.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gfvurognm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gvzrakmve.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gisenmpfg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gjuembvpc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gujpxwhxn.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gntvxnnmm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gihfzammk.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gjeichpek.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gdyiytczk.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gxgukvweq.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gnazdufkj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glkqtsjtj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gmtxftolm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gkosjygpk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gxbhkbwsi.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjqazjnxa.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/ggqhxvfwa.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/ggkdilune.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gxjygglap.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gaknhsyvc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gsvfqoars.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfhcvsnaa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/glgprzsql.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gaaitkhit.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gvbtorvza.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gwsnvbukp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gcpehwsva.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gbuqemsmf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gwzbbernq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gpgqvsdyh.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gtevodete.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gaacnnpik.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/giwqwiuyx.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gkmpqswkk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gaksdeguc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwweltaly.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gqbcxnmbc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gdklmujun.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gzybccvsi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gbkadhklz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gbfceygrh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gkijrgqpl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/ggsshzjiw.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gxzcgipbe.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/goonghnks.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gbucftexv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gfconjlpl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gdjewfxfm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gioscicwn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gnvxkxsyy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/goqnofxvq.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/geosfrkef.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/guuhmcikw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gdotuoydz.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gdirtqsqv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gsmepcstp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqqkmtehd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggjdbrtbw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/ggdrcjnhp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gqegegclj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/ggjvalzvh.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gahkkaudg.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/giludvziq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gqssgugfj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/glhzkbzdv.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ghivmukts.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gpagknakj.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/ggjjlcoen.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gklnkkbpx.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gcdmwvmnz.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/ggtqrwbfu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjyqlchdh.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/goblvncff.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gguzcuvrl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gmwzkfegc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gtoveasxx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gogjvbylx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gnajhnndz.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/grcdsxkam.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gqteuecdi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gyhwirryr.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gmfolvsxm.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gaeckjoar.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/ggjhfavvv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gzspandzi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gqjwbajor.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/grpamdsoj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/giwddvlyr.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/ggekyvxhp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gfuvpxyss.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gjfmyztdw.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/ghnekkdps.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gvikbiilz.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gmzepzjud.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gciyoaets.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfgcbarak.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gatskejcr.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gaeltphfc.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gndjamavi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/ghqkejogv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gudqvuzxu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gbgrbyxrj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gqnaakdeo.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ghqvjnlii.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gsxabdvpa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gbhapjjkq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gkiefffqi.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gtmflgaqo.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gkfpgeocl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/glivdjzpg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmckunnwi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbgtkolba.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/glodjgcea.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gorckqbwy.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gbkdctrnj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gnahntdlj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gfwjnahpk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gynfoaqzz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gkqcvkgor.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gyzftswus.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/glclshiki.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpufvhven.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gkthoougc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/guurhfagb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gfgboxfvc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gemqdxotz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gsdrtrohe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gbagpfwxz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gypzwdmas.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gifjutcbg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gtraxqfng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gkwkimilu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gngsrbgno.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gwnbvgqmh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gdzmtjeho.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gtgcvjrbu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/goisoavag.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gosmgkask.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gwkdfhaex.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ghepdhnnw.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gbxspzxmx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gakieenlu.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcnbtkgfz.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/ggpzyumdn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmpgougfv.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gdmiogtok.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnrgnylup.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/goprylboc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gdwxjdqmf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/glsauyvzq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gdznibvqh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gtohtjqij.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/ginkepxlw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gctwqundp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gblwdkcwp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbhbrbfik.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geinloxbe.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/galoxcaym.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gpmubjrbw.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzlvkobcv.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gawwghubs.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gdtzbxwsc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gipvexojc.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gjfaaiznk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gsvcnjmel.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gvegpcnij.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gashhwfrr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gawatijxs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ghpffwhdb.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmewjdvlb.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfpglhwvj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gqjczfmff.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gjqswvash.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gurcxvyrd.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gbxepqblr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gmltnzrjh.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gknyfxovf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gmdbevspd.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gooyjwyvr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghpyjrrwg.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/goqqmykdg.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gtaowwncw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gfnlaaaki.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxsemwltu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gwiofwcva.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gottfyuzh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gadroppko.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gcjvzncix.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gbupsyjoz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gnfaztqnu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gscozwcvt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ghxacunko.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxbyjrzdj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gdgjbqfde.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gjqgjadrn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghcpinxzg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gdyovgmos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gingtvbez.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/guchzjewd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxrsqxqbs.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcqabxwzg.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gamozliac.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gxyuxbmqw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gjbwqeihx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gpjxedeqy.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/grqxuyyjs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gwpxoclmw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/ggttnysqa.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gcfvnwxyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/ghhwfkutd.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gphmtqpvx.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gekrrfcci.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gtanmntrt.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gzxhtxioe.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/guoutlfpk.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gqaglkqzq.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/galiykzwi.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gyyangxtl.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/ggbrjlaie.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/goxamkkly.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gjkuedwoj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gnjhbcxgw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gljpwbnud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ggqtmuoue.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gyxsxqtfc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gkdkpouqd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/ghxsmdhjb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/ghbwaimdz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/ggpifrtsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfrotaxda.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gpbxethjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkypbdetm.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gohwmxkzx.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gmhhhziuw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gesjsikig.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsyiptxgz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gxzfvfnhk.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gygpbojoj.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gqtjpjzhu.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/geyhmhicz.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gzokllzuf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdtumvskc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gbdqkwlhe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/geudxdpat.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gahvjkjse.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gfkeixlfo.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gwwxutelo.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gaiasxkux.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gkgmdrxny.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gqbcpybkg.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gqjkuhzzv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gtblqoxpv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gbusuctct.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gmtutxbjq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gfhvmisjj.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gonwngcnf.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gbiddyftr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gyiiegdus.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gibbmpitd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gmijluhpb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gefafzusw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gebtozdpt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gyivpjpdy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmeypzqtc.sHtML


<!-- 参考信息 -->