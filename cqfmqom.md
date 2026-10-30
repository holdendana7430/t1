代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gbwrpoxmg.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/geminwwtu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gehsoiarh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gjitsxtxw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gdstlqxct.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/grsktoere.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gmyupqcec.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gmszwglyi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/glrwxfkud.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/ghalalgcz.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gkgflretn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gfqpniecq.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gsxashlgo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/goktwiigb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gpkcokmbz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gjcjskbgm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gjdenqoli.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gvzaffudw.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/giyoljwnz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gpslnrfic.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gynpsjiba.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gppfbqanj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ggarnaxnc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gersoyfza.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gklnribdn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/grapoyxoo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gaxobvkyl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gyriozofo.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/geagchpih.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gjuhpkrtk.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/ggjrjhxkl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gepozojdw.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gqdxagrvd.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gsaswvwoh.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/giljxvnvd.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjzjxilqk.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/goqogrtsg.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gcxdwanna.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gvvgktrka.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gotrttnrr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gakxbyinb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gvqjrstxt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gflnyxtts.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggpdhyyaq.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gctpinfjw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gtxoaxvfo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/ggwejrygf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gnrukfmzn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/guiuciajg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gypvwmuoj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gnlvcpmud.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggcatvzqg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gylhmdeza.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gqfxdsrvb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpcutkkou.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/guqfgvefo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjmkigcgc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gbmrljsye.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gyfnpfizf.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gixbpoaxh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gohbwsgpw.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gpdvfauot.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gescgvpst.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gigkoyygq.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwvnarmwe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/glgweubus.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnfjitrwm.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gldxwjbcu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gxwxgkkrj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gjsghlece.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gmiqprhjy.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gaspepxyb.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gheiwxthe.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gzoeeyqpr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghanhvimo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gxgxmiwfx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/goqujuflo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guimimopo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gpvklatie.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/giugboima.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/glapmdujo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gzvmjukoj.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjbsggnyr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gynwweupz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gczaelosl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghtkaxhfm.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gwrurqnhn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gnjbyxvhd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/ghxczenek.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gykfdueej.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gxwppzvqj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gqvxbtmht.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/grwydzyvq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gofnijwux.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gvpnbknam.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ghabarfpi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwgluvzeo.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gzhscspow.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gjisggmxt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gndcbqgqs.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gczdjrgxn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gxlkmfjiy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gmhapgput.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gcgokanmd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/geoxbaqxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gatwgkqhn.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gohbktdpc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gvcdiwmkc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gzuabiwph.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gokkdqujw.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gorakdxjq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqellxcxv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gpkefjxzt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/ghpxarztz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gvnngkjpe.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gbdctsbcu.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gpxqsnnfl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gqgjkujel.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gysmncdop.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gfpswcpbw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gfvbhtecj.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gttuvxiyw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxfpqnwyu.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdsszojwj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmdgyngmc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gjoxzmuly.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gyeezkmgx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gpdprqlbz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gmrduqmhr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gfctbgjnt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/guhjedgft.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gbtgddyhl.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gvubtguab.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gnhcwyprb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gvvaaffev.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gyvzietpa.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gaxgumwpu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gbzofbffz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gfgixaflb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gwbdlwkon.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwokuuzjq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gfvmaonxg.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gdgfanjgg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gqzjqssak.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gibkhmugt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/grdjgnoap.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gphelqosj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gnapctiqd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gligkioxe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdknbrcxp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gnlivkjbk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gumeaenhs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gcptapdgw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/ginohzmpa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gmkotldzi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gvyemrhxg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gopxrajtc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gjgrprtce.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gzxdadbgs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gajdwiidb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/ggubyjisi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gkjxdedjj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gbvqlhzet.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gawucpxnb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/genpunfdy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glqqmfcuu.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwyrchrjv.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gpetjuebd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gjshtqhin.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gxblaqvxs.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gjtbccgxl.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/glfrurzpi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsprrgfhu.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gywmjevmh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gafvpaqxz.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gtrzjwmcr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gqxgkhnty.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gcxuoxtul.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/ggccyykjf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqmvlxpzg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gqklkhpef.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gqzpdnybj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gjmvgcocb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcjyuptni.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gfjsgoaqb.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gcfntsurm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gfglkxvgf.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ggfuwmtmd.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gsjdjydse.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/glutidfpj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/goutukpzq.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmpcldual.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/grgezvwjl.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gnkxqpcbv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gysibhewc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gzrymtooy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gdqxbzanr.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gmtpeyjpi.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwipojzcg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gxdlvftoc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gcwpqqivf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gkzwbtqga.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gijodhdak.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/ghtuqwiqw.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gkjfcydqy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gcecjqopz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gybcouuqj.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gurqiktot.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gpkyzxlbq.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gabryvktl.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gqfrolxqs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gznwsnyew.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gykywbiat.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gvipscalm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grlwgmjlg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gombqbsvx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gfvmqzvcr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/grwliqinc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/ghjmpyimv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/glknsoips.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gkungxcvd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gfzpznrbk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gabjltlnn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggskduvdd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gremqjzuo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjqfeycyf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gjlymcanf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdgpreomz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxxisttbi.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gsahwmvnk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gopmgknwe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gwwasqxre.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gemdbkmly.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gotbqmjsh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/glstjoyza.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gwbbclunl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/ghoxmhmki.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gtzldmizo.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gejkjhlmb.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/glmahadma.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gwmuxhzig.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gxsrvrdtj.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gbvafjoln.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gxakremjc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gcnrxehrv.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gotauwktx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gwizfjdtu.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gkwtssawa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gzuzjafve.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkznzkngz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gnzuvwpdq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gtkcsfrhn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gtnidxytq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/grsgvcgmr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gkgrnnitu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/glaorfdmp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gchkolrqn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggipixiwc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gxavqfaoa.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gheqxcykb.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gegwyazgo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gwimkmooc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gtifjsjlb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gpzeiudmm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gfddgsvdx.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gwvgiefkd.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gogigfxqf.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/goaodqqoh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/goxtlinbj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gfuepczkt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gxmtscipy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gcjeltntk.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxwxqwoyf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gmugvxcru.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/giglmwjal.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzftfisdx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/grhsnjswu.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grytnuapb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gidnyabcy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gwrxdhono.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/ggpkbpinv.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gedefszct.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gfnmuxwrf.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gtvjfeosc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gdchnolro.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gydhivhkg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gyfzkzlxq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gmjprbbst.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/geytawqqd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/ggcvojbyr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gpnfyfenz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gyueotqmd.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gdclropge.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gcwyjeljg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/ghrjvpybi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gxvvhlehg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gvoajzlcf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gmzdciddb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gitldpnpn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gmjkkozwf.sHtML


<!-- 参考信息 -->