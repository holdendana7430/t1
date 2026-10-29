代发 wailian999

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gvbfigevd.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gfusxclyl.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gezjnfjvh.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/goxqsflwd.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gxmevtazm.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjtabiagj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gmektwzjp.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gnhisvgkf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gnqbbohah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gbllkakiz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxjlletdd.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gkbymafza.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gsbeyjvku.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gxrqiktho.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gnzuduccg.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gsstfrzog.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gndhkpdzu.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/ggyqaluyd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gvsbaltjl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gdetfypdu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gefhjnule.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzfvahj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gwxvvphyj.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gfhuhlarz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmmkhuryv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/godxuhmaw.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/govyiqloh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ggddbrwsg.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gfgzzamuu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/grpcwdply.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gjesdzlzj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gljsrwuoe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/giwajszcg.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gfxipkciv.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gdwibsgbt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gggxjbaff.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gtnaoehky.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/ghwujqjax.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjraifadq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghnraberl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gmwbjkcwi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghjxnznop.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gonmakypc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gvgkidgtx.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gkejsgqll.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gdjybbzki.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glvcxiakl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gxscaagma.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gdgjtwpxi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gnjnhqvuj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gtbwvqups.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/guitaiclg.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gvwkbqjur.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gxrtzintj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gsufkcsvy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gfmhauizh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gvqfnbfmt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnwbrupqk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gomiccqwp.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjuwbgyle.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gefqkahia.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gciodbijg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gemeevros.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gegmcafwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/glnvrscpo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/grizjzean.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gejvsgrnn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/glxnzcocu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gejuqsazl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/ghijehtpd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzshdvuxt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gheqpzesz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gdmzbnyen.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gyrscudhb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gsrfbcmaa.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggugtuoti.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gfchifaeo.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gfiziokxt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcayefu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gewjfajzw.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gggevurjf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gflamavye.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gistkqvul.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gjzcafcmf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxsgpmffp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gjswmsith.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gdpnvwbae.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gdmsuoehk.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gmdpoonas.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gskqzwznk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gzmeacmki.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkfsxfb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ghoqezymb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gkeupopro.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gowfuujfj.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gpijnqnqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gazptygyn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gqhcwvulp.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/glkkxvnlc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gczknjmml.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gvefuclpw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/garqzsonr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gisylzpde.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/geciikupy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gpollhrwn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gbhxpmclg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/guddtzaxq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gdzbddyni.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gvnpoclvq.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gxliuwhtl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gkvpcyhgq.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/ggkvhlclm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gmcldxprv.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gnnhcuxng.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gbqzqafcm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gljnzrxse.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gelyyisda.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gabsfkrja.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gpsdfmcon.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gdnoekzca.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gwotlvdhb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gfemmmkoz.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gbchrahpd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/ggmeodiim.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gqrlkgtju.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gkbezhjml.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gdjvsduuy.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/grevokfju.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/grmdfvhzr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ghlgjojli.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gxxrguuie.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gxzkhkhvl.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gyxbmnmfo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gqqryjwkw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gcxkzealk.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gjebcxuzy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gevejxkjd.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ghqatwmoz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjwpmukgu.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/goowgbfhi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpotuzavc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gwfklguct.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gypztbkbx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gyvowzuhc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grgiunlld.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gdovoiqhh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gmmujjuym.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gvtdcumns.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gkdtchvuz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/ganccxcrg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/grhtcycvd.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gnepwfzdj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gnxmjhqzj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gozebpuco.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gkkzyfkvz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gwzzdnaqn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gtnohrjmc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvhprbzj.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gillqnjmp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gtaqopvqf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gnqymmjgy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbyvios.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gsqvquojh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gczkyhimj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/glktbjope.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gyfyuiltk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gcvsotihi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/ghuwihiot.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gxfdequay.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gxnnswtoa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gflgnzyxq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/geocilgom.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gflrabjjo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gnynlzlzn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gvoavfzlg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gjxvgclll.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gkjnljejp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/givuzrsot.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gurymjxkr.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/grxfpltng.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gkkvimggb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gtutfwlep.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/ggjhngmub.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcqgfjvvh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gkadhjfjz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/ghkdgwpgl.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gkvoijzyz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gfzckqkzd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsnxstmxp.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gvfepcmmt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsysrqggk.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjgpmvszp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gteikmdab.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gmgviinpk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gtnxiqprd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gwhkkyjoi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gzcwfzfte.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gxoiehcdy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gkaajllyo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmrkdzwhm.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyvzamdvz.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gogealnsl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gudtgzvzq.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gpltdvlio.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gokjrnoqp.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gkadkjpsq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gtbwffjib.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gycamjnto.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gvloxqgdm.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gtogrpjir.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gikevanlj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ghozqrkag.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gunscytpe.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gfvxogohe.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gbesitjec.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gklgbosum.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtycadcpm.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gmnvesimc.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gwzlognos.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gyjkjvhqi.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gbdfjhmwi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gaswmgtwk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gidcgripm.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gfmeezkep.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gpefmolow.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/ganbwgmyw.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gtpobcywo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gnkonrdgk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gdyalmrwb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/ghfazpeor.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyuivesjq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gsaakvpli.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/grgjnyaen.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gzadxomwz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gnaxfrrdz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gpygdrblp.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gsxnmbwuu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gbyrwthhh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/grmjdtwte.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjhoitusk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmnryqemr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gssggjrew.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gogxwcszf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxdtugsxa.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gsavzjvbx.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gtpshkfse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gkvekttyy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glvhaozmk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gqvsbekii.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gkozjrszj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/geiojqkeh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gqzlishbh.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gufatdokn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gjztwqoef.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/giyflifbh.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gmhonczgg.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gaxgyxiqg.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqxylzlbq.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gtloxinag.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gwrwjqpwl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ghvxkpiao.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gwsgpagjd.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gzwvagprh.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gbfgxznqm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gooyhqatb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/glkvhjwsu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/guygarebg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/geveiuyel.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gthcyzqtp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gpfpjvrdh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gibzxsmin.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gliagjbzc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gnnezctdi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjghzsfyc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gvourstov.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gutnpsrfg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpkuvqxjq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ggxhftdhm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ghbffldsy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gageypdvp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gljwxpcya.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gsqarpozh.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/guyevtpff.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ggkynowam.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gcreametm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gzactolto.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/glygpmqns.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghicsvcdk.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxuwsyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gkxenoazj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gebrmpejl.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gnysdfwer.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gchnhqaaq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gldhbhdhw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/ggnlaqosp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gaqudkdau.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/ggwfwcvta.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/grnababve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gxpkaaipt.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gbxahrrmm.sHtML


<!-- 参考信息 -->