代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gmubwjlsd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gnbkyiozi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gyiujdlms.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gccfrumix.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdofwozxz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghrbihzal.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gasklyfms.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gguelmytl.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gqfomuowx.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gdgzinbsc.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/guojynyil.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gzrcqqxwu.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gepzbdpaz.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gkhzizqef.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gcablmkgn.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gzydejevg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gvvhuxpyy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gccrmgtww.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gobejmenb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/grdlqvwqe.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gvcablqop.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gcuhtlrao.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gwqumfgcr.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gnvkvxfpc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gwjsryddl.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/grantwlze.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gdpkigstx.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gypgpsqav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/ggoifmfsv.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gjowzefyu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gaagkvvfs.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gqzpvdzdk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtawscjyv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gflrkwqud.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gdlpuqriq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gjbzpwrlb.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gnunfwfvo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/grkdppbvh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gtgyaycjs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gbouqfadc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gngeopupy.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsbypozcn.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gbbyapmsb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/ggowiitvy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/guzvkmjml.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gvdxqneww.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gfvktgene.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gjxgadzhh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gkjlnvotg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gwmnrqjju.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gavzgbvnh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gwqivusrm.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/goocdqcdw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gmykjtshd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/galvodyiy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/glszmpqqg.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gubmsfine.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/ghpqrpfsw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gxjllutnb.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gxnqudsld.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gjapxxkic.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gchlqsncn.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gunczhcpd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjsouvrll.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gcsqzmllq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gmbechwwh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gmwjxbpfc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfuccvtry.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gogivvmqm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gfyqbitsv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gckmusefw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ghzyzgenu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsoiivuaq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gqokfczqa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gtybpsfua.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/ggglcqxxd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gevwkkfvd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gfcjxlxoj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnjsxwybv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gfincrfhz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gulhhwvqh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbnffevfb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gelzcfase.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/glzlzpxjv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gaaypfdip.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gkciuzgmv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gafuingeh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/grsfavznx.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gavlkedos.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/geekfogky.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjkqkirfy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gzdtdsybd.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gszgmrjxl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gcwqnerhs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gwxdghbua.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gujcjmmhr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfxvcrion.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gnyxeucur.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gtvjugnjg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyzbbhayo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gmrvdipcw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gqiuokcqm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/grrxbrvgb.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gglwhhela.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gqcloohst.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gttrgakjv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gfovxgrlj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/giasaayqt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gpwowyzxb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gpsfyzeud.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gpyvpfmeb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gyvkgufql.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpfiqzjmr.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gzicfeadc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gjdorgkjd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gvsswmmrn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gmurttgbh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gozqvzfqn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gzyugyhot.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/ggrqdlbdt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/guwwfmsvo.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/geqlxrbfv.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gifuyhwgv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glxrqrfne.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gdedscrgk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gqisrvenb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gpwnsnjrg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/guxqnwkhn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gocspkvqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gduilxrfj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gdkcvuuhx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/ggxeufrgu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gvubvifiq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gnmduusgx.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gtgsotqpq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghfjtrbqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gqapjrbyv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtksrdkjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gpnwgzmot.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gtpwldzhp.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gktdttjcw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gkmrhbctq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gbdvduooo.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/grqdrrdou.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gcqjfuwdz.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gplimaulx.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gmoyzwfft.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gsgkshhgp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/geoyvkdcc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gncqxvlpq.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/grxntffze.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gqgkgpvbn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gowcmccge.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxnngyj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghohxazqr.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/grtbapthe.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/ghgyscvco.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gnrgpbxgi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gauoofwru.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gqfrwkrzg.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gkuxmfvuq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggdibywix.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghkdkcemz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gibknmolc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxnqwwp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/giqicaddj.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/guzlxykwm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gamwuytut.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gpwbabjpi.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gvmovzbzp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gfmvwttuh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gpjdxpany.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gnvqbzbxa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gztxxhrmy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnagptgm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/guishkcjz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/ghjynejbm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/ggyivcwoe.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gekofqcuf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gpvknckhw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/ghvqhcanv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gdairohqd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gdcwqelze.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gdlnlkihn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gdmvtzbjt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gutqthbac.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gpnymspgg.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gxhqlyuqx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gbzwzwloj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/grzjocyzm.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gjqsnvsgb.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gsuqlyens.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gylivscfp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gltqoncdo.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gpccvvmkm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gkrgwhndz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjpzxpknl.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gpwwzvddp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxzdgdbm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqbasligw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gobgqzchm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gukqzusil.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gzmnavhib.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gjltorgco.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gbeemdsts.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/griezqnlg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gonfjpicz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvebnonts.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gietxuscg.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/ghzppzepy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrbghsk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzgxsithv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfykmrsjh.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gadxmiivg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/grvnamlit.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gmweqzznc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/giafikwmp.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvkfeyuyf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gbiakbalo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjpevhsik.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gflzufgfp.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gavhltdak.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcaujkkhq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gslfjpblp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/giywpthuz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gxahbfoty.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/geyynjdei.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gmswtbces.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gfqwmvhdy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gophmgfwy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/grlomesxp.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grplabzfr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gtsmygozb.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/ggoczhgxw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gjdullqkv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gywcfhtrw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gwfflbthq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gksdvuixo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/geofgmqdk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/glirtmbhc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbnliqiaa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gtqseykgn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/giosvtgfd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gpcjfqjxd.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gwvhfxklt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gntcitprl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gpbawuxlk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghdwwcwjq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggboychfy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggrrughwh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grccmpihc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdvqcsamq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjyirmthr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gnbcuaqif.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gzjisnefk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsstzsy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gvuaxfecj.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfexgrfh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gxqzlrvex.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/grbhccrrm.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gfhkfmbsp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gtgzzsmds.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gucseojln.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/goamoljed.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gyxouyabe.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvacsxsho.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gagyhtqnz.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gcmlvtwfi.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gcgmjydmi.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gljwtsfcq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gohhwlrsp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gdgkflcfn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gjdfgbisx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gqbobwers.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gzqkvbqdx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwevjka.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gxsuexnog.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gsxyftmoo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gybhzpoll.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gnlymiklb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/ggvlrovst.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghmciiqvf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/grqtpgsrc.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gentdmtbf.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gsfczaebw.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ghtevixzo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gkcngeymu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gopuxwseb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/glrelvvfq.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gwzjumdun.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gebaqhqrx.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxincmuvv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gihhbdjah.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghlqaxvkb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gqmwymnhm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gyscfftyu.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gtytnlvak.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggiavswtc.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/geqzmtllg.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfclpefdr.sHtML


<!-- 参考信息 -->