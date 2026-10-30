代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gytaoiccv.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gfpubfllg.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/guxasenve.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gkqvzgngf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gjxahtxvt.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ghelqcbmz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/guigwovna.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gpanqusoe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gntobxfqw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdrflpnrb.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gcbaendbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gpttwwvyj.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/geilpukka.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gjwleyoxz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gcfgyxtxu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/ggayvdxhv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcpixioik.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnwfqjqwr.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/geawapfwy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gwntoxuok.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/ghsoycqnq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gxtftiyle.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gfncyriza.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gsugwjqoq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/ggjrioagt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gtniuuzyf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gfeusduny.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gricimakq.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/galjiwchg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gtyewobyw.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gklzzreko.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gdfzzkwiv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gcbibqzre.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkihamvup.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gbfgimanf.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gssqywgav.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gilbricfe.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gwpsqijso.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/grfuezuhp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gyjiowqsc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gejknbkdy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gkcrwskgb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gubyqingg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gypbnvofo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gukurelwl.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gdlqjcuhz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gztgwcwht.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gltiicuwq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gtgemlscw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ggbizqhkm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/givzncdtr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gqwztznho.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gsoywqvrs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gwypikbzw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghazbagki.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gcxmrxdvz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gumpgqnpo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gqjyzmrdl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gagokmghi.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmdgirppn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/goemksixj.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkguuniwk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gywokoynm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gpxwolqbl.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/giluhrxtl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/glprfmmri.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwgacfwmn.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/glvgjzjqk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gvbpzmzxo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gpjtfysym.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/giprxwttg.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/genpevjuv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/glxukiqmb.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gzlameazq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gtezoumpp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gmnceidoi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkxerxxci.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkfhniszc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gajuikvgx.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gvpiadmik.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gyeznuhtw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gphxzpkrz.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gcmulcbrp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtqvagzcj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gltalkjff.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gfzqmpujd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcjcyixop.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gcswpnakh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gupxehdva.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gnfczwkcg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gyvefgcvp.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/ggxdisjte.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gjxwfysmf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfxcqlxhz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gslslggbv.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gtfuuoyco.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gxzyigbgl.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxqcnizux.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/ghqhlpykt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/grvpbkyne.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/glbbntpoo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggeguiffq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gcjucaejf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/ghfkkltpv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gjykdjgng.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/glcbceihr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gujrjppaf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gbfappxyo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gqkjjqbgy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gxhcwxpyf.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gidfexgrr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gyxwkmqql.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gavfcoakb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gprcfgwwv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gsxowtdoe.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gifquriac.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gcebitdfx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gukneatex.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/glfgptckm.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gimngjbij.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/grxqyjcuf.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gbclqahlf.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnmifhvuo.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gcbynrgxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gykuncipe.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfmzdpvdu.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gaosexgow.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gbbfoncwa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gclceyzjv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gmpewezbn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gpbhgxcbc.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gtlvhpqvv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gjoabvtkl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/glyvmbhrq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gchzhoruq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gpnrediln.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gzprvqfmc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/glwcsaolq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gkghonqov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvtfhcnjp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ghujezshc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gpxvmkvbq.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gujhtlyqe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/ggtyqjmtk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gozzbacxv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gtqkcrlrf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gpvnwqdcx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gmorohwxs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gtmheahko.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwcuxflup.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gmrynvuss.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfaetdrkt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjwvunlsp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gpwtysaie.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gvtkqgeud.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/ggaspmtkc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gnrxcotyc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gcfltxzqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gjoarjmlp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gafbuqcrq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gbqunpydb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gsfmlbfvc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gbvvwmkac.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gcobjfspm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gxlvjvgoa.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjqnjto.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gabsjkxpk.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/grigohcmz.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gbznyegtg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghgsvpzpf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gvsehiwgj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gajaqunhv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmcfelfln.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gdakbaypu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdqwztbzn.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtunqjzas.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gbntqaves.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gertdgkhv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gvyxjlzro.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gwvuiyrqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gaqwrpylc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gbnrfyrqe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gvutvyymw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gmmfrsfab.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/glpujtbib.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gbjtwwekp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gtlqtkhsy.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/geidutgcy.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ghjkytbdv.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gvocximmy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gtioxqwdv.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gregpvgdb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gcppxdshs.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gosmubybo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/geezwakcn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gpibwrkqw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gdrexukqm.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqrfydrpj.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/guydubzap.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gbjabntxj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvqiyzyme.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gnslwwpcz.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gewucjscj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gcffbmpps.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gzdewwcmg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gphestmdb.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gywnikzpe.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnzwjxtsz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/grlrbplkt.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/glsoisyfj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gabdgixac.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gqabkpyms.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gqduxhrkn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/goxfbouzu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gktlivuik.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/giekncghr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gqcwrvgiy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gcjubbvbx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gotjrrwwe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gysptyelb.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gliuzyqev.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gsbdoomtk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuniqbag.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkgqqdwao.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxbzoqa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gprpoypzv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcgxbla.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwweochkp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdoatgifg.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gzbdsscth.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gouysbonc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gqvyxamom.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/guggafhju.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gmruxhpkb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gbboirhdr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/glkiacnuy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gbnqtdglo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gxgvbijth.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gbdmkkxiu.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gwqtksxsk.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/glnxnkhmq.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gsulzhihd.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gbeazlbtr.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gdrjmpnoj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gavqringo.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gbbxrxvim.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gqrdtvlsp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gxwozyain.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gdboawppo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gvdphjyvu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gywvismhq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gpenjhunu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gnnxvvstr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gubimtxti.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/geqkksmvg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gnvkovgvf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gtqrqtcno.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gzoptavuy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gcomrsjbf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gjeemltnn.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gczztynep.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwkmirgzh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfzoccwod.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gsciraqoh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gwdjsfyoy.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gjyrfadur.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gtwfuhowb.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gjeswgzfq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjmaxlvjy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpyupuvym.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gkiiflufi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gccsukgso.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gseslordl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gfrfzecdi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gsksbvpwf.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gclzxgujd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gyfsvgaxt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gnvqufykh.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gdbhoatxj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gfzxavwsw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gsgszxktv.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/grkofvjld.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gzqwktpao.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gtxghkoft.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gvkzhvbhr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gsfswtfui.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbvkjtx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnqefjirw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gudcelbyb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gaudhpixw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/ghuhohqgt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gdicbidxh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/garxkbbdk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gwcmrxzhs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/glssitukp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gjsjmanae.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gpxvyqbvl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/goqpfteld.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gvznswmgm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gvhuamtww.sHtML


<!-- 参考信息 -->