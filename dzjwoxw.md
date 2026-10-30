代发 wailian999

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtleranay.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkntwbftk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigczeklv.sHtML

Ruby: arr.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gddkimdsu.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gcihtxvrj.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gxueguxht.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxrpyfgq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gocrqsznv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdkmoqn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyitoyeef.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gociyuhok.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugsbbiec.sHtML

Ruby: arr.index(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gbwpsenxi.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fanxiaobao.xyz/Article/details/ggqssnptn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubvermdv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gtzbdfeog.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvkzexcw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gabzadyho.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgxgrplh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/ghtxnmyfx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmelfjqy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvcjrfavr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnesfnid.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaccsinxf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gqcsnsche.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmltwip.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grfwgmkxa.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/glkfesdzu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gbntpxyjy.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpcgktvch.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqvfhxym.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gsgnttkzc.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyhhdpkf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gzsxzcaof.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtkslbvc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/glsckpvdx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdgdslxn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizxazfoq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/gaganmbre.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidnthihv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gmjtyxlfj.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/gooqclfba.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glqkofnyk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxvjdjk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzgpsybk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesodkabw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gzgtviokb.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqrkgvet.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrmqwhmp.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/grvnsuhfq.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gvcxkjrlh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdluetjo.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gxtvdpibp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevvcqzue.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwjeoelol.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gcathiivu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncivvsf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fanxiaobao.xyz/Article/details/gphsqfnmx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxkacgjh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gslddsekx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gnnlftczj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsirldwti.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjehdixw.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/geagnydhh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqejhfvks.sHtML

Go:   // 手写双层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqjegjlf.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/gfumdkjxa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gmrfcevlr.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbzfrbok.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gykptgryt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvshwxmk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvuovam.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimhbmcyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fanxiaobao.xyz/Article/details/gnywxcqex.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/ggexblfmd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgrgdywp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmtndeqp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gxucyblzo.sHtML

Py:   Counter(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gzsppoqwy.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjvnzldz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhkienth.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/girubobup.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fanxiaobao.xyz/Article/details/gtmgzuvao.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fanxiaobao.xyz/Article/details/gtuijizdo.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/gqdibusja.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkoutxqq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fanxiaobao.xyz/Article/details/gyjaahlrp.sHtML

Py:   x in arr
来源：http://mobile.fanxiaobao.xyz/Article/details/gujfwaqwn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaociyfq.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbabvszhy.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnzyavff.sHtML

Java: list.contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfaifvoyp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbinrdpkl.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkounwlyn.sHtML

C#:   list.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgydwhfw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gclbwfyid.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghvvagmzs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxtzxgjw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqwmcncx.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnwksgiv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpngznzp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gowvohnml.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/gtpefwzms.sHtML

C#:   new List<int>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfkzwakr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwljjfbli.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxtjelyp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiveqkeg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geynqhbux.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkhuvvgw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/ghgdadjrs.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gufdscwyz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtgyiwjh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqxpqhzy.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjienvtdw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/geagtvxed.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtemrxsz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxtfovfj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesurdpsl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfugkzad.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fanxiaobao.xyz/Article/details/gcsitxhbv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gacccgjjp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fanxiaobao.xyz/Article/details/gqukeqkdl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneerimlc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fanxiaobao.xyz/Article/details/gvvgpkset.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/glbsjddbs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlqxopeq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/goiquyxws.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/geqmfpipb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/gywnglteo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaazzllxq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/giecerqmr.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gshsjczdp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmdjghkh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbilecfen.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gumkkjfcf.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gskcxkiym.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjegpsyew.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gdxdxdmyh.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gdxuzxqdq.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxcgtabu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzbsvpgt.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfioblav.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwixuahac.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqyzeqx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbikqzer.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghewimbxj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbybxrrqh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/glacbbwda.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fanxiaobao.xyz/Article/details/gelktsmbn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjilydcgn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fanxiaobao.xyz/Article/details/gcvgvrqpb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gjnezfngi.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsidgavf.sHtML

Py:   "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqxwhlmf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqskpkdy.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxykcbqjx.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaminorzt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfuxxqpb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/guusqppbz.sHtML

Ruby: "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gqazlbkzu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqthuuq.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gfcoizpal.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeedyhys.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gedqobgjg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggncbazfn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/goawafkom.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gijcbiaxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guskgpwgz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxqgitak.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/ghevfkysq.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/glkwaatej.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpoukyqp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/gxbxkilzk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghszoszrf.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gqhwknkxk.sHtML

Java: s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gapqelrzs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuywyeny.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedwzsvmc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuyqlvsv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fanxiaobao.xyz/Article/details/grchkytkz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfopqjiga.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzjufimi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gnaomlshp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gncauvyag.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gorpxtylh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzryyose.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwonguhh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gggigkbar.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlrashtm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqnqebzh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givpojoco.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtvizkim.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/ggpviwhuq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypisyquy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjddhhsaz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuymkhvx.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyoyfmhe.sHtML

[E07] 按分隔符拆分
来源：http://blog.fanxiaobao.xyz/Article/details/guxefbger.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgfddfax.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/geptpedwe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsbtzfjl.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gbgwwmull.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktaqsdnk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmztsiro.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/geiqblajy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijroyei.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhflbxur.sHtML

Py:   ",".join(items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpodyyvx.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhmkbvjs.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudnokmnr.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/grlmrzdvf.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgyqsqjk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fanxiaobao.xyz/Article/details/gwaiwjfzb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfthqfhbz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbtntdih.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fanxiaobao.xyz/Article/details/gquzdrclg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcghfzoxk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqokzliyx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gucveudca.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamsrgajn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/grkxhlmou.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtafwqvpd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gnrvjomkt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/gyymcujel.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fanxiaobao.xyz/Article/details/gircgtiet.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkyxdlcr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvoroqwa.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/goewgepqy.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggboxjfxt.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gapndnsme.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gidifkzst.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmekbsuf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnqosktj.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtusvlfso.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfvwvgtj.sHtML

PHP:  strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gcuqcvdhz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmownjnsn.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gssvhfxvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjjbctim.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gysitjury.sHtML

Ruby: s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/giaiczsdw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvhaiflj.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlzsdwvt.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gfhqpkykn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqtxxfvh.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gopagqosp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gtwvgjjbq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fanxiaobao.xyz/Article/details/gognuipsf.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlwulnhg.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gppvyraxm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/glwkwvajf.sHtML

[E13] 逐字符遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzotyeial.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmrtvuqc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gssvzbtyx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrcqsmam.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqzdkpfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrvtwlyi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ghagjniax.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fanxiaobao.xyz/Article/details/guanunjne.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtcafxob.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/gjbflmrel.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fanxiaobao.xyz/Article/details/gnburwavy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gamscmzfl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gemehgajg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gedegjwmp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gonhspbtb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/ghrmjbliu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/gfdnhnjup.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsgctfda.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgtlztam.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmpbdxmv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubsazido.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/geovxbfrn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplzllqwi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fanxiaobao.xyz/Article/details/gwvbhrvbv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gpaxahuqk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkawkliim.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gayigezmc.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gcakaapee.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmelfszmh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glduhcmur.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvfumlcu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gekstyowg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefrncptv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrlkrvuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gewcacaid.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlbcvzpw.sHtML

[E17] 首字母大写
来源：http://3g.fanxiaobao.xyz/Article/details/gmgqvdlbv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrbpsaey.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaahsxvsm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakxitjuu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklfmrnxe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvdfyrvox.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gzaemtonp.sHtML

Ruby: s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/ggzczdijp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/gnumrqlia.sHtML

[E18] 模板占位符替换
来源：http://m.share.fanxiaobao.xyz/Article/details/grtsofull.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gxjtiecbo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnoxphkt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvetuojrg.sHtML


<!-- 参考信息 -->