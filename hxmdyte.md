代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gdubnmrsx.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gipltvywg.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gguromdww.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gitirbaju.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxruecakg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gmfqzaoem.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/ghhvxuhou.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/ghpdxescb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gxtenovaw.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/grcjmvduu.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/glshdrvdx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gpzxkamgs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gazqokirj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gmuxmfjio.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gxphinqso.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/glxzqbfqj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gdntriszv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gwoeszkwn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/grmokypia.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gsnpadjoa.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gsaakzkxy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/goickanzl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/godickyua.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gwgpbdccp.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gcmvfznpy.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gnnlefqts.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/glxfavnti.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqfopfgoh.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gwfqkyeiz.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/ggaxkzbla.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gedgrrcoq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/ghxmziszj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqkgxreiy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gyoyodwtw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gecylaioh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gtkxxrknn.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcwgpfosn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/groexykke.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gmoaqjowv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gmfehegqz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvqlkaccg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gpojuqymw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwzagvzcx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdqhxfslv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/glkbewhaj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/guoukpdej.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gurtvevpp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gvnffocxd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqxqkiswj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gjvglpzob.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/ghebakgzg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/ghrmaqfcz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gbpositrq.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gzzgbqeoc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjqrgunbl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzxcdstes.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gspvlkodo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ggujgznrx.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/ggkkretzt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gkgisjsjn.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gtdrjqveo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gzbwihmbq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gzeivezuh.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gayikidzy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggafcubor.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gpshvlmbo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gywcesyjo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/glhjfrtmh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gkaawsyte.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/giacyrslx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gqtgvosry.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/girypuvjt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gszvopebp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gjvssxlch.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gysslovvt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gklwnhnxj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gguuhebsu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gxmeeoqij.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/grzizwzxs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gnvwkyqkr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gbxannlge.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/graegfufz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gkgnuoagx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ghqcchwlz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/guixpqfte.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/grvpthxmy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gisnhcfdn.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gmzlosxru.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkqywjzzd.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gaceiqyuk.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gnwfniosa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gugmtvesm.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gssbswyct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gcfmkvsoo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gxxaipzfa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gnaiqfuoo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gfdrrkjdd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/ghebkmkbj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/ghlyhwqyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gpozxgodc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/geujxqoac.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gqsvialqf.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gkkfbbdvv.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gvcfktsdb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gyzgeqrwg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gcpuyxoox.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/glgugipvg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gjemyhhze.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/guydtwivp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/grsdyhnys.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ghwdfiqtm.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtixfkg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gobmuxtvh.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/griqrwjfj.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzyszvurn.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glcbljoia.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gexdbjysn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvhuwgwuo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glexfzsck.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gslghvbmu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gevslxrgt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gjukkpeak.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gulphxxhm.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/grkorfcpv.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gztxfywnl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gwjdqgreu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gefmavdeh.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gknnnvtck.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gtaxncypb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/ghwbtynuj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/glkrxferr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gmjxqwzba.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gdkngxaby.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gvpzbjsbe.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gitfumbiy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gerywttok.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gyljdpkms.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gaahzikbo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gplbaploy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gjkwjxexh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/grllfvcev.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqjvtvwla.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gpzaojfra.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/ggdgnqxsu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/guirzphpo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gltbdqndz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gpvzzlahj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gtdibsvdl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gpckhrqgl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gwscyhwqx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/ggbcihgru.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gupizpxkk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gbwokwotu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gablzalgp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gzqwbufee.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/ggmawigbg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gnxslcdkc.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gspctdlab.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gpcqawseh.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gnbviqtba.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gpfftflhl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gavddkvop.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtojhmheb.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gtcgheetp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggjxgqvff.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/ghuznlome.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedqtbwqp.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/glppwgzdo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gxetyjsxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/grdxlyppy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxsjvjtpr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/ghoyybvxc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gyxmbrkpe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gxmuoknyl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/glzknrtyq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gztmwmfoi.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/guzmyesaj.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gupdcnqnf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gzkftnkiu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gkwpofcvc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gwlhgncii.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gqmiqptft.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gdloqitfn.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gdsqxsyly.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gayhowddu.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gkgpfrkyo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gwaivkcwc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtboykzwz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gpnkzbpod.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gixbqrvxr.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gpxqqryyo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/grgfeemqx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gjofptujx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/ghrcupcsq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ggigyianl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gibubfifc.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gcnpzkpdq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gtzcdbhrv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gzlogtroq.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqtyyzovc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/groybvgxa.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gcgyyyvez.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gimvfrkst.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gacwmqqgn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gsiktobdl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gfxbkwcta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gstdhqqnv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/ghcbdowly.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gehtpxomd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gelduzewh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gikngnyko.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gtavpvmdd.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/ggcusjcfi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gnuzhwcne.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gyfeebcka.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdrhywkyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grqydzxhv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gklndrrsa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gibeingjh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gurdvmvcr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/glfoshvcc.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/ghayyavmi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gpjuunslg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gyzwxkjai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gckufozoh.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gqyzffwgl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/glysibiyr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkoznths.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gypzjpkrc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gvumswsbx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gnchdzbbt.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gtzdygxvy.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/glrfvbndz.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gderrhxtj.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gkjhpwobg.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/glwsmlrgf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/guvoldepf.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/giduzstfd.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/ggxjmpvqq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/ggdnucfyj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/guxxipnjq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwtepjuph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gcgmlbyki.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjlgcyvun.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghkkqcatl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gqzskbfoh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gtonuewhw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gwpuiydht.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gujndsmdg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjbiompqg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gndktxwlb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdxuakleo.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gityydcdf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/grsbrbiug.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwmuupbzo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gcfskfugw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gsdxsoxzp.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgxzeyk.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gignznhyx.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gdxrqbfqh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/garedeeap.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gnsgxcmqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gtalfaoyv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gbnpstisc.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/giivxswsm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gnvirywni.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gqshhwekp.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gciaabbiw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gvomafaif.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gzigantmr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gyfjdnunk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/glengldif.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpitihlgj.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/geyqvrfvi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gmdkonfxu.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gezfbndbb.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gzzclyxjc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gcamvhdoh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gaqeqbcjf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpmpgnmsx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdpemlbft.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gtpzyyshm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gwzjawqzz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gobdlffsb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gleckhcts.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gnwkftjtl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gqbnvgkfm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/grcvabxfp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gfqivvyjj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gqigprrrr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gkpoixqqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gevmzqwwm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gdiukctgd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/glfixbmyy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gapftcozu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gpeyobhlb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/ghguijmev.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gqorxbvwd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gosmhhmiz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gpcnbifzh.sHtML


<!-- 参考信息 -->