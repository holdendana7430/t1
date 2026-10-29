代发 wailian999

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gxjkpcjcc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gpgggjawo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gqpakotxh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gdaytcjmq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gwafizcvp.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gvzywqkbs.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/ghrccuqat.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/ghyiwrmll.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/grlmaiffq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gebxlzjxq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gccqckxcc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gmwxeoxrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gindqehsr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gzwlpmycj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/goiuyizra.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gtxaeguug.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/grnjaeicw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gfqwikndd.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gswwieldp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gfhawnttt.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gkzswhviz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gmgviqcnm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqpidqqtr.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gbjmfygyr.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gzzctnrti.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gkwuaroao.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gxknfcihg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gixgzzkny.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkrfkdntp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gwqoexnah.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gyuogbiqd.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghyjlthhu.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gwkxinsag.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/griuoticg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gdwxkrgfa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/ggcbtznls.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gabloogxx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gnstkqbiu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gewzaujqi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjtkuwuvv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/golptovub.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gmvnwsepv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqwfclabt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gxjxdopkt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gjdgcqjbj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gnfrzwpon.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/grzjlqfhd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gywfezryh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzkjqxszg.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtcmggejh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/goegezjlc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gicljczry.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gusquphcw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gdcmyodem.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gnvugxnzi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gshqieztj.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gfcnwwsuh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gucseanev.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gsrriiycd.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcncxvqwj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/grksryukw.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/ghhxdwguh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gumbmzwiw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfhkhupop.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkdzuzdol.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gmhywhrbm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gjckkrixc.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gdesotzgd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/givvyjcwu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gapufltee.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gofxsspru.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/guurussit.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gwhcglpzx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gzlabpiby.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsxusgzei.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/glrmdyjnf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gqeiymqit.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gviopoikx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/ggwmgapew.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpyunabbc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/grwrkqdoq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gitomwdaq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gwuxidxln.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/grztukpuo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gqgacayug.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/grlxectpc.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gybngkuth.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpfydqgmj.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gafliklmw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gybsovapd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gtbdfssjb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gmyymzqia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gchphfxas.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gzfgeplkk.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gsbmeocpq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gwsweijcq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gljphxdnr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gnvalqhdc.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gtkdqsamh.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjekaokxh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gzflumugi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gorojsmmp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gtfnnhzmi.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gzfpazlig.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/glwfdqxgm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/ghzfumiow.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gtomheffe.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gilkazzxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/grdccejgv.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmbkdsxas.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gcxorfqiu.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvwwqpdbt.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcfqktlom.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gkcngpubw.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/glcjyozwb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gwnoelvol.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/grrzmhkjq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gyhauylcm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gqdawnuls.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ghohdrqzd.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gukzubqqs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gwlgjofpo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gvajzxspl.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gjyjlnmnc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/giatjgnra.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gzdtgdfkr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnhmmzvxi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gveivdxzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gacpcxrgr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gymrgqthv.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gwkrisbak.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gddasfwvz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gdchyhkim.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gvezajyjb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gyrjswyzw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gwykodsnw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gndugebuy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gijfvryva.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gchdkhxdb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtwmzkdwb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gurqzaxzo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gqgooohhc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gjissildj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/ghkousjah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gmuoxiflj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gtyjlsqdk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gryucscwz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/grogzoffb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/grkidtxwu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gunynroid.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gcexilvvb.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gzddduyaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/grozutnqi.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gxpiyythp.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/ggvljqdvn.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmolxjdom.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gpqjwqtis.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gwjdzmifg.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfaofnnch.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gxrmozuzi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvyjdoqud.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gvbsgqonk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfcktwmct.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggtuxpeah.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/grvroegqv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkztrpvcv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gxtlxnzbo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gvolduuwe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gmypbpglt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gmbiscwmu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gkxmrchij.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/geekkmrhy.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/ggxrevikx.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gibgelujw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gbyqhnael.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gdwkmqdmq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gihykvefs.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gkzhfzhfh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gicyunfzs.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gbntnucua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gtaufycqr.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gihoxkuyz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gtyysncdg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbkiaeeng.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/givpegmep.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/goliopris.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gfzcijbwk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/guomcdiws.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gxbezpvpq.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/ggstzlfjm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/geukyjfpd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gctnbrqsd.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gbodqlcdw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gavpzyulr.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gggolfzrw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gxdaimjca.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gbhjlewbu.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gizenbzzo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghyszeetm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/giyumlblf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gvzodrtww.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gequohxoq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gumuhtgoi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/ghmsmphqv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtosxgmql.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gubgqajeh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gjybxumhd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gzgvqhqem.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gdrbfirpb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gqtzqkvpq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gtqdgheuq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwhjtnqes.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gywxyuqzz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gsgfovukm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gqymqhjyp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/guishbrte.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghdlylvxo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/ghvsnzmag.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/goynatcve.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzymhhqzj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gesmsmmaf.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gqlzxzmgx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gekixxtpo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyggihihs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gjmvsjdwf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gfiddgmcu.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/grcitltee.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gbpzqnatn.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gdogeooie.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gegldhgye.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gyiesovtc.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gmnylflkd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gzeoorcek.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gndgltqtl.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gfmbzhhgc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gveafufye.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gsbmnpzbb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gcwkogfry.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/geigecdws.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gsaoyhzgi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/glyfskuto.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgfhptjg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gdbayxhxv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ggfwpwkzz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gczxktisf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gutqydseu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/guuzstfsn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ggrxlwibf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwtukigkh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gqatkacdl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gyfhgspvc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gsxauyuku.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/grqjowjwu.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gepwhbbyi.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gbqvusxsq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/grhqwhykd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gwomthlrw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnyyxyjqb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/goimfermb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gfwenhbsz.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gjhbfqfwy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gleoqminb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gwscjugwj.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gzqfrcqro.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gwbeugbiu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gvoelvfwa.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gmhraiazi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/glgkkjwwc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/geeifpxzx.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gsggzpbbd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gfwithdhz.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/geagilprp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gepgztgsw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gpbpmcmxe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkgqjdbgz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gufvvazbb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkhxcnngo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gotvxchtu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gpixngqdu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ggmqxroes.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gkxdoqdcz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/ggtnofvzp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gkwuencii.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gwmrpmgml.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/ghgfirhpb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gptxytvuu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gwrgybkqy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/ggoxbxebh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gggqaofha.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gaxcvnzet.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gslseswwh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glsmqeicc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/glqtrmbzo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gyiuevdju.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gopacrwcw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gjlpmanub.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzrllagej.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/ghjseftee.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvdqnwplp.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghrzuldhv.sHtML


<!-- 参考信息 -->