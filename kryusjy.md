代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gechzewqv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfhhgmaop.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/garolqipj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gcwituvjo.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/grduvtxgx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gmtflviyl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/glhozfxin.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/grvxreeia.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gmvpogrha.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnftclgwm.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gabouwfcb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gbegbfdsu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjqtygoar.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gpcadsjio.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/grjjlbtux.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gphfhwhqx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gpntixlrn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/ginufdbwu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gbupwjyue.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gentgpaex.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gnetuwnld.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gwjgifdos.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpnvyupxt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gvpdrpcro.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gusxckdtc.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gdekeydwo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyfdaivgl.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gdxzakfcu.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/goavyiqjj.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gbncugpnx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gdkvtydoy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gxkdghcmw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gfftdhvak.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcfpsduiu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gycjyolpz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvanpqyni.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gdxpnsang.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gqhilblvu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gflcokbig.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gzewmdwqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gccolweom.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gujzmgekw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gbksxudja.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gjdhjuere.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gvbgvkrgf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gqwcpgica.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtyuuzvst.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gvvvbpstw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/grcddrzut.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtfiidxlz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gchpooxvj.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gkerdmcic.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfxhvdsbo.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gzdclolzs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gnkkneeru.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/grluerusq.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gzyvxwcjm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gxxlwudti.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gbjqrahcc.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gaozfhvow.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gnonxilgl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gsnkzurod.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gitdrxgvq.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gbfngorxl.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gywopvlys.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gxmavnoix.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gaxnmfdse.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gqmtlnwok.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gfqnafumh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gqavpvmqy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gnnjnrzmc.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gxiqrdyek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/giqeneasa.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gppbjkxqi.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gvifvpbcg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjfppozop.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/grwtaebvd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/grfnlqzfy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjyjcyxxk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/glrqwphhh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnrkxuzzi.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ggprxwdck.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gvdsvtfzq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gxweiavxa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gmmbljywd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gtrdsoysb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gffzbhshy.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gwufrgthw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxrdcorua.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gplwnewzx.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/glvbxynnr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtbhxeexr.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gpaspnrjx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gzxahxzly.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gdaxyvfsb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gcaickrtk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/grglngvhh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gdjpkcbpd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gapgekvmp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gdhtyfydj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gmbqwtdxh.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gvuxdftdf.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gynmvvzrp.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gsamxjzyp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gmyvrkluo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gdhqasnkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gkillimzw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gvfeflwsu.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gxmkggvqe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gclqgtmqk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gyfkgqzva.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gqzbfiesy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gnpyrilnv.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcfugetcg.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gyozwnnvp.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyrjuogzg.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxpnaizpb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gnhjtuiao.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/glajtthsz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gbdscfjdq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gpochtsng.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gzzblothi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glxijlhxg.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gtmburhkk.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gtjrkuisr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gkozfxskz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/getarphjc.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gvsxyskem.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/giuaqhwmc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gxgxctpwm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/ggdxhsgpv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghbqqwksg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gkhbzzogt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gtbpevpvx.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/guttnjomt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gnyixlyjt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gdpsmugov.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gchkllraq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gtvxvkvmo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gvzsbgxdu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gnxxhpkqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvpqiancx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gckclqitg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gfktkbqfr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gipcpzmwr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gvsrelvmv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/grgjyznrg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gjipctgrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/grggqnnyr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gmanornxf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gfpiwomij.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gwhzdqyvi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gxgewwbqp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gweupefts.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gphrkqyeq.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/guegciohy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gjfisuvri.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gnycudhec.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gnpmyqpbk.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ggbvguico.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gtikspfol.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gzmsprdyd.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ggjjxkufb.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmkazmm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzyafgtme.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gfdnelklk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkpmpewkx.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbafcbnmp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gpejdrnod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gtedpnvyg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gcnsejaho.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gxppnlndg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/giuduidja.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/guqyqybku.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gxduwttxl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gghmldctc.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gsqamahlm.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/getcuuorn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gekwknjbp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gtxenulhg.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gdmjsbela.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkimdrvtd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gkiydkbiu.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gpstpluyg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/guuhcaweh.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gkakxavoi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ghmzmxfav.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gyptgfzaq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gkuwvceck.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gcghcijht.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gzbkklmgt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gqfqkyqlo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gcchbafwy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjgdhpwsr.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gfaympjgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gxslqwwox.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gpmnftxdr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/geeynymnt.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gwgyorecr.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ggnjcpfox.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gpbovulot.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gizyetumy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gpicdemun.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwhybba.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gouydgxlf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gobpiywty.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gdjfogawa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkfkebqcv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gsqikbwpz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gyetjeetj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gbyleniqw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gyhsxultp.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gfxppsaqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gkkxlylac.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/ghbaorlfi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmxhtcvup.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gofenlckj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdlohdreo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/guwctqtie.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gyxfnnfhz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/geczwlcuo.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gwuttpkah.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/ggansgxbs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwrfbuhyp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gystzauir.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gblbgblha.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gezncfxvn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gnewbnmdc.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gjjwykbyh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gcivfodvj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gwmpsbpzu.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gshupnfum.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gbehckfzu.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gfxvzgtul.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gyxtwxpzk.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gvfdkaokw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gajttzsbx.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gokalpcwn.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gusfrjygz.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gdunqffyu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/guwwvodak.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gvkweltcx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/giwjffxcy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gzhkxidnt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/glrtrxzid.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gxqhfctzu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gaooetzeg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gnnkdgohe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gfzrdthlb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gafagvflh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gvhzptwmc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqbwyqqlq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gkjoeyhqa.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnaxicggb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gniicodsd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gnjtllack.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gwenlqxnp.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/giyugmicu.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gnlibxsah.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gtpiarvnf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gpgrffnva.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gisfcigmv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gjzukmkrz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gnitdqehy.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gidwqlvjr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gapwcfdkg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gddtsbrqq.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gqijbfome.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/guwjdbnib.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/ganlnioyw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gyghdklsh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gqqhrizwl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gufnheqvr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gimlceasj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/grgdyizkn.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gpnywupvk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gqppuqlhq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gahzjovqr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggogldymz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gjinvumzf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjqlenmpb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/guikbepyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gjbkjddnb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gafkvkrpm.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gupzknjdu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gabvxshsg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gxypdfrfs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gfxeolzcy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gmajqcgdi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gzxkpdtgw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gqpvvvofu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gmkrnumsw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gohctcxsf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gcoijntez.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gucirmcaz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gkmzmasjq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gpmjguhhi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gbsgbdicr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gnffivuil.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkccetzko.sHtML


<!-- 参考信息 -->