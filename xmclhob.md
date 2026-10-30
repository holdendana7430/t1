代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxonmmzyr.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/grvcubvrw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbaqapfw.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grezxznyx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswgylfnd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunlyrgd.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/grnjrqcrn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkywwdfec.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyvjcziu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/ghejtiazo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fanxiaobao.xyz/Article/details/gocnotcql.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqparitz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnjbthhf.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjdlgdhj.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptjhmfr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/giezmhvvx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvwppbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbedalsk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcaqxln.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmzcxmtg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/glmfeirbj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjblcirxz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fanxiaobao.xyz/Article/details/gmewihlzh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/glwpmonec.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/glbghtpqb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/girqszhpw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvrgiznd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmymqely.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkaxwlrc.sHtML

Java: Collections.reverse(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gsprokzls.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxutdmpvo.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/guthtstap.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/geadnofgs.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/guobvdkvs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaniqvhh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbewydsru.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnpbtbre.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gguzshkia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fanxiaobao.xyz/Article/details/ggtdguyqp.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrulnktj.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gtalzszlh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/godwmagme.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqimvrgll.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/girmoiikj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gqvtayzxw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gmuqxrhxl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggavnbwfn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/goezuzntv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkggsxzxj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbumdhfd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gltpjqlpz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/gzngiqtgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gngxddksd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gedxsconk.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghljutjfm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcojkoqje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gchovuzao.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmbqyqbk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/goppfzjlh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleywvopo.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gpduhalrn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdprfpeh.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gyouzvbso.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gifwyxxis.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/giojepcui.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsybhgget.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvnjttba.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/ggixdlklb.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gbhxaligv.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gputhexfi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gcxixilyf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpnzwmyl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvddxiqbm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxrskgmk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fanxiaobao.xyz/Article/details/gvzaellot.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/gbokgbspl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajigasor.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/granmruog.sHtML

[D17] 最大值与最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gcwqbkjtw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/genxlexvw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhiqcxli.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gsulbdgwl.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjjoubcbg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/grlvedbbs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqhlpajb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdeiiaek.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gddavxsuk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmkogtf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gdumtozzz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gcekwjqne.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxlodzrp.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqkfffqh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/govgayoix.sHtML

Go:   // 手写双层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gqlllsciu.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gimhbohqv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gzralnjcx.sHtML

[D19] 按字段分组
来源：http://wap.fanxiaobao.xyz/Article/details/gnikcfyrd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcjslqje.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorrkszs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fanxiaobao.xyz/Article/details/gshlyqpgc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/govjkohya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqvqwqmf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwgeejwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gksaknysc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/gnlfctibl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gydiuufyk.sHtML

Py:   Counter(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/glppfatye.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbdnmuya.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gvsvwnntz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gcieaymrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gpepnrazn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gsendwaxi.sHtML

Ruby: arr.tally
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpckvwvi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gacktythl.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcehnwnll.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/ghjojjcty.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrulaouw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxdygwoz.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcliqvjdr.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbeubrz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gakldsumo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiftaart.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogmpwwjl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkofueqju.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbrhmiug.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gjehlldlw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsppamkqb.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gyifnwobv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/ghehhvcwt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphldmfpv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/ghrfbmpuh.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gzmwhgnfr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquaudutk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gusbyuqgt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gnqjeyxjf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gltvfmdvd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gzesgpjoe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufatvqbq.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtineoeul.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fanxiaobao.xyz/Article/details/gfucxngkr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fanxiaobao.xyz/Article/details/geonbftzg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fanxiaobao.xyz/Article/details/gztcftshb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gjofmpdij.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyagorhq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnhkwjot.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhapehwp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gymbfhsei.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxigpsdzu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gevocmxfc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmysmgao.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/ghiqrgtjl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhdqwyat.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gyonrtmsy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvraxxijq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfpisyi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkshcbgb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gqhmkycui.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyirehjh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhrrpvyu.sHtML

[D26] 数组转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwosnehao.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gsvoygjqd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gjeriyzwi.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdcumaer.sHtML

TS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnbcgyxm.sHtML

Java: String.join(", ", list)
来源：http://3g.fanxiaobao.xyz/Article/details/gapdaqwwn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbasicfgi.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gyidvxxob.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gytlxacwx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcndlyiy.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/guvyhteot.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gluocfqma.sHtML

[E01] 拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gerrfwirg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fanxiaobao.xyz/Article/details/ggabxwkgu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxwqcauo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gpiugpvnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gnpkmchzr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fanxiaobao.xyz/Article/details/guuphisup.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gybappuwu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/ghrlegxkt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gbnezbgxe.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gteujeuhl.sHtML

Py:   "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gxsvehbnp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxmuqgmt.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/giefyqbqf.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gngugmfhy.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genvhwvqt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmbrmghf.sHtML

Ruby: "ab" * 3
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxfgrbpc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwluvuic.sHtML

[E03] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gkjuhqvqx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/glodfydxo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gnvxloxiz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gliageoph.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpccotwch.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/geohkdcey.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gwjyaecgs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmomfks.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddgdxsa.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvacaatsf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gbortlehg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpdqkyow.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gircrvbkt.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggodxunnu.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gwgsvnayq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fanxiaobao.xyz/Article/details/gnrsmayet.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garhvtexw.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/glbgbymsu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gpsdkorjj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gauoqpjkt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fanxiaobao.xyz/Article/details/gdtdfpgpl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghemrorju.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfquwktp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gswvrjkyq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gmckdgejk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gvvczhmki.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/glqrsfzcq.sHtML

[E06] 替换子串
来源：http://wap.fanxiaobao.xyz/Article/details/gcnvsuwyh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibxkcbqf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkksxtus.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjjdgowh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpqspyeq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxsvlpc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvkhcifc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gmtpzqluw.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gtcwgtzqr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gydesbdqg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fanxiaobao.xyz/Article/details/gyhywkqeq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gakwsatex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gnrnefgne.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gbmrwsdfm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgqnurkq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvzqcxst.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gubfsxksz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/gqosmczrv.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqxkiolnt.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/gtxcarpdd.sHtML

PHP:  implode(",", $items);
来源：http://blog.fanxiaobao.xyz/Article/details/gqbnrmmdj.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddpgmwbw.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gogbralkg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuopihs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebgdezp.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaywjtddh.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gqifcizhu.sHtML

[E09] 去除所有空白字符
来源：http://3g.fanxiaobao.xyz/Article/details/gqzrbkntd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtlisummd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaiqqobb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwtoksoj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gpnvvvrnr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gpnvixkkv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqolomdqg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gskbmcwvn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/goexvmhhv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gcakivlap.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gddtwfene.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fanxiaobao.xyz/Article/details/gonzqxagq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqnivluw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gpihqefbb.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjkxvbwn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshbctgp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnsynrfs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/gckygbxih.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gihetfwqf.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsragmwdk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbxcoaov.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gmsutdxrz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmspgqxqb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gdxclrrdj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/giblxwfzx.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcsetshp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gwbjcspjy.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gwychgcfz.sHtML

Py:   s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpavigiq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzicbust.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gusckxhog.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrrogbm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqpszab.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giidigbxw.sHtML

Ruby: s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqtlvhuu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxatgssf.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuesuwmm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaorovirc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfclxlnb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gutawxumd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbeeinywi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfciffbij.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbugpwhjq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimmejucd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqolrlvkx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fanxiaobao.xyz/Article/details/gibfqkjak.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gamjhmduh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gocggeqlj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggofmqjcm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcifxgljj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghchbjljt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvtzbofl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/ghfycmyms.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqgcjvsx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgsnvehx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqudmdlri.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gozjnrfgb.sHtML


<!-- 参考信息 -->