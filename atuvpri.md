代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gxtglmoin.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gyukzuepg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gubrgulqg.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gbtffpyks.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gnuqmtqka.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gbeydedhn.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gchqtgzrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdtbvuqyt.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfywqisqi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gpxrejunm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gpivgzege.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gybyeadir.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gcimptfnv.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gdiyexnea.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/ggnmwdqgd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gqeijhwjc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gyfghiwqz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gbephcllm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gbaroajkj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gjqtpuspa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gmrsatmkn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gfffxxddk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gvyjlmikp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gltkjvcwr.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gydezacet.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/grtbgyflr.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gvgkghfqg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/grdkeusae.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gghxsmkvl.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gsokpkzof.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gimwsdhzk.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gtczkpaps.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gfyavsrkd.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gaaienuvo.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gjzjzpoqk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/grafkxvop.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grjkrdxzf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gnyxqzkou.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gwtmxvmxa.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpdmjgqnr.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gluqvvjjp.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gbnflgkzf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gbvgsapoi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gpgctvlvd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfagbmvgg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gxpjeayrj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/guidredgx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gawckboam.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gcrxnfloa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gjrutggyw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gutgynksb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gthlzkdbg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/geypbbtzt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gfilipbbd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/geuxyckxe.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gomzrqfqs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gqopbximz.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfldyckua.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gffwpvemq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/getqswxuf.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gqhoqwymd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gezvskznq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvimpmehp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gsyawddsz.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gsiwyrntq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gcbhkjwiw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/goyroeyld.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gsrhsgugs.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/glmgbchno.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gwejuwxtc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gnqjfncxs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnsjhkvth.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkdflnyor.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gatiduzat.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gpubvgqxa.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gxdzkryhf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gczalhnmn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gbaicgfat.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/grwxcidoc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmldgbgaz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxsxlyvbs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gfxeoyerg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gjypzwsjr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gghgbbert.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/guvyxdldj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gyrjsicho.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/ghdyvflwt.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gvikjuvzd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/grbeputri.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gvqjljqep.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gkxurqigs.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gsxrmbgwi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpetamyja.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gpbudgusd.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gwxigielc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxoezrohp.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gicaeejle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/grxcdtrbj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gzzdozfpg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gofmcgwtj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gafoyiuul.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gaszlpfuy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gcpwcqwin.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gxmtoytxh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gjwwetoau.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gwsmlfkdl.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbthiwmmi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gjlucwfjc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gnrioivkr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gwpvhbdjs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/glkhsrcog.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gcjktguse.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gdvonyxtz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gcvlcqtho.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/ggolyglqb.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gvhkxhvsz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gxrixuwgy.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gimtwkfcz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gczpprcdj.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcecsqecv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwxvxafcc.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/guilcjsrd.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwoyijdmd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gmqtxilqo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/guwuumdgp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gyttdzqwx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gbpdefnxt.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gysfpqtqg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gfgqmpnbb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gjijqycdt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gynleucxl.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gexhflpnh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gbeckaqdh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/ghpcjiosd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gpmfgzgyf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gzlsgykam.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkxeciszy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gubzplmal.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/goiwnzdjr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gcdauvktd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gbgyicxlg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gfrxqbiuh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gwmjemgkh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gsplxfiok.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/guhentabk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqvuitboq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gsrnxkoln.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gkqyqfgtb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gdycjbmts.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gluvithqs.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gayjsjbkn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gdlcildmv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gafffeoac.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gmkxclsow.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gvxafshvf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gpzsswijc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gvvvpblni.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/glwlyccay.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gbsejxaww.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gypilvslz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gavkcczlz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbuwkaapw.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/goddnntta.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gfhtgamss.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmnielbrf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gajtitqyp.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxkcnkzab.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gvzkwvuvy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmnjnshjm.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gcbuuwotq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjawbpubq.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gxoxvtwdq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/goscikixn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzelwrzb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gplmhlvzc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gwhllicfo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gvylusmrf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gvdgcxhip.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gfocongkz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gunjlockd.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gzboezfej.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ghnifrzjm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/guwxaxelp.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gnzkgtttr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcfibak.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbcflmozv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gjdxmjspy.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gvciqcuth.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gswaijwtn.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gmrpeailr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gwjyfipgo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gplrpseyb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gcyotrlfo.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gtdvlkzfl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gidhaikrq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gadevdycg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gcfmmnlmz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gputgmjjd.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gxbxpfzlk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gfxyopxnb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gdutwmpnr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/glxmykdxl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gxiqughqa.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gyapayyva.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gpveoyurt.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gmhhxocsr.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gbvelricr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gywwergip.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gczzsfmqv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gmtyaqogo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjjqzer.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gsgjgvpxt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqtlcwtlq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/goxsmncsr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxxwjphia.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gumoqdxnf.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/glbvilrnu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gknnebazh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/griasacaw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfgztxotc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmrxllmv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gubxilmgd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gxpitewyi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjwogdedz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/genmcebgg.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gtpndjsgr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/getzeyhon.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gacijgzeg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/ggvyvoyjo.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gqrouvqwl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gttipmxoa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gjvxekywb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gehaczbgw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gmsrechae.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gphqhtpae.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gcuveuwec.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gbrdomfot.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gdhrzeegl.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gnstjasrh.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gkwrpyouj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gxmlofqha.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gcsdvqrpk.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gikbkornc.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gnlhukdiq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gcxccends.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gmyqsbfpz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gzkuxfqob.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghhfcljvr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gorixvjll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/grfmicklh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gsdbikvvl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gtuyluknb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gwoolslvo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghfioqcxi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gukgkklgu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gpracenej.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcfijxber.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/grxtktnii.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ghgwdbmdi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvkfsbaqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gbecmuqne.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gdkxouffk.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gplfmhqjp.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtusfxnfe.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghhbxaztr.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/glxaixbph.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gecwmanly.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gbneamknr.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/glhpbwjib.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gfwgervdh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gmhvloxae.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gdazgkwea.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gzbxreiwb.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gcswutruc.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/garoxwhsu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gwcvppshh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gwquwtxet.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gksiesmyd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/galupvhgc.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gmlpkmczb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/glciqdeik.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gxabszgkq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gpaxywkje.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glmwyljnv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gjrqbinam.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/geqqljwgn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gneygicgj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjzyetldp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gedgfvztg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gtbzgknqx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gjsbtvcwc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gqansgmco.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtsqbcczu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gforsplgo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gklnaqmzc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gajtpluix.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gkffxganv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gefhpfmdo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpxfsubma.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gykqsyddn.sHtML


<!-- 参考信息 -->