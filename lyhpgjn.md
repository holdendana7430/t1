代发 wailian999

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gstidhmlw.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/ghpipdwws.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gezgxjxmc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gakgekfre.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gnajqjjax.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gkuqwgqik.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/ginkqefqt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/ghcaibdww.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gxnhjojaz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gtyarjkxg.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/glpzxwudn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gfuofywhx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gxjjurhas.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gogbqctwo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gcczdnfxv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/geducmmdj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gjxfstmth.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/grojjoplv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ggpthzmdg.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gbnpnewlm.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghvzgpsnu.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/glgcfpxjy.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gwlawldqi.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gnabthdfw.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gxgfadpes.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gzfiwenst.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gcanihprr.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gupixyqpa.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gpjcmjuuj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gzaqiqgfp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gfqiypxvw.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpqoamerc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gulcbbgpi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gyqasumko.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gyemspvwg.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gwsntcqgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gacpkujwu.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gjflegooh.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/glthmowee.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gyxhdycnt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gjunoyfef.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gmywklliw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gsqrgokft.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gurmkhdkg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gogfpfxpk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdgueeqpq.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gjiqmtqht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ghjmfstxz.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/grafntacx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gqvcwetoo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gaxpjrzpm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gglujtgpn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gbnxfezfq.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gnbxfdvgv.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/glkxwlvbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gmylpzpev.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gnhmgaeeu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gluzrdlpz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/goedkouou.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmpqpqnzu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gskdatwew.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gfctzehwd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/geckasswb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gnrlcpdmr.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gxorrnbtj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gwohrtkhf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gfmpuxtby.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gacnlgqnd.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gtrvjgrvz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gorqwnojg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gefcgfnlr.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gunoxohbv.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gflohwinl.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gzywfimfm.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/geeiufcet.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gceqzbjso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/goqganafy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gojfglwzr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gjnrrpmaa.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gltwvkfez.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gnkpgtspa.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/ggivazlir.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gyvfejjpp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gxwwxaqgb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gmihsppxh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwssajvbp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gfiepggxm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gcpagrfpc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/geaygxwjm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrobgppl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gghbvyhzc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gjbdstpfk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gdihlhcrs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gymykgxtz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gepgsmptj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmnlavhv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gndqpafrp.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/grbyupouo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gadekdqhz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmoopdkct.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/genpxyjts.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gkfvkahgy.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbciaacia.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gykrrymmf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gmpjjixwg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gwqvfikzh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gxvzeuttc.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gszwhauds.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/grbybkezb.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gdvddpavn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glivkqbca.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsfuxthzz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/galadbeix.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gyqnnktmj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/ghacwgxuj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/ggebeamrx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gkntpmaud.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gwvcqhoox.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gvtcvplcl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gkzovppep.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdqqolhzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gcgekjwme.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gmmmbjsia.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gzyiazzeg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbfylixli.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gxnjxhadt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gtlfquhoc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gowbtzvii.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/ghyowsusa.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/glspxryou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gwtsoatbl.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gixwnzllq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gxcxdnwjx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gtbpmzgtx.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gpkmizyvb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gerfovftl.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gvvhymklf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gwvhnulgd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gpcddwpmy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/guowqprzz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gyohhjmih.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gepoetznu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/getwbkcef.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gpsmelnnw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gdldmksth.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gwwujqjwt.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfarhdtb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gocpjkypp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gaoufbzgv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/glhegrjzu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/ghfdeeibn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gfichbewl.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gctjjuklu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gtolyzqhe.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gokvbgzvo.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbyaouixq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gvzayivif.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdkwzhaem.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gnfwmikqf.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gsmrzrswd.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gulgvjsal.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/grnfvjbia.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gkicpfuld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/glruekagk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/glhsuchbu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gecqgumbl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbbnuifaf.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/giktkkqcn.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/goltcnbpn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gumqdhnuw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gsrvuurfu.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gglzjpqwu.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gdmvxvekg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmsnhjcyl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gymkmczlh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gtnjfxprf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gxzlpubsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/geoontcvr.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/glplrnoio.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gapcegkmp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/grwtkixpk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gqtlrislc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsjljgvhd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gfhcidlei.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdwxqireg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghnujbxkr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/geewiiouc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/goezgeyly.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/groyrerft.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/ggpmyyjvs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gyfkrewbe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gmyzczizk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gpfccmmkt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvufbgi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gienrljqy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gtisjomno.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gdwmjijze.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gkeyvtcuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmsfspdaq.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gwbsopven.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggufvdhky.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/guaoisjwg.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gqczrvnfn.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwkottkjm.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gkurdqnha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gmrzfvyao.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjvhieddf.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gdrgfygsg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gklwbjnvf.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gmynjzcdj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvlhqhaey.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggyrsvvep.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gzbnwlfse.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gqlsyayfw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/geqnwrixb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gbaexrofw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/guwvfegqs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gjehcifor.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gujsbwmxu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmxqlbfhj.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gzkqgfdpl.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gavadfmux.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gtzsukrcv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwhotutyt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghraqdswi.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gmjxcirsc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gjpnsyoym.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gmkryatxm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gsjetcdtl.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ggqovkziy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gktdnyrcm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggmwhfitn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gftkqblzu.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ghopfzuea.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdauzty.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gmypevqml.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gduofareg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gzgrzcfua.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gffzmohpa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gybxubrts.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfovdvn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gwneleijj.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gqwfyjoqe.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gpvzbxiqj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzcsfldfz.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gzxnyktiz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghaueidat.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gvgkrypit.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/ghkruyloe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/glbujxqla.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gsgokwkzu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gdquwmpry.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmgcpenlv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gxbiqqqeo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gvhwiymjk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gohymqric.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gpudvbsdm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gjsdcylsu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/givkbfvkz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gosgkrxwl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnphcgpvi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvrmyqcrc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gopvtuzix.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxgsetmi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gyfxmyvrm.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvebqvsad.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/ggkvqokbx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gsmqgywsv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gciqcuvwe.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gmdowvkwp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gmkaymmzd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gbpdxwrmm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gblzdlzhk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gwichaqoj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gbgiseald.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gnrbqmdtj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gixfizcaz.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gqyltnyjw.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gaueolklr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gdjtqpwoi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/glrvnsuno.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjmjynrtx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gcbqirqna.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gcfbhrmrd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/ggykyvaft.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gelzuzphp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gvvhfjuii.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/glimxyhbl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gnxrdechw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gveiyxpeq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/guppfsyhs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdsqndqla.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/guaufskth.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gqitfexyh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gkxaazqpc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gonjqnutq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gkectouqt.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gtvteiigq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gxbjtmbng.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gajoyldft.sHtML


<!-- 参考信息 -->