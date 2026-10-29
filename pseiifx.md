代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gjdqimurt.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gcrjjkquo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gkutpzqex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/guwvjqaqq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gflkmfxpw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gwrlassak.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/ghsqkuujk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/glxulqoxb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghosqyboe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gaeccasne.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gmjegyarj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gogoladnt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ggituqsoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdotdolft.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/goxcxadwz.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkvawzuml.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzhyfuywu.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyxhsnqbk.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gkwtkiecz.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gkdnupzuz.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gfhcnjsbf.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gaerpfnig.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gxxctxawr.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/grmixjahp.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/giaxlqbyc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gwozhjpsw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/glptuxzfo.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpexgqvmg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gcqalfuic.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gosqqktdr.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gqptnqplt.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gmltrciwc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gnntqfqff.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gkgppdkdl.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gmlxjqhaz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gaxdyegnm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gjozviysj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gahnkqhhy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gdkrtyzde.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gpffoccun.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gibudeszc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/glslpmhmg.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gveqazvyg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gfooqbiyd.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gucxbobnp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gsfktdwis.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/ghxqwbmsd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/guldqbhro.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gldmyxhgt.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/grwgfdedh.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gnlmiotvc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gtupsxucq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/giehslwur.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gusmawgha.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gjabcmxhk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gdpkoixnz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gasygllas.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gqcoeqrfy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gmfogbeww.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/ggtxheomm.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/ghuspgvta.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gabkxnqvz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gszrmwyto.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gahpcrnhu.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gggtemgrw.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gvmgqclif.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gcdtzevoo.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gccbbyljx.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grbqwkbvu.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gurhlkzsd.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gnuzbiddx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gjoevotkp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gnqghqeew.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gvoaoapkm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/grvwdxbkp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdatcebuj.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/ghvqzemjq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gmzhxlblq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/glazummkj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gxdzxhnlp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsxckmwwd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gujlfjugv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gbanwbedy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gimqmgsms.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gamphdhhf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/glpsgpton.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpgsainad.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gzoanlxlc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gvfarxmdn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzgklmcko.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/giuwupwry.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gzdmtkssb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghgofpsso.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gmtvyuklv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gnordflyq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gttthvehy.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gbnjgaizp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/ghbtayikr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gagogartx.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gvgytpbhx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/ghfvofeug.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gpkfkvztn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gnjxxwycs.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gfiqvgkwr.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/ggnsyfxjy.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gjxhwzcoi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghncwdqej.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gkuwwygmd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gqrzhgyno.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/giliimsmh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gzeppehxq.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gwmwihlkx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gcireosxu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gzeebhkpm.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gmenrifoz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gpijcjjyf.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gcolskjiq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gxeiavtnb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gtebolabh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gheiinlkc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkdaoaklw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/grdnjltba.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gzvpgviph.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/ghmthjyzh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gdtvyzphp.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gsxkchzwv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gelhiovua.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gfonbrdxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/glfgfpvap.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gjytgtcwt.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gxnzienby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyumhkttd.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/ggecjnpnn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gpvowrkul.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gmvsbjife.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gezexqbsm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gagbyamhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gurxadypv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gziwqeinl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gyqwirpyc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/glkjyjyvx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gtfkwuqzt.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gqwuawycu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtjiomfgy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gthncaspu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gourzovvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gfuzbddtz.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/goapzyfov.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gjdyyphxy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gijiurchx.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gnqfjqpay.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gsddgxjac.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gefsjznvw.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gsrwdrybq.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkoschjfq.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gxabpxoez.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxdvmydrp.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/giiileleb.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gcqzvxdga.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gyyhhhuhn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/grdonwnyr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjwftvrxj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gcxgqldgc.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gdtmbaoxc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gfoyzywyn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gnzgemtrs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gnwlqksym.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gupjpnbhm.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gzahigigk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gcuqwakgv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvgslhgbn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gxlohaatx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gyyjkxbif.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gmayisaku.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ghsowpwuv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gemogmnop.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gwzvivkoy.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/ggkidbfgt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gcbvuxnin.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gnpergsjr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gnvwernib.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdftkanir.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gxmvpsjjl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gxtmywjxm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gqouohwfp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gjwuxosiy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gphnspyui.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/geikmsnrf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gfmhonmmh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gotoiizns.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/ghxprpaoq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/goeufmqwd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gkhufcxrl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gpvxumrvw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghrxsavze.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gejxhjdez.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gvnzqsssu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbjgfaql.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghvdjcibt.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gtzrxnvhh.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ghgvvvbwh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ghcsaxkpl.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzygckulz.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcfnpuyz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzxrzrifw.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gsvgcwveg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/govbzakdo.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gmjciskoi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gwailhuyz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrkkfzwu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gvsgohlwf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ghclahmyj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gowtorsdv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/ghcijcvha.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gokbeqqfy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcxzbpnlk.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ggnenbijp.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gsixoifju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gofdeikxf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsxfvouua.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggfjeyoci.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/guivesclj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/guagqxyqx.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gmzvfxovz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/goeogtsaz.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gikfxwfpx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gyzfhetlf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gchtvhuex.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjflzdekh.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gijwfjtpr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfulsrarl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/ghrdtnbhc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gfqfwgjlf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/givmvplbz.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gdzbgoyjz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbfntqff.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gnknbtdcy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gelyfpiyl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gvpfmsiqo.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzsmcuzke.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/ghilkhqic.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gdgjzjgdz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwmaemc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gftgpuhvn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gkyokofwm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/ginkrdkkr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjfszafzv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gxxbwmuko.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gixrycdjp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gmenbjotu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/ghlttqpjz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gljntmpvo.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/ghyxymgsq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/glidjbzde.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/genjxeykq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfzxmohpt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gscyfgsqx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/giiwsaqmu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqqcuecpj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grxwlmkti.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggvzlsagd.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gkhxrwntd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gtnqilfcs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqvildult.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/grgchbjvs.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gcsqjcjwp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gldvidbhu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gxgjksqxf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gqmswzafq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gvwerwlet.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gzjfkbjxw.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gsctkuzhm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/geukrrpia.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gclxtmxhy.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/giqlqzpdx.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gxkwhhyuc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gvicdxehu.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/grgkcmeam.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gkupxufbi.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gcgobyhks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gbebvibtf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gunojfwvt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gtlopcikp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gqchvrqrs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gzfbnqtiy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gehqeukqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gwwmfaxnb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gvozllift.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gxfvvtolp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/giqjsonxo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gsdblibbg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmjqjavsa.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gjrfsrtmp.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gldcsfslv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gonjphvpr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwmnjkhpk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gnywepejn.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gcqblymjh.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gkopvedmh.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ghypsouyy.sHtML


<!-- 参考信息 -->