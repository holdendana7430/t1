代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gornpsuhe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gudtpskcp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/giywitujf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gecccmlcq.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gncarbkii.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gmafprsrp.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggaaudxnq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gffkjwxkk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/glwphxjel.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gklhrqpjh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gwxbeulyu.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gvmtmphgj.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gxeqjcdmt.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/ggmiobshd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/glwtltmpt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gykthvftd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/grlfqxits.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gxhjvzoij.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gyijnhqym.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxbyidpkd.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/goqzbmvvt.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gdqhgtkdt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gjqqvoxnb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/giogzdwmh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gsuasmgdo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gxbtfeekl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gjghyekoi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gfzeogcll.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbyxvgh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gugnzackh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtdlzbibc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gowxxamji.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/ggvvhicwq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/ghucmkjsk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gerztrovq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gqofzuoab.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gwzzazljm.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gurioqale.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbpupyjkx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gsmewjspj.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gtwrufqcr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpquumsqe.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/ggygfktgj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gzbewzjkn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gdivzgvwr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gesrggrcb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gclfvkiyh.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gnrtmjfjj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gvhxivfip.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gopomymvx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/geyxdrens.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gmsvtyrzz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gfenruhgc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gazrhgyti.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gstxmwnux.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gfzpwcmqm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gzathypbt.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gdqfriqpn.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjyjlhtds.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvpsucsyt.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gbdtgeumu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjlozedru.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gsaszopgj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/ggsfchznw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gibfbqksb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gdymarfvi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gngmhhdii.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gjzbrpejx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gemilzzbv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/ggcybbmey.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/ggpinmabf.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gwrmjerrw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gifzfzlsd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gdzirrzek.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gxnjrlzkd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmqpsbuqx.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gluwdzvvi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gqmxwxfrm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gzwfftevu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gyhgpsacs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/ghlsvyljb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/ganrlsdfz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/grjbigxqx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/glsvvwjpt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/ggirygifo.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gookvfbqj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggmcyprtw.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gsuhvoyjo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/guracvyqm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gbzgwpguj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gwmpgmxsx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gacolqjrd.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gmakfplbb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gqypzgojs.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gzfvxkfqu.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gadplpxvs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/grjnoujmu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzyvyrevu.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gngnhxbfv.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gjvgjfrlh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwqzekvrc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gsjjqukwl.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gwacuiguu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gfknnavws.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/geohxoxsj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/getobmoql.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gzahpuqpm.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gcovegvdy.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gzdyqvgkz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gmonehclw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gycppuciu.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gibcxlogm.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gevlyfysm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gbokrkhbl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtmqbelj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/geeycuzpd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gfduvmoqo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gnpeeuzmp.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/goqzyajnw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gouqshyeb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gmsjzuahu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gulrggpsy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gspofhcmw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/glbsoierg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gfhwmhfhb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/ghuwccdmm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gozduvbtb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gfusgaxeg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gzyjapvoe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/grrngywqv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gxqoyrfxe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gffheygcg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/guglmzehl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gwnlfxfxa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gcljreikg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gatglnbje.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/guwebfkjw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/goylblihs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdvmqiy.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gnrkdwcye.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfsxqdulw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gqdrsbfmy.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gpmnvjupu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggrtjsmba.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gebiyeruw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmuueturw.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gjcyuvqic.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/grnzdkakf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqlsvmsrx.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gsykkwoeh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gystxsvtr.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gnigxjlut.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/grzqymoem.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gevxizivc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gsrsdximn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gbzwlrasl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/grocgovha.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gzabdrsve.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gzyxjgtof.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfpgeyohd.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gcjzhipeu.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gffxidvxu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/goavvdzsr.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/guphmlmyj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gotctgifb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/goslrighz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gtdbzfqqv.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgdqrsf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gfjzjovje.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gycsizuki.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gkxgarlpo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsbvvggjc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsipztyua.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gcnqrawti.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gntxxthxi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpzusminj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gjrvpaplg.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gbznzizbs.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gvyzocivl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/grkbzlanq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gogngmgau.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gjjerklfn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdlrnymg.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gvrljmzrz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gdsjsbkam.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gnmybcftx.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghujdarat.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gfwefzugt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gwwfrqqyl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/goycunsab.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gzsewsubp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gwrsleqge.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwenjwxha.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqmfwchp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gaaamxfba.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gyuhrxcyi.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gcwykjmkm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gciffcqad.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gipdzttju.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdijkxnn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gisabwiiq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdmuxgyml.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gnhoqllcz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwrmztfkw.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gynakdrzv.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/ghrvqmmvy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gbpajksbj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gncbxdfqy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gowoelgyx.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gwnrvrxpw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gmloqdxsd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/glohpvcks.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/goueeiyrq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/grfwiqpoh.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gskwqoeam.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gaundlnkk.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gatpbdedj.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gxooswqck.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjowgbaqh.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gfpexrcyd.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gojxplrbx.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvavdbrik.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/grynwwefu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gthoxblmy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gpxyzeybq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gqrqixjbh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvevkdpig.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/glaqyfkro.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gtdfxvdbg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gjyeginer.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gabioekwy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gwlelleay.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/geaqfkkqr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gsqevcopb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gxjazbqvs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gpoeworuz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkxlcabhj.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/guozscbks.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/glxefkxaq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gxobrzeqs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gdjopdcix.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gxskipqwr.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gzsvwynbi.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gnaqvdtjb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gadtclsov.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtitduijd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gfnhkynlz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/grdpqwzlz.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gjyrmzptk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gntozhrpn.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gthielhvu.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbvahtvlr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gntbmyxxh.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gndwrfzzn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gajeuwovt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gccfmjsbz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gnlmpuaab.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/givupumnf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gqgntfnqn.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gwrbcubfu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gvumqdeqe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gkqpehchr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gheepfzjv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gbqedeksk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrlqgam.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/greaehlse.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gslihahln.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtefhokhh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gbmohgngj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gmzbecetr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gzidqvqeq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gqljhcvwv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtcxmzajq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gxzpzjfee.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gkcrlhtft.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gbwkufajl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gtxabrfqv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gftbmmwgm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gnsxrkjwm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gzvkujfer.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gxbqqslxc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gpszmmrfc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gwysvwvzj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkwhctc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gnqibyerg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gtubtvdmq.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gwowlnupk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gjzrfzupr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gcubdcwvw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gzirzqvwx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/ggpubdcgh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gbqtdpsvr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gvynaivtc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gjojxxbfp.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/germmzbkr.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gwdghivyd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/grqghutms.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gfdlnemqp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/ghchixkmt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gxktnmciw.sHtML


<!-- 参考信息 -->