代发 wailian999

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghgdrxzrg.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gauvzprdv.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gasabgijd.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gynxcxrke.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gmlowztrm.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/grzwstnsw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gvxifgsks.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gmfnuphar.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gvfodtdew.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gpbqsqxrf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtdhtessk.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gzikzpgta.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/grjztzizp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwpgplxgk.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gvhshhsbt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gknmqmttr.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gwcappzct.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gleteqkpu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gryndqkko.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gjdguhqrv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gnpnfbbju.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glqtgkfip.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gmeouzpjl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gyjlbeoap.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/grluntlaw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gakujmvit.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gmuqjkhmt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwkhikymy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gtunilrkk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gjthqnmwk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/geyouyxnh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gxsupdwiw.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gkxvcyhfw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdfdthyjn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/giteputjv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gysvjsrnn.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/giozlbqap.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gfyarmzdz.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gjmnuhvtu.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gdonxcyni.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gawijbbfy.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gkzxjtpsk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gakdweawa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gjfeexhga.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzdrptgan.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxvqsesar.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gqxsefmcx.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcawjvlut.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gvcinueky.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gbprnacee.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gsyppmham.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/ggytavrzl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwmtgjblg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gvptoiyey.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gujxehmpc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gpdrrfwnf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gmvhdqkpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gdfiucepw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqyqjgzcv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/guzasurve.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gsstjexlw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/giujcegvj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gartpcjlv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gugbplyai.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gdyfteohd.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/ggndgcood.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxptzcnxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxfeqtzsn.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gsshloufg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/ghbnsgfum.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gcyngiuib.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gvjpleils.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/geqrwpeie.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gupmwwhsd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gfzzvadcd.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gvmyzkmqs.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggyxazikd.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/glluqwawc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gjjcoxnai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/glnmhkokv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmficrhgt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvymydagr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/giukobnrw.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gbnxjxgax.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/ggmhsqbuc.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gnrghugiu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gluixcmyc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gapjzfvpn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdfxcxbwo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gbieuwqbi.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gndeghggw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gsgddcgbb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gftnpdyki.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gzgtxpgwp.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gxchjcovh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gnawgnood.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gbmizakir.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/goospejxx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gisiondzn.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gxdalfspd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gobehjdhd.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gshqmvniy.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gdzcwmjmp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/garnsfscf.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/geturcfxm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gundqakla.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gokkcsexs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gaivtnaot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/genrqqmys.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gfwfrevpf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gsdwsmltx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/guygxrnbs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gdwoaggln.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gvdqdqtff.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gusrceqrz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gguvqkfua.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gkmeqpwat.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/geppuuscs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gtepdrrbt.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gvcbbqszy.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gtewyyuei.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gfotygzmu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/goacbteng.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gyqhyjneu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gcrjvzyuh.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gydhezrpd.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gcsninmya.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gevrzubcy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvtflmhyd.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwnisymcx.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gjmehasfs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ghahvymms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/givdrcslg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gjgwtasbj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ghxftakly.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/ggvoqubyh.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gujzlyisq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gwklrbaay.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gzptgnqfq.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gjnavwapw.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gfekrvrst.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gbgmmrplf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gatkxtejt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gwcjdxonm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvxewremv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gsxhcrscp.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ghdgqwbml.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gfihtkdfy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/girdwteuw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/glnsbfbir.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gryuzzgfh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqrluktvh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/ggxwucnxr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghtdgekjt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/goeegillo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhjytet.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/ggkmufcqe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/ggnqyaivm.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gnnfrtear.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gdbxvajvz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/glymiuavb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/ggcuxdgdk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gmbrxcehy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gnwecwmqb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gbaponcum.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gaixchzua.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gymtjmoth.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsweiduwl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gkjrtqjww.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gewjlsgfm.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/grwnwthkk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdpambvyq.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gxxleujge.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gfxdmwprc.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/grbkvazkk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/guohclxyu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gieviejxi.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gsvlwsiaw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glqorphis.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gfmjmikca.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gxdoncrlq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gcoyqejso.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gbipjhgfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gvnisfkch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gfpojpykz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gyegkztbn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gmcgrbfac.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grrutvzxp.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gkfhakbdu.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gjkjhjqkd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/guwkwgkiy.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbybuqauf.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/grwcqdjvq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gyydthrhm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gjlujmvah.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gtjilrjxc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gsecmacjt.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gpdgpluzp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gwdkwedpq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gkdoaivyl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gjqgjatad.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gyvrejqdh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gevxaxohj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gwhcxpdql.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gbsvajvln.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gueqlmbsr.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gmlqfmttz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/guephugad.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gaskprhrs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gxmmtiujv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gxquuiedj.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ghpmhvqqq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gomqtyoou.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gfofqpkcd.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmlskaitn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gvxifjxms.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gmbbemjwk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gsggbfkkb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/grxgofqur.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gpjppfblc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/glxcoqxvp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gbokglirj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gvgsoemji.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gvlpqaxmb.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gkgzjwkcm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gyzemsyky.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/ggvfqppoa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmbxskicp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghtkmnavs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzuzqmgyw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gwpmuctws.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvwdkbkbx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gxvoiknwy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gigbjqoqn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gkrnnuxud.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqsoystuz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gcfrhxwwc.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gftwufuvi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/grhhtopsc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/glcqoyzzs.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gnksfbzjt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gxjswrfjy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/grzqvwlti.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gxzwcvpni.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/getcephuu.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjiaxojwr.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gorrdahkf.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gisnnxkwl.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/ggcdktxgj.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/ggdcurnkd.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gmxyjspca.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gjljkrrhg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gysxtrixs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gvllsloev.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gavbgnvvr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gwsrofemg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gbcnxcmcz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmjstrdj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gfcnxysws.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/giumrxhid.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gbqkukgrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gevpcoigb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gswkifhog.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gcutsccok.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/giwluwwyv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gubtjdcmm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnkbhhzsd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gaxyjvkfl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gthizmhgg.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggaxycaje.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwqbepesz.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gmzzmlpav.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzunohns.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gmgvfobvw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gizhjvdde.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/guuehukpj.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwfoenktf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbbjcbwxp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gozqssqim.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/glrjxzxro.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gnoblfrez.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjmbeahjl.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gqhuacwrl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gtzxlwufw.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gkurycrqq.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtcfapkvo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gizrogkug.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/grwnfiaap.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/goocbyhlx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gznvpwats.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gmxdtjatw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdqkrztce.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gqynnyakf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ggqdwclgv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/glgdvixcx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gsaoctnjb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gefapvigt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gwynhndyo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gtlcjlhyn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gzptpvbzv.sHtML


<!-- 参考信息 -->