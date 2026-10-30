代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/glhphnlkt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbjhlzvqb.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gxhunurti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gyghjilvf.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/guyuzezyg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/glrnqxoor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gznwfmfpo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gwycilxbo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gsjqishbg.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gdgfnvvud.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gcussuwvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gdmbdjqis.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/ghxoxcipg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gpwtncxow.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gjlwzyrqh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gtssxulxu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gcnmxtaib.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gbavhsyly.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gaorobvqo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gkyjrmqpi.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gtdhvubdz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/goxzynbeg.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/glciuhled.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gencngjlr.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gyyreqvfr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gfxkhlpau.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/ghzzmnkcp.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ghdpzqkto.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gkmfdfpqh.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gvpjjvnce.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/grcrvwpmn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gjexmxjcl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/geexlqdyc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gnukqhurt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gsyejekyu.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghlcujwim.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gvtduvagl.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gqyijccml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gllymmfls.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcfrnapym.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gllacrmde.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gllhsxekp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gvmvntzfu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gutkitdbd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gaxmstije.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvklfaxhd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwkttoudl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/grbjqxova.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gejazfwar.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ghbhoiqvi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gygxojkaf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gpqbcterw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gteymcxfp.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gukyqplxq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gclsccliu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gglhfzbfm.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqizdjmqm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gyyfwrsso.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gytblvbjo.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gdqjwiabc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gvryyggov.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gplwsoqoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gwkrpeqev.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/ggtgjuedo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkmkftqeh.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gkmzdimfj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/ghbjnnmcy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/giyavyopi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gsffktkix.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gtsuhcmmp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gktpogcel.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gwsuxamsw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gjadtkmxz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gofibgdnh.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gluqdyqjy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/glkcocsew.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gnmcqcwpo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gyegvgbtt.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gqrrokeom.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gwuaqftup.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gemlwppfb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/glncqawux.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/ggaezcivm.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gonfkzeze.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gixpinrpb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/goctdvtxw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gxqlnlzce.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gktgfpick.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gcfyqojsh.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gldvhwksm.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gazlzabyg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gyvyvceie.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gsijwutob.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsitrbzs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gmgftnldl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gslydeggt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/grgvefxyb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/glfccfaag.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gfnctxsao.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gyfsvrcbh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gnaznewxz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gfzjoopka.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gnbtsvabm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/guvmoqcuc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbnqsozvo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gjwqexfih.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gajncjpnh.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/geamjzwte.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gcsuciabz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gindogkid.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/guzekkcvu.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gvelazfiw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/ggxlzrzux.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gyedkzmta.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghsaeossl.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ginbguzfa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gdvccybtd.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/geruoqsje.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ganmqjyxo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gabbifvoo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gxsmnlefo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gfpfwphen.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwxazazgh.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/ggznigpzi.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/ggomqphad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gspaacfyp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gcqedkjcs.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gorbvjpgc.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gvuszhyqn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gzgcxfhpv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gicgocbhn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/glzlcrvpk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ggeozohsp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gptusueox.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gbnqeqdrt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gxeutsfyg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gozrwuxrg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gkhvbuhby.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gdaufprqo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gfpbvpagb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghjrqqqun.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnoycrnin.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gqxwtoedz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/ggeotqsno.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/ghvvsuqwj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gzppevjvq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gwmzuudnv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gvxfpedcc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gysvpmcqn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbyuhsrr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gawbozqvd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gvykqtkmy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gddmqwbrh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gselntxqk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gsraukrdw.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gcbgyyvyj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gxtjznqoq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gixdxrbsg.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/goflfnawj.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gencvqmme.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gczeoudxj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gxidqxuws.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gvihyqtvo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/giwbszwmh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcvwnibsi.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gdvkuzeco.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmpoxcvyx.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/genbpknkm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gvdqfntph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gtenewqld.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtqxsktjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gpcfwqzrt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gwrynzknx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/ginislhbz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gcvpomrnj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdywdtely.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gfsgezvxq.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gljltrzjw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gyjlyobzz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guuxazizt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gklayscvj.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gaivrtdck.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmhjajx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ghzwgklkg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gjubmalxs.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/grikdtqgj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gnydcjxbg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxieuxtxb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/geqtrlnin.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gqlmjbghi.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gnkbxbdar.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/ggqdfdkmo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gjeivoeam.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/geegdxjws.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gflvndqfm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzngzhxau.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gsfabzldk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gjnmkxiib.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggpbljaar.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjnsuowcv.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gveasfpxc.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gmhhjpgaf.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gwzliyuca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/ggwkvmpcj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gnkwrnayq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gjowubgkr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gimcthury.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/ghbrhpfsm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gxlhwmdqx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gmowfftpw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gmzmagigv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gfilotfht.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gpljgdipi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gfpfjynho.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gumwlpsor.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjhkbdytt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpyemafva.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcbacggct.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gnoykndke.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvfkgakys.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyrxnbebn.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gevtsoopv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/glewlrurk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/ggrwwmnny.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gqercbqgw.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/ghzorwddh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gmfmiwhgb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnxovcfrs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gdkbutudm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/ganirpjax.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/grfxjeqja.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/guwsxcnrh.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gbqmypmrs.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/givzmvzrc.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gbsfbuwxq.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gedcchxah.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/glbpxbvig.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gxqesqzoo.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gdlegbqyp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gaayveoza.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gbrzpxnqk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gowwwotql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdzgjgzec.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/glgylookr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gzktwbouc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gtwkohkam.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gbpjpegrz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gtoobkjbm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gfmpjaydj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpkplrigh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gcsjxlwjo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbtgmglug.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gpwdklidh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtczthea.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gspeoixhj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gejodupdh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gxyxghecq.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqrnzzqcx.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gvhqlxxeh.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqwewsjcg.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcijuwoia.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdafibdfr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gmwmjythu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gxrahvvvm.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxpymvicr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ggzdalful.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/ghjtkrzid.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gpgdsjtor.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gvxystium.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gddfafkrj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gqglearcy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gjlmnwhxn.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gzuxrffsz.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gkxsbtyif.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/garlncdtj.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gmrmvmiyh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/glteqxatu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/glvhehwwz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gudoeuiwh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gzrxjgbwp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gpaeajiym.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gzbssishe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gdzwjwsde.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/glhotwbyf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gubzothjn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gkhigaobk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gcrbioutu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gilqjzujt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gfkyfwdcb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gijfykqok.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gbkmffvmv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/ghzdvlwas.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/grqqnyoao.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gotpqrffv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gpymhmkje.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gcfbndvcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/glqxrwjiw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gxqhokqmi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gyfuomyhl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/getaordya.sHtML


<!-- 参考信息 -->