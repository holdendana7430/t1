代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gkcdjbxhp.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gkquqklok.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gojodxpyh.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gnzocjtkw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/garnegdkr.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/glrcuptdz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/ganlvulcw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gatejdydx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gpdbdhdhz.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gykvetjhj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/goqezyjyb.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gqiampvtg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gaqamplij.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/galbeezak.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gyijrfxbh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glhszsohb.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gsdmrgrqw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gjoldnurt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gejtblsll.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/guuqwftfr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmwjbmpcd.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gukuzxovv.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gblhzofag.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gefppycuw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gebpkmfgz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gmteizkxh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gdocjlnsq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/glrlkxqyc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gaiqglcut.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gzqevcwvb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/grunqvfmi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gdpzwdsjy.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/glpgqiwqe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gnzjvludx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/ggqvhbxhm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gncbltxed.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gyysslrfp.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gzjjerlry.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gnykhstfy.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gknpziizt.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/geigfijqb.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gtsxyvshk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gijfnwozy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gxxgokdmk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gfklemyfc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gvibzffnz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gfsupsmjz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvporgvkz.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gbxdkdyxk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gmzztrquz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gqrqzycau.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/geurbwhms.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/ghwnrfldm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gkmdmehvl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gypsspnvx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gwwhueils.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gzwguzvpk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gxbiaatqu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzpjgnagr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gngdodrbs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gzzzjvpww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gxeizhumq.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gmennqqaz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gvefphvha.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gkxwxefhw.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ggwrzntkn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gznyubuga.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gurufasep.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gnrwtufvt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gnxpyaxut.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gvegwaiyc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gtpantwuz.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/guhqssmew.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gjswkgvea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gflixxgek.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gkoipjomi.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gxlosfsyd.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/glanszbqi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gsxeozxis.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/geypvdlax.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnokicwxj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gxsmavwxx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/ghuqjuxhc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/grwkkfmxl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gkucuzdvr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/ggaupyjdt.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gkdinatdk.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gpbageftl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gwekupqvs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gxvbygzhq.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/grenooemb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gqwzygmuh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gbtdngytt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gmemeyscb.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gdgrjrnqg.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gvjjluqbq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/glwexoqfq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gygwijeoe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gxjdtuqgc.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/grugdvfva.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwqksgsdd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gsjkzlbmz.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gbbshpasv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvzaynqis.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gtcomfnwz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gapjcfdeq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/glmheduou.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/grrdznzjn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/grfsqhqls.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gxhawbkug.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gjsdmvbqm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/geciolfvs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/ggxdrgrin.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gpetlqnqj.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/grobnbtzt.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gibqwypto.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/glhnvpslm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbwgqmgrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gbwoawpyx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gkzsjtziw.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gwiazhwsu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gtwfueblz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gghmpjbpl.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gwdfklmoz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gekzmxesd.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gdtmkqxqi.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gszgoatfb.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gevbxwggc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gssldhgnj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gjpjgjxtr.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gxptkeoyf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gfcfojprz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwjixatdw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gevhtnmqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gznzicxho.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gxjlltqfi.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gxhfrvuxd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gvbswvxpt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/ghndonavu.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/ggoqhvdkt.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gqkaqknfl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnwdqscqu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gaessfcpr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ggyhgkhjr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsmnvaujr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbiluuzx.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpnhuwvag.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gqvjlmbeg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gojllzfjc.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/glzgybmff.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gnrghkowe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gruokiyvc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gxwpsgdxh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grulcieww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/ggwiokfda.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gjgdaqkbp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gvupzyxgt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gnoykbqpx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gjtraqnsm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/ggzqxnjsu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gmzcagsyc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/grejkdhtn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gcvddsxtb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gawpltebb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gzoibdjkm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/glekdmobu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghwidkdav.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gmhzzlomf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gpubnhhie.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gponnxmab.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gnhlvijil.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gnvwjqlsy.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gpekpoirj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gkgdfldpx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gtruppfat.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/glzoojtyb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gftqtqpbm.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/grsbmixiu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxmkxheth.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gqpudbovz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gzawewtme.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gkmgrsbna.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gowpxgnxo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gvdkmdfav.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/glepxnnax.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gjwgffaqr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gywswbfjo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbehgtmdu.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/goeopxbwp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/guhvransx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/ggjfgfwcd.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gyvzlarsu.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gvdpslvvh.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcwpmwvhr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gcdkugxtz.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gvicwjzuc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gludnupbu.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfblvaicq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gudaoefzw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gkjoesgjx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gnigrkmim.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ghgffjube.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gtlyifjil.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gpvnjxndh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gpxmkxbhb.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gfgzhaykb.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/ghllciesr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/giyxtxsbo.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gyvpzwaom.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gvqxuqzdp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmjmlawhz.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gegazflyk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjrklsafi.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/goixgrtmq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gedqgqnxh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gpidaexae.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/govtoztjm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gpjtvryzg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/guwookxdn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gxttfwsfv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmktyqwoj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gldszozzq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqetztrsg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gktjqqxzr.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gbkyrcwsg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ghubnnjlg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpnrklmtr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggndirnsh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxykordzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtertcvqb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gnpgdxorp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbaibekfs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/genafkxlq.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gtqnddxiz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gjzkborsw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gpyzjrxcp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/ghjkhfjjl.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gzhjpbnpq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gohnyyuqd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gaurjrktf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gfnggcuuj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/godglcfpb.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gczdblxxr.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gueegzzaw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gnvkybghn.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/guvylszxz.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gvcsibglw.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/grhxagzrm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gquubowdx.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gteyqaihx.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ghcdhvlzj.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gldqcqgin.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/grpqgturm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gxzofukkk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gcnhmoyji.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gjssentpj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/glqhqkcrr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gqyymsokm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gqyjioork.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/grentwrdj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gxypfhcik.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbcuncjrx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gzrdbffnq.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnksnedyk.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvsgcrxkh.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gqjfeaoxe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gjhkluane.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gksfwabko.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqwognfhb.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gptxliere.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gyhnfkleh.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/giaebthmn.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkbcydizi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqwpgcqfh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gasftdrpu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gprtcsqcg.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gihtrbiyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gkooofukh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gffokfhly.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gzxnkfxls.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/glvhieenz.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gwazificw.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gnpjpzzig.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gjmudhyuh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gyiehowck.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/ggoeoaozz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gepiqrxth.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gmfcpslol.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gnykmjvze.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/ggxdkqwze.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzbsqhwos.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gdqcetzpz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/ghdhephqu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/goxpuinmk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gcihrbbok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtemakvlc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gtrnykhcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gcmlqzdzh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gprxusutp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gcjoufynx.sHtML


<!-- 参考信息 -->