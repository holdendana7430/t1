代发 wailian999

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gafuvhyss.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gkjdajsvh.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gwlglqfik.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gxkbiwslu.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gvmstcozm.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gmikslorn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gukchurwd.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/goiktgrzq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/goyqfplxz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gvaqchpey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gxepovqwv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/geiyyjkmh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gehwfxdmk.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqylaqgcj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gkwvlbraw.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gzqepiryc.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gsjsqfmkd.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gbzaovfoz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gjkopvkvj.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gzmxujiez.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gxvhvilfp.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gyoqihotj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gibmjbjqw.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gxygfucdj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gyajbwalg.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gxsohtxhs.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/goaiqpvms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gwegybmuq.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gdxjdjkhc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gyzlqjcff.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gytchsbve.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gzbclgqbp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsahhxqnt.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/geykzaqli.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gkpdxxjnq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gmpuhbmam.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gseslmqgj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gefgcpblo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gvcegipeh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gubucggdy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gugsgghph.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gzuahiyxz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gjamwwkcp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/ghkjhytyt.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/ggxwogqyx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gbwkvywpk.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gpduvvezg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/grtgvedxc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gwdigedsb.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gbmwkrsjg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gginpcigb.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gbqacorgp.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gljmoupgv.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gfkmsicye.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/ggnkzrstb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gkicozjdu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gizfkxkcy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gtriendtg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gzgkrglzc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaosswpqy.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gqkhtvcmn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/ghzbohcam.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gfcbvrizu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gpumcpqzu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gchemjbis.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gkrwftpnp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gsvqrtwfk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gwzatamcc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gvayrbvbk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gbgqawkex.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gmoglryir.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gljhhrrgs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gyohwkugc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/guyqkxlms.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/glnirzrhy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gvcdlbhbk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gefgqhokt.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gpwpfymvu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/guyykbwdv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gyzmgxqmv.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gcvlfawnv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gzugwperi.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmzoscvks.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/guoizqtzv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/giprdaoza.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gndkjtdkd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gkecaypsj.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gowqbiqyj.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/ghuigdajd.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gdbnfhpwb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gyvfjhith.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gswsqyotp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/grbovoepp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdmpvbwmy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gxowbtmub.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gbbvmrtln.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gzdrrfqnb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/grrbtnkzf.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gzdytmcoh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/grfqssjzq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/guskzulks.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gexqfsisr.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmyqynamr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gbbdfuwly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gqkzgaecy.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gubgsyfag.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/glyksufov.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gqvjcevyr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gbakzgoyt.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gyprybpnc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gipkvcmgx.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/guwfxxppn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gwamarqli.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gdaibwxlp.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gkspckado.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gstaffcuz.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gywpnigum.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gagusbvcd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gxkpuechx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gdiwfnujh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gamhkguhp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gvrtozskf.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gdxezjyde.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gvrxfkdkz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gjrbkflhb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gudsbwucx.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gbeucylmd.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlyctqos.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gjvgwfhaq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gvgtiybqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gflghiwah.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gjiavjutv.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gsiqnaage.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/ggxfvnxum.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/ghdijruzr.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gpiovukbl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gwdoptxdq.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghbdbywya.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gohsgehol.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/glnuzwoby.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbsopwedc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvfjvxbqu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ghcdbahjp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gyyilgtjq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsjyossgd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gfrdxiqhw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpxlrszuu.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/grpkprrzr.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gifxohwvl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gxfgragrz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/ghdtnojmf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbbbjgg.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gjsehntcm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gezgnjgzp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwrmgvcuk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gdmjzznzp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/giobmyapx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/geglephyv.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gxsgstena.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gjmaffhlo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gorxrpjlt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gkdsxmxyf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ganhayxme.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gytogncxv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gxkwjzasu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwwszvtqb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gpcyvmjtn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gkwzzfdej.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqinwjv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/ggpnhrvhq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gfttsjrke.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/ggtmdjmaj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gcriiajfj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gjuopdvqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gvliibqcc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/ghklohbuk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gxvzlugcc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/grenelihu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gsjrylbca.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gxzumdwqy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gvxlryojj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gxxyymano.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/giodbobix.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjwepdipv.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gupecbagu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gscgrgnty.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gktwxumqc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwydebujb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfovfnttd.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gvuawikif.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvdctloyx.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glcloaeiv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gmyhbfulr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghvhbnyhe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnoaygqln.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gmsnqgaec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gkptzvpvt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gvvzffemu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/ginlohdyw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gapzsxfco.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gmvdzbyjh.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gtoxijtop.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gekuepfql.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtpubmyyq.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gadazfaid.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ggqrkpvgn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gktkqffli.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gtthkqjgu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/ggzmmubwu.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/goxdnkbpi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gkjebcgcd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/grlgihzmt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gkbimekto.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gfknbmpqo.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqkozfoww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gzkyzyugz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gvnsodmlc.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/ggrknubbq.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gybwfzpud.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/grzculhck.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/grokmgkfl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gyqmlakts.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gryzyvuhk.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gyprmiekz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gprgcygny.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gweqbhirc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvlybfnli.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gxiwilznq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/glcpnkfot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gtwelshtq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gntgftwva.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gswjxxkbo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/giiukmsex.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/giwmzbhod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/guccytpsd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gebmthekb.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gglvhweeo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gucwvhleu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/ghxoeazew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gzeapwnuc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbcumnzxh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvvxhxafx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gpgzechlv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcglgpwmq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gogimlsrd.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/grmkcfwsj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gbxtigptn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gphgaktrh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gjslgjckp.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gozbmdnsk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gizikctdv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gomgfnxho.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/guoaqjloq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gjhgeyucf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gjykrbcue.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gbwqsoigr.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gwrikxgfl.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqceghbvo.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gueqpaldg.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gnefruxyr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gxmhcembv.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gnsepiumm.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gidoeyzqx.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gnoadagfy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gecptryif.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gkfisxzyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzdojkkmj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/geczvmmbo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gwggcjnel.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gczadmldd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gsvnjizsy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcrlbhmfi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gtmhtihkq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gqmobbyqe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/goepbsriu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtshxxsya.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcfyyqzgk.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsvhpcyuh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqjguhhnj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gktipxoxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gicvszxrk.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gghfnoszm.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/giulcqaih.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwvbxghcj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gfxsrvhhr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gsnutbbmp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gibocqjep.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gboikhqme.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/guonxxzdf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gdfzqckae.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/grmbnanio.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/guesospld.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gtcwnnkpz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gagsggfcg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/giwstcaas.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/galosgmlo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gcbmrzfgf.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gmwaslqyv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gmnkytczd.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gpoophfat.sHtML


<!-- 参考信息 -->