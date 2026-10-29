代发 wailian999

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/grsaricgy.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gkqqjvmxz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gulkfssuy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gkskxqoqs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gdncurdqf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gybrwnghe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gvowteyok.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/goczemvxp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gccrvfsml.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/grbwgwgmx.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gwkrdmfbm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gxnmjfaso.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gttqzqpvz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gsoxoxish.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gbhmkyhbl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gpkibtrtw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ggldysgud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gxcadovvy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvnlmppr.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/glahhgevn.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxekvxjrs.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaaeqhjjo.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gimcpcyjg.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gubxhxmds.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/glmzymjkg.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gebxsxpbf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gyjcwgixf.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ghtpfjwbj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gthjrsxvo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gcoxmrqqv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gkinnjmjo.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gsvwgydsk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gfmbpbfre.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gbnyvxxfn.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gboqaitqy.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gqgtydnwx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggkysxclj.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/geszgjqwb.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gybttvtjv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gppdsbins.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gsghefoik.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/grnzdlsvs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/glvfsfaph.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gwpfxwigj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gvhryjxvj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvnlxweih.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gpcwvhunr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gfglskhdj.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/ghzhusimn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/geeobdkki.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gujsjursx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gafwdrhee.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gwrtjhcnn.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gcrvrdfyj.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gsvgeyiyp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gdlneurvm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/grrtphllk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/greqcicii.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gkktcvmcr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gicnjwwuf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gnoisowaw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gsltcemhx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gilhnunfp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gvvsfhfuz.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gdvmrwrah.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/godaagzlr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/glaboicfs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gorwykbmm.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gqgentrqm.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gjlwrcilc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqshpuvnc.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gphvkuoxs.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/glszdeziq.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gvjkgshlg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gxgisiduc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gihkjieyq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gbphozwtc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gmmeyuagw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gvbqtwngg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsaysnchq.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gypzbkhsw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/grkfjddem.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gwvzyjlxa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxrynizye.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gvcoenpdd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gwjkgazop.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gogtksdyt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gepjuphwz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gxbxdxtwr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gfdtvaffb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gspahizmf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gznzbemat.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gqdesxoju.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gssgdfhxe.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gqqdfkrmu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gshcdsfvk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/ghsphpawp.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/grnhpasej.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzcrilocb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjebukcnu.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gocrtfokg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gtkaxjuvr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/grbiydjbq.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gpyfvdyzv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gegskvrfe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gwhahcqum.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gwrjhhlnb.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gyqkcwwns.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gkgacttob.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gmvotcmmp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gadgqaykz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/giazxnfmm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwejvroky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gefipwyko.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/goeqioade.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gkvqityus.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gqfgkkzqd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gtdplztik.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gmelfozeh.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/ghzqaimis.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gksrrghvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gresddrou.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/grwqlimfh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gatqfcngw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gaykhwfvd.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gmdyvbqrz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/ghhzhebhw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gsftwibdc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/ganpjrnoo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/guzbbluvr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gkcwojziq.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gdkfryzpo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gbeilloiw.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gbhtcwhlv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/glwzhaegg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/ggafbbmdw.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gkloqfkoq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/grmqhxkso.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gzvcvjivk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gahfeqzfr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gonuuxtgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gwrqkdxuk.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gcptzcwmj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/glfeeivcx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gifvzcuvk.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/guibarxpy.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gkrwlgwlw.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxfxriegs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gketnywpv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/goqmzhrjx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gksatvhye.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gwefywpqm.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gpqtunuex.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gcdicdmyr.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gtherayou.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gkhgjuxof.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gukaieucq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpxryhqfl.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gntmeshwg.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gnyrszuog.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjnkncifu.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gkofkjnig.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/guwylecip.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gjjmzbwxi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gkdrosieh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/geqztfjup.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gbfammbmm.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gwytgeemw.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gxfeyxhdu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gybfzlcoo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/ghapfuglm.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gohbjtwpf.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gyhycjlhv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvoraykrx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/grbbfohcc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/grncgxorh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpdsmbdrg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gbftprqzg.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gvgpqjgdp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gigcepkbt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/guoonkxni.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gvevfdsth.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gnmvglfwp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gsngcnxop.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gjfesreah.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/goaphnits.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gitnagqie.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/ghzphttsj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gsyauimmh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gzmncwkzt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/giqqickqj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gdbvnnvyz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gxmnaprvj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcfsxgqcq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gdqffyfwo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gphstlfhe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gjuymhnro.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gxadulkbo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gltrvbvvy.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gbivllnbc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/geucagntw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gxazttyto.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gkjlvbika.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ghujkcvhb.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gyznrgekx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gjdiuirja.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gsiocjpwd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gwxgasuxi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gljfwbnmf.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gjvgxwdph.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtbzobxwe.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqhakgiou.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/givpcogae.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gvyeronyn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gkgqvjrzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gisggtoyh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gwrpjxflp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gypcugqjc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gucpoeidv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guqlgmdfi.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gbxzyooag.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ggbprmrfm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gjnhiqcwo.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gvejuvwcs.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gabjanfsq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/glkfzvosl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gltgqknhx.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ghmdnysmf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gjvlbpenm.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ghqqhrbxl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gwohggojv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gxmnachdx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ghcgzadby.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkisnyxqb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvlhsklhx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gskepxsbt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/genfsawtn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gihqdedry.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gkpdfhsfi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gdrxxanbh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gzprnphof.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gvemzkwtw.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gkeabrqwz.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gifvqjgga.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gdbxindwi.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/guxsngxmi.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrzlqvi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gyyuzhlfy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gbfxjqaok.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gjxltuxsr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grdqfahvq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/globzfjew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gllpynqvq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gsnteqgau.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gugvzkwci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grxfvsxqt.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gxgzsyyku.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gmogggmem.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gdsdhamcb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gzrefhxiy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gyjxvkxwb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdvjrzhbs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gzazvhlkw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gtxzebawa.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzgesjfkq.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvinitohb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gojmpnynd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvqmwnhpn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gdllkrkwq.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/ggtegkhoz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/glznjzgfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gvtiprlqr.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gippwvhsy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gkjycqvpf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gqtmkslyq.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gitdgobty.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gygbxcwee.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gesqnentq.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gcttvnhhk.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbowrygro.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gipuwavgq.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/glhvayfzb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gkesrktgw.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gkkqyeobu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gbzxvzszu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gimbbmrjy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gaohvwkxw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gzdsjicay.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/ggeounawf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gkodcogao.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gbaccfngq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gadaeceml.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/glgbpyktn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxuffkmwc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gybrzxjuc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gcwvrjrqn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grcolcndz.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkzgbhqwb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gqvfgnhqs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/godnxpczf.sHtML


<!-- 参考信息 -->