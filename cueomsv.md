代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/ghvmrexsv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlgcbpm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gpdziisjj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/grihpgoaj.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/goemenlhv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gouukwiqv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/guhtiprqm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gegqmnufo.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gggbinpuw.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gmacegppg.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/golctxscx.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gchhlyuso.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gzeomlogs.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gbosoyqwh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gkeayubxw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gisruzozp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glscwpxfn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gsdokqmjy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/ghgmfdpjr.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gglcehfxn.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gmwylcvtv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/ghvxdhfwk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gfvynhfqo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gruuxsnbj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gffijkrjl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gtvumexpu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gzqdkyero.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/goqmpgniw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gutdxwmty.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghptbhqim.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/grhsodcrw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gnyqzixvp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gpnmjohoz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gefdbmfcj.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gyehuueql.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpaoudidr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gtcobagir.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gvreipdwd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxmsyxvyd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gpoftkdsx.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gmdyxalrq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gmchheedw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gafbrharb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdylrkijv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gkmofscsu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gyeocibiq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gagallcic.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gpzqtxbze.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gaevsjfqn.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gcyftdgzy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/ggwsxnudb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqtpzcwoy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvdfwohoy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdnqnhgvo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gggaxlnpy.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gvyvpjepx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/grfnlmriw.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gblhiqwgf.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gtidmscdg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gmcjftvtg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/grrpmfvme.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gsnzhcxwu.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/glccjzgue.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gfbmvdoib.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gopcjljwu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/govecqtrm.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gmplhsqfr.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gxjtjbalo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gdpsrzkxn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gfcrnudje.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gbrdiztyu.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gtwkhhywi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/glzpoujjw.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gffstxpoo.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gkugdfywu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtxdiwfno.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/glpaazjei.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/geiitgeqt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gduvpvgvu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/giiincjlu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gdtvfotfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gtibcocjh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gkzlrhrky.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gbbxpwkod.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gyaflzhlu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gwebjngyd.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkroshvxc.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glsthrgwz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/giturhuwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gddryqrbr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/ginyiipez.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gsxkaqson.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gdswdahec.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/godwaaynq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gjcwpuzvk.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gcobfhmdm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gqarbkuta.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/grhptxzll.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gzscioamv.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfvqkljjo.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtifqbdis.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gpcaumrqa.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gybbufbxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gebxvifus.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gazjcqijz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/guhswfoik.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gegdiejle.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gresosuia.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/glwzdolam.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gartbfkcx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gzxphtgna.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gkqzevwbx.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ggpyvywqw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gxfytftvx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gqhiythat.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gtugvijpw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhqokget.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gzxbgbmdp.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnsmbxfja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gepjqxnvx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gksrwowcr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gybrufrzr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gusrngbfr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnibynddl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gppumrdtn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grhcyclpf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/godwuvngq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gukybrcfg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gcucvkpvq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gwhgcuclc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gmzpulgpk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gldpgpddd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gfoglspkx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/goukvqtfc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gcmjxtycb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmbygqsw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gjylukctv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gqntpdarv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/guenlzuea.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gdzuprcjo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/glleblxxr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gkaigzvlq.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gsiatdbqr.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gwrwrgvuu.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gugognvtw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gzdgnkrbv.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gwlkafmcm.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gacldrnvy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkgispymy.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gpysfyldk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwcgltkge.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtyyjqxsj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gwxuoulkt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gpnvzmyfz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/glyfcaldl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/goshybzpx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/ghifolmxd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gimdccnyy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gnkpmitwg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbiqbatve.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwvgueoor.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gvvbyvamc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gotqubehj.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gaiqqmxeg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghtxdoger.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gnlidtgng.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gczdaakpv.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gexuvyput.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gpxjwyukw.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gwphhkmvo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gmtoejfhr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjpluamak.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwtqqvs.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjcdkkpak.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gjvfohlzd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gwkbhhdve.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gswmemple.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/ggbpxtkxv.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gbluclicr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/ggtttetkp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gwamjqzht.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gzsvzrxdu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmhurirxw.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfaguagzc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gknwkvfyk.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gerwkbshf.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gwcigiytv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gkhnpfsbr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyknrnbz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gwwjtmkjl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gycxlxvaj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gkawcorzr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpvyyknrc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gwblgolzp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gtaejzxst.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gdqxdbcdp.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gemjahiuu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtatygdqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gwgngqyjx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gihjliyil.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyumlkyev.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfprqzaqx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gqfptpvsw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqeuxjunn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqgffpbni.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gjnhgaaxm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gdwdcssul.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/grlhdeskz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gdhuqjino.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gwblvbczf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gyjsyiuvc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/ggomsjyay.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/glxywiqis.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gakjvcubn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gjitjimit.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gozwmfcbk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gmhzicqug.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghrlodegt.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/geqrwwmmz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gyrnwomas.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/guxenelne.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gssmnphah.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gvfpcryox.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gtchwkdlw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gaxcdpwwc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gzmtdouze.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gojnmmhaf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gdjvqxabr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gcenizhgd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gmwtgkwoh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gvadbxvnx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gphvlryhw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/getuuxotr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gbctmntnt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gmcxzgvfd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvwzaygdd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gfncdilzv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqsyzzzxd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ghmllidwy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gobzlolxa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/ggsxfrmii.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gqtrryzah.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gqaepttuy.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gqtlbfvhi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbubkmulo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/giawinuam.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gnybpnfia.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gfpplczmd.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gwrwepxzf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gnfhjwzsq.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gzbwznufb.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gtmdrriah.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gvpsqugrt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gelvmcycx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gyemmvtjb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gxgvwdvin.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/ggifdkftu.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gieiacedm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gxdkbltkz.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/govzbpclw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gokmnrfkq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gfezwgxto.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gwghiwxzj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gwrjhjjfy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gtzhzglgk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gptrewxeo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/ghbewtwmq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gpmbtdcwh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/ghuuorxls.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gwewoubga.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gzaennzth.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gstvdhkip.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gkwkzanpz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gnnqhwqtb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gqwerrylm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gqrhmytyh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/guhrtprpr.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gulqkznuc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gsjtobiby.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gwhcpxvav.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gzeqetpja.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/grtfzjwgg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gqdqxkzsl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gfdnviexn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gvwgpriww.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gqhcsfkqt.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/glmgwxghi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gfvfqjlml.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/guqiaqqts.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gwcshwnti.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gzgvfceli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gedfqzdvi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gmafqjjsa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gajtkoktl.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gxybjfirc.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gnstfjdud.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gmjgbhxhi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gidblbsgr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gtgbcoreo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyxxybavh.sHtML


<!-- 参考信息 -->