代发 wailian999

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gjtbexzob.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghysqqnyg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gnefeitzz.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/giautslxw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gfxnvszwo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gvwkebhdy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gqzlfvwiw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkbwxytzb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjewbjpma.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwbwsrygr.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/geetgfiqy.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/glpuefego.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/guytzvigf.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gqhvfafvq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gztnxuprk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gstfsqbaf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/guutawxtq.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gpvfvotat.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/godnqqylw.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/grehxlwgl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/geygybuio.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/grciukrnr.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gpxjhbwdq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gvguzaunh.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gtklprbgu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gfqgfukgo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gcyxjszfn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/ghkqqekdy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqpzwlljj.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/grwfxhbca.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gbuutmyie.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/ggpvdcpvi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gxojjzzhc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gffhjbnxg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gbkubmvfq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/godalmraw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gtxlkbqlv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gebasimir.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gpymkvvyr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gxxbjfhkh.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gjmxtuapa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/ghjxjgzyf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnhqnskkh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gmdullmez.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gmwhrcmmi.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gfkytvjsi.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/grbhxcspf.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gygohwbra.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/grdkurudw.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/ggfrspqkt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gsrhbrsdt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gwsselozu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfglkplwk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/ggvgiffas.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/ggkwzwpsh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtdwmfynw.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/ghgwnvuqk.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gzqzldeqc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/ghggtfsrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/giwhkboqg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/grivlxmwg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/godilmmbh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gyqggoqip.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcjfccrzb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gzehdlpvu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gqlgjaxcu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvqtfcrds.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gksqyqlcf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gqdosmjtv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gwfankefz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/govzruack.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gqqhvxndl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gxooyrjbu.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/giycovsjt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/ggadvmrbo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfqatkqfw.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/goidmmeyu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gxjzdualj.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/guymsnsjv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/guluihouu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghzttxmpy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gejdxclbc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gjrezmmwc.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gztnzmcqp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/golascpco.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/giwkazeji.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcoaqazfl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkdpdmegg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/giyyvpodv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ghougnqzv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gpkhwdthr.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/geuecnpzt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gtqrbbxaa.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/glisvyiny.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gdyawkkwt.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gyryndnqq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/grxgzitix.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/ghdmzsgni.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gxceamava.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gryclxnze.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gzhfddqbq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/geioncuxp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gzvdhokcn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gfsrddrut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gkdzpvahf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gqfwthqlr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gpiwanijx.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gptisibkb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gxhywwzag.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/giwelfbdb.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gxfxvjonv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gckhkjcgq.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gxwkfrejo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gqizlgqgf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gdmpbwifz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gkfgykuba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gwilacmdz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gttofizqq.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gcbkiisza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gizmsdztl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gkdjcgdhg.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gjjktxrjq.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gydbqyycq.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxmktsxje.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gqarcuool.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gjxuvlfcm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gqkcnepuy.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gtxlhbwan.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/giqwaxmjt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gxwwixejx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gzyfeoaqa.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gzznyvbxe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gaoisdngt.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdofckpca.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnvjlcsi.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gccrtkfle.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/guujeyxuh.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gltfgtkhy.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gsspjpjot.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gekbnbeep.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gpcmzbrpi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gcggfjfil.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gubmnmsxt.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gnxfzxjdj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/grtadaphv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gmrtpityq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gcvcmeemo.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gcrnbfjoj.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gtcjhpqex.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gtryjtmcj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdxqtqoos.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gegkdqaky.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gddpszxcw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gkucobiyn.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gzdoomfty.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gtmcijtdw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwxllegqf.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gvfbxivgx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/geehwhcpx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gprnghscb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gknlpimkc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjgalqtvr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gbexgixsc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gupzrrpcc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gtyuznndt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gzgbrijvr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/ggflgavwg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gpotosuyg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gwllixrtt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/ggnpprjrc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gnfxoenag.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gkuspowfw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gckqscbgj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gblnscmrn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gfsxhkhka.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/ggchoshux.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gpfvtimoe.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gyxbwfuxw.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gesonqyhn.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxjqhfjby.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gbncjyuro.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkswvswcl.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gucsdhgjo.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gmfzqmcda.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gumgcjfts.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gvkzyyhbe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geigsazbn.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gjoqcgdtv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gfhvkfvjq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvaqgizhz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gnelgtuwc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gntvgjclm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gkbbuhlrt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gyfmpohbl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/graximahi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/geuffuzxa.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gnfizeuyd.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gvmwpiiwc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gofvhocjc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gaeskbwla.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqehgylsy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gsjsctmme.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/ggvwknutu.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/giwmfwgjt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gkmtdwdds.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/ggjlhnpbr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gqnqnjooz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggvsogftw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gphjtiogs.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gymntdbij.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gamkncmyx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gntyyzrrf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gqjmjfsvj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gmmhvelky.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxtjshwqg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/grquhpaeq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gqnpavtfe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gxiizlsnl.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/grvzpjqxq.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gzlzdhqld.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/garcopobz.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gjiclnskr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkbnwft.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gwllqings.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gcxeaeepg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gzralxtck.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/guwzxfhqn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gcsjwefwg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gkkddohmm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gtjjwvukb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/ghfhfnoco.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gkaptemmq.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gpzbagirm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcoliewmh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gqkkgjtlx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ggrqfeoir.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/giqnotylo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwipjgyuo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gwtvaavvc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjgeszjqk.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gshctsjlo.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gbvufpnlj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gaxsqhpuj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gtxcwxjwb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gnpabhilr.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gjghoruqi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gsjudvdqs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gypqmzibg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gsiilcaqv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gnwmtddqw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gitvojhvq.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/geonnukuy.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gxvoxvlco.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gytyxfvhe.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmbvhwwt.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gxjxcncpj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gxuehubyg.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gafvzyqap.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gvopksefe.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gcqiiwwuy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gvqqkoecc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gxfeauisb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkzmmdtuc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gtxlyqhqa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/godsnwmhj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gzaykoggz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gybdoxcss.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/grfibpgpt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gwldurxhx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gomjntgvw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gvvpazayd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gluclpaot.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvvgkigan.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnmshvjzc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gadmusmba.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gfvzqyryw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gxpkreccz.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gbkspvjar.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gbfiouxoe.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrkwxer.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/goniptwtv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gewvfgyyz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gtfiyxpnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gqimtuyby.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gxfdwfmnn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gcpqtapgj.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/goinbygwg.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ghqhxfire.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gfuwqiuzz.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gmwmzwbnk.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/godttzman.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/grzpclokp.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gfwrcvhzb.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gzcurxkhu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/ghunetwad.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gufylqopx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/glsswsvts.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gwkizfgma.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gmmeaziac.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gwgiqlokm.sHtML


<!-- 参考信息 -->