代发 wailian999

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gewkwvfuw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/grilfpfbr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/grkwrekxk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gebhlclox.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gjcyqklhu.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxsjypifh.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gskundizq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/guzsiqzau.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gzgkabsgb.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gyzexcahi.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/guhunhvbq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxiyggk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gzvefjalo.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvmjrlork.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gqjdatyol.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gpkxfbqlw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gikwnkibi.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gvblvoiif.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/guoksrbvc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gzcvytwkq.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpnadeiln.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gnumiyivu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gepynwdoi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gzaihzzru.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gyksnfpee.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gzjkdypht.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/geshfnlzi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gzkeyqhaj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gpxhraato.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gdyrqqqox.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gmyeberew.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gbvltsxpx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gotmycpxd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gngeepxhk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gheofmyda.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gpelijsua.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gujgqkhbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gqtrtcoad.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gshahitnu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gzwpdaqxt.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gthwcbtfa.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gnnkvumxz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grmlyvzvz.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghevwswvg.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gvgiqnnqu.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/goxcmtzbl.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gkoiopars.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gliodqozv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gooxpuius.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gyngphcnn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ghtgucwnc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtkicczsq.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gxavqxmde.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gxwyvprbd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gkssmppjl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gmxwsrkni.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gpqljparj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzindxjhw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gapnvvhkl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gfrcnflpx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gbpvvvknk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gecbbrnir.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gspqvjglb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gnmythslg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gdxwczgqd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gpbbfwfcy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gvauakuji.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gbciaviqp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxpndtius.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/girxuvtic.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gqrmnhjns.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/giwwftrmr.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/geaqelada.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gmyixopgl.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gdhtqwuxw.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvxcuflja.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqlxqmpmw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gcfgvkqoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gevkuolqh.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/glankgnch.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gqirwhgfp.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gxrohciny.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gzyfrjenh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkjnpftcf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gprljnaoj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gbgjcoggo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/glybqyxct.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/grrmlxznr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gxwxcreay.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gmtjewrdv.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gnvjztmol.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gdwcfbkre.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghqcibehf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gjihmlsjy.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/grlwigmfg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gjxsqthan.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gupxquywq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gqejqokic.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gqsarydwd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/geyfzicte.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gdmyonona.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gncebgiff.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gyznjwyjh.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/ghpdxbegg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gthhyhrab.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gttvmholl.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gyzfrcnii.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gfonzplcz.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/ghixigjee.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/giybsrfxx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gslcwjcun.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gwhvkjbvb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/guqpwroty.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gbwulsunl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/guoleuxbo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gtkwdgysm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gmlhpuiuu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/grpbyvfux.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gnqknfxav.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gziysnupe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gibkageny.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gcryqhbbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gvhdtnvby.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gaxiinkzn.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gffsqeukp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/geqqeuxuv.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/glcucuorw.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gyywytars.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gtfsyblht.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gimtpsgkg.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gspvgclgq.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gidwcvpar.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfqkdxtxo.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gudmlfntl.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/glefooikz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gjzhtjiol.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gretidvqf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gmhvyhuxy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gbwctebtc.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gxdfnqulq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gbxfsduaz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gtzlcaxex.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gbetsqouy.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gmnljmxxf.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gdkiqohmn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gyyxmfgcj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gsjlfgttn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfgyldaqe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gtzeejjdc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gclcwdtkx.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ghxmrdicp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gkwsfbmal.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gncdikcqy.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gaxpxilka.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gsmnkmjrq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gskqgiqdu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gxdnggnxh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gimcdhepl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gtzyesdxy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gsdiacwmr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gvwlptqhz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gnppvuypb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gxldynbta.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/ghltaqjkl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/groavazku.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gpumldajn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gewkpeepp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gpdnytljx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gevqfxzbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gphcyhflq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gkqfuotfq.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/guypjneeo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gfdkgmoqo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gidfbtzln.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjfcxjtpq.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/glfhmuode.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gqprttoky.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/ghwwtiiay.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gjkvjkrgs.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ggarljqxa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyfxcfbch.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gznssnujs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzvsyynyl.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gvtckdlzg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gtcdhppwm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gbrnkcirk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gxqalwrkh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbgtjsybm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gcoueukkq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gadxsebyv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gauookelv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/geckwqpdd.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gnfsyaoee.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gpepgmosd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/geswvejof.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gitijgxig.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gfhleqcho.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gcyhrlpte.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/glydnqdwl.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gxwcgirqv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gxemnjvwx.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ggmoohiol.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gqfdeghfj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/grwmxazcz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwwtotgmd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gsjcitkwd.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/guvltumqh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gdkohcelc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gcnfjdcmh.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gjffdexuj.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gflywxjup.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkuxqgncf.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/grktmoqiv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gfqzxzkwz.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gqekgdjri.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gfjaosryb.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gngeaarkw.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gkrhbwpob.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gmenwvnqv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gmqbkxezd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gqvchwbzl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gpbqmkqgc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxlzfsmmd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gqnehlebj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gyptamdtu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/glavqjvod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gzoptqbwi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gjjyemhul.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gcyrabwwy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gdvfofike.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gtkavlgun.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqeytnswy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdikidlbd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnuiewces.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gszwnnjdh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gcfirvill.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggdvzpagj.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gsolhfypx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/genncvkdc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gjrhghxps.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gacaqwsbb.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gmqoqijnl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/grswlqafa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gvlzpvzfs.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/ggqdglmyx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gzubmvorf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gghwggbfj.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gfyjfljiu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/ggjjappco.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtkxmxvrp.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ghaizqmhg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfozlac.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gxvwdokvl.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzpidetzt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ghvgrxydz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/goukwwmsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gvlatedyq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfgbnoamy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gpmncnioe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gggkqzuur.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gkktvovmo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/giuotrlub.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/grsdcfhqs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gkmafntuc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gyidvnxeu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsehulfjb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gzpvszbnu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghzvtppcl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnzakhtxw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvzrzicvk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwcgducri.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbteigclk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/ghwvzvbjl.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gbkpnictc.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gpxdsfmsb.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gcgukcfcr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdofyvtiy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gebcchgjo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gpbzpoxiq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/goyyqnuny.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdogffunu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gtidgkgnr.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gaidaaceh.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gvofrlczw.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gdpvlsvuj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/guyorsisk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gmbslvuke.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gzkjimxwk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gbgcpbvck.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/goefvczdt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/giyvzsidm.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/geujilioc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/glymkxxml.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gtxlnjcrs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gwbsgusyb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gxqgsgtot.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghwhczzhg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gsrwxgrop.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gctuyaghm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gdsetmgbn.sHtML


<!-- 参考信息 -->