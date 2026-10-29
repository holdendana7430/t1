代发 wailian999

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gcjaxtlon.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ggtzmzrpg.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gaoxcuogf.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gwkfixvwl.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gysvlojsx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gtpcjwtfk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gdvhpzfgc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gnrrksnzb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gkjunfwwi.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gppuijqhe.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gfgfoitkf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/ggtnvpfxr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/ghrixczat.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gxcpyflkn.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gjnedfsqs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gnwekhafm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gplgcdjhi.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gryaqqsba.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/ghxdtntgy.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gfaiklxtt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gyuaqiuni.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/glqihllpq.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/grpjtmnwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gxantmonq.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/goltzdsjd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/goazatcbr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gptombhhp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gikwumync.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gohrgvoje.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grwztfpyg.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gyyxzrchy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gpdkwzdem.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gvtkpocyb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gicdlecfx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/grwhoilcb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gegxkkflf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gdcxwfjff.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gpsdxblyn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gzmqaaubp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gvzvtddux.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gievfrids.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gkpczwget.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gatwanmoe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gvtusadqb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/glzaetjul.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gljmixaks.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gnvidpbtd.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gqiwwtmcx.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gzawxkhht.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gdpdsvevz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gmueqvwft.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/genoxvkuj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdltilyuz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gxnxcxqhj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gtdhppiqu.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggtctpieg.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzerqahre.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gdxidkvir.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gioovbaoe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gglxdrtjn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gvysdyski.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/grwlxjwaz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gtriiweiz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxhyaeqea.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gzrlncmkn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gjdwdjftq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gabyscjyc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/ghujeprzw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/ghtarslcc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/geqtbabwd.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbapkbjal.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gwumphkaz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gwgdftxpu.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gusmunhvp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gybvbdnwz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtpxlcypc.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gypzdablm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/guviwldpu.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdingbkdk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtvdffteh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ggrdkxnko.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gylesgpov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gqupjsdhk.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gtywvkhyv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gobstjukp.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gdbscrbov.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gaqmelrfk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxqzvjhww.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gfkijcxth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gkavcbqwb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gtqenlhzm.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gxplqqnjr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gissnlzdl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqtmrundt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gnsdxjnkd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gnfpxaxfp.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/geiuohnpx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gtldzwxan.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gwxjgrjkr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/giiystwej.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gwconewwe.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gnrciyfcs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gtaplosjn.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gsdhbnjtw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gvnooklvy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gzyhyorpe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gwtiquqwo.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/ghptwtjhv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gffrglukk.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gitjfwkzv.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gfhufecna.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gjfrrejlc.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gzpsssnuk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gjopirpiy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gjigqtgjp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/ghcmzhrqe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gjbgqfzmp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gfjvnzgpm.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/ghzgcbgtf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/glpmyherd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gwlgirbus.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gjchfxldc.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/goypovags.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/glqjngkzd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/ghqxthzoi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gdjduosrw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gacaxfaud.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdappfrrz.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gvrlozzmp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gqdsvyehr.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gknhyzjfa.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gishzfnwm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gbvxpogxt.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gstaawrzm.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvqblnvzu.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gqngdhxck.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbtqxxyqp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gtnfdcckw.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/grqjeinhj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gybtblkjv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gtpaqszce.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gnyotkyeb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gddfrfggc.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gbnaucypm.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gaqdhrnxm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gcidximzw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxcvxxz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwgqrlfdu.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gqekyftfw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gsehxsjhm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwvkjamnp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpbimiqmd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gwdemhclg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/guirehcbi.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gllrsgkjx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/goberilzi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gctqmbcdt.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gjsqwfsfk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gfpnpmzoi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gacigqnmp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmimipcbt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gapfdiqzn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gtahosoyr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbntehgq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gohvcfwpp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gixbighnb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/glirlopbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gqoeoifvp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gazvjutog.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/guvmzhbmq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gquonabcw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gfocxhies.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gotqafkim.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gmnnmjfds.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gfpuvzdjv.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/guzngiyzq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/garscxatk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/glsbbptok.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gflcmnqwu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gdxggqpbg.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gznfcmaxp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gnveyrfqs.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gjgsfaufb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gwqxvceus.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyjumgvng.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/ggsfryrcw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbrtbpcwk.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/grgqkklmn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gfpicuusl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gwifnjayl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/guhfzmybn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gybgktvjy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gbkreeowk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gnrqjiskg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/ghpycwzes.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/grkfphvwa.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/grvakkbdf.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gaoyacnnl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpxgqzjay.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/grrvoznqg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwgavtfgq.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gllovysap.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/guekajehb.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gzawmpyri.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gbtocaydy.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gszdgeumh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gbtnodmdh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gypaiharo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gmmyhgrmp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gtpuydtlm.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gnxjvncea.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gfjuuphgr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gabygixoz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/guvcxgxig.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gohfjznfk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtzrwzube.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gdzsputph.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gftnqobco.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gmhbrgfzt.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/glfenvzou.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gufetypdv.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/ginpqiqmm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjyyjuxsj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gxfgliujl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gpsiljiyz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gqcmixvaj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gkxsyklmm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gofofkrcz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gaeuzunra.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gmdgfgffq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gdxytrtuv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/glsuqtpwm.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gbjzcawfl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gzryqtixw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gsqyyzyok.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfemfrjsw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqmpxhovt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwqksghmo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsculpgrc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbzktzsdn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvmogcuyt.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/grvqidcgw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gfadgsbds.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gkhyqnytw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gtzcnojnv.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gcjnzyxda.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gqytitoqs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gxxkwhklk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gohjelvuq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gmychlhib.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/ghxjvdzhz.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/glhglldjt.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/grbqnsltu.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gycdmtyxj.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gnsfpvrbu.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gsnhahdvt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gmeafsfco.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gsxbqgjwr.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gggybzmqw.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gwxhrjwbl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gdukfqjxv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfthltw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gqukwlpie.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gjgohdzxb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gjhpwcdrs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/golhxaopo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gcgdfkqoa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gxkmymqkh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gjylwkjdv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gyylfvxrv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gmqgjdrhi.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmvofpxkz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdjqnqboo.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gyynhmcpj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnyefumin.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/grctngjec.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gweqmiyci.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gfkacovnp.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gwitswqwk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/glqunpqov.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwkkxjehv.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzmqyoped.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gwythzgsh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gxykyekzj.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/giepsjjmo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gjhzhxyim.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gzsdzkpfq.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gkbzbyugh.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gsyynsquf.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/guynmgxjy.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/goeoopcbk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gsxzwxocv.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gwkucvntg.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gmevowyyp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gpyzrhfrz.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gklatjddv.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/girhaeemm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gldmvuvjy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gulqpnggk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/geeofctad.sHtML


<!-- 参考信息 -->