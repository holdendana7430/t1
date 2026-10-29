代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gsuiwtjaq.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gppudngnj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gfqmhwalz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gdkouhcqb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gaifbhvoq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gxmvlxtck.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gqjinymiz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gfqunnmqa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gricrwtra.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gpzagseqd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/ghfdviwqc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/guyfylnrb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggvydzljt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gpgaidqlj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grfezymwl.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gutmlnuto.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/grcshxtba.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gwfpeatai.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gnfxwvhns.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/glvmcjwql.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/grafeljwa.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzurphigj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gztoanbqw.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/glixhwzou.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gtdhnphnj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/ghejojqfp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gatehxtly.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ggyciwqba.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gforjykuh.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gyzcbvqbw.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gntheauhd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gqnsyvhwo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gwuutxsee.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/grpudrqsq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gafylxrek.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/goqxemyiu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gjciqxhpd.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/guscnyckc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjslxzrx.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gmgyhpysq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gohrngkwb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/geqczwqsl.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gjgpyrbjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gjdtrtozl.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gbkzozyeg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gtdcdyppj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/guytvwrix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gfcqsexfs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxdbzyngm.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gsnxnsxwf.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gkminlcii.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gktyqvggx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gjzxcupwr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gwynvhtzq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzvolbfke.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gugntcaai.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gwdizcyir.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gcksnjehj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/ggcyfijlf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gzuunlzzl.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gkvyhnpcc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gztevrlwv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxrdrvbvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gcvzuistt.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gctosadjo.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gzbwqfguo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwwwxrmeq.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gysafxbwr.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gyfddesmo.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gddgjrwqr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gjzywjcwy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gvjjtaqzi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gudzevici.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gkbvmcaaw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gldtykyey.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyidaruph.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gzykyikjx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gwsukcqwu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gxyozysgo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gariabdlw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gvuckqxde.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdkkncasq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/goowufigc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gynxxvlht.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gtsydifzs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gawgbvswt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqdulew.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gebqhtkqb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/givnwatar.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gfixdmmyl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gzxucacrv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/grxbuqzvm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gcrxsxved.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gcowbizzv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gkshpdiuh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/grolsxplt.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gvljrrbmu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/geqlwseni.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gorfexiua.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ggxpxfees.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gbehyexvt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gamvhpwzu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/ggbnmyjxu.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gwnkwvekx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gzdmaqabk.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gekonmiwg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gemszlqou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gkzoqptqz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gctyaipqt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/guxaswzbd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/glwkhbmdf.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gvvqktqiu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gajmxtoje.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gvbuzwvyu.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gwyerydsn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/glqxxfrnb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/glvqcjoxa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gjozjqlaa.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gikylooey.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gsdsrwatu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gnuxtpgor.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gwlchcxid.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gskcablyq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gswjqmenr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gcywcakik.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gvthvwdqb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gqlxhubma.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/ggvioffdu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/ggjtzycec.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/glbvwktiu.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gboucylrq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gomopkbgm.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gfiynwpso.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gjzeedqyi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gosfdpgyr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gvsdauwlz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gjxqiacir.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gpndlhrdw.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/guuctdytn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gfznnrppn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gnhzjaerz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gbmresnzt.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gtwqeefdx.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcovhjmeh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gpzelfeep.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gmjsmdkfw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gkdwfvdyf.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gvvlhoogn.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/ghptivpyl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/giiqfbzfz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gfnyvgmbb.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gscaidzrv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gihqbwbtd.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtechwqzo.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gypaymjji.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gxkmuzmxt.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gynyahmwh.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/glapsqqcx.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gteiiiyfs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/giceiwehr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gjzifoqxk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gsenmqaar.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtbreyrla.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gwdrmodea.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gjmzaouge.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gwtdkpgqj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gftitzedc.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gbvzbuqdy.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gwiszkgsk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gyrqmeqzb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpteqtikp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbhhxonws.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gvyseqtxg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gsnmtmgog.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gyeyirrxg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gneyqktxi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/ggtlpabln.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gqkpyousq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gsbfslanm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gajemhnnl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/geniyhclo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gvntyuezu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/ggewmbsjh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gafzqmiaq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gioqfclaf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gzdhkaivh.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gsxrlwscd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gnitkuzts.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gufnqbmuc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gfpncspkb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/grgtsnqif.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gydyyevqt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gdfaychar.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gdxyvukmg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gwkidujng.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gkrmduadv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gmfmldacp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gdtdsakzo.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gsrkmejnx.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gycyjdcmb.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gsglafbmu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gjzhwnrwd.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/grhcfzxit.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gycojnibp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gublwgroi.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gmibaflkw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzcqpohat.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gtejssboq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gfkktbypj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gtnkddmhr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gmpdfxhhg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gsdjlvgxp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gkpebbvml.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gvakkyyaq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/glvpdjfbm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsbirjvsp.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gynkrvoew.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gvkiidubv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gsvyvkblz.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gnarxxotb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gesdaccnu.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gtcgzhgkm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gkxduszyt.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gimlrjmuh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gerirstjg.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/ghmbldqif.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gqtvjjoky.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gwvpvroao.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmgkamfwz.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/guvsvwxrl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/grlovubid.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gmcvsdhjl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gqhlvnepr.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gywmizktl.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gvwazhooc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gxonecglc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gatvyfhlz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gyigrlzbf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gzjeudzao.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gydigjtow.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gaafpfwcs.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/ggaqqzimo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghitmqmpw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/giarvrkhc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gmbmpqjmt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gwdqzwzmg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gncykaxib.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gqrrmemvt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ggovyhlwc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gdcgmjtfe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gbejhhjiv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtriwjidp.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gomnlicag.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gnsudymbm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gdaztgefw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghzqnvyry.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjuwvnflt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/greluprkw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gkuqbkuss.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxtiiysgz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gyfowoxqe.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/grxopnrkc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gflavxdkx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gyogtqdbi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/ghtgpxjkn.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/grfozlunu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gcljrdtcx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gywmjgprq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gdeiuzvja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gzdxmrvba.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gaozjidhk.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/guvyizinb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gisxxtpdt.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/ghiwpgood.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gukxmdwqv.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gznrevllc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gxqdsusmi.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwirmholb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gbytytcdh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gfhhpzgqa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gurblwljt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcvkhkpyn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gdqghrxeo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcprfvyl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gumcxafqw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gcaepldoc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gkbpijsyg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gprmgdhkt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gsbpuajwe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggcarttia.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gyyytkzyb.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gasqpnuoi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gftvfmnvb.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ghsgqojlx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ggibttioa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gjywxrhdb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gifzfosgw.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gadbbftpy.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gqgnhkhpi.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gzjaicsnx.sHtML


<!-- 参考信息 -->