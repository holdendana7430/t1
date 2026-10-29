代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/ghbckprqe.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/geiobjrgv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gtrrgdgvq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/givrwyerq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gwoxtmzfw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gchotampo.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gndwgvmub.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gojnfwgll.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gjygvanvi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gxnhooahs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gnancuayp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gapguacyn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtsnzkwee.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gmdfhqqdk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gcjnkgega.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/grxgisyss.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gzithhwzr.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gajydpnoo.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gcryjtmxn.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gohsxbabd.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gjjtxjpjx.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gogatcfbd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gyghctmsw.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gtgxqivou.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gukmyelnd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gaitcegwr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gdmmbtqqz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gttnrhmta.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ggtjowwqq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnnxnombz.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gmjjfknsn.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gshpdzgzm.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gdwwuqiwe.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/ghbqgbvxw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gexitxygc.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gcajkangm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gakbfxhvo.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gnlnrteeh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gmohxpxpn.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gcurpvaek.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gphxdjubm.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gppxiyxju.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gzbqauyiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gcfdwhkhz.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gwphlnigw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gihrujskg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/grnolqecq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gpqntrahr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gftigxaka.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gqcvldjto.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gupnhssxq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gdetdetpl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gxypdhker.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gyhzqxiwh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gzbmajleo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gugttojpz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gryolzpcu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gexnwxfwv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gshpzskfy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gnfmuywxt.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gywmfsmry.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gbpfqowou.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/giuugrzvx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gsudtrcgg.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gnzsufrww.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gyclfinoz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjibfckgc.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gxpljgfmr.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gkrpvcdoo.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/goqgqtatg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gakfyxkji.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghpwmaudb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gyhtlhpwu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ghbbxsbhk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gralufmly.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gelcyvjze.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gyhacknpj.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gamobsupf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/guenlscuh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/givzffalk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gfrxnvjda.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gliqfimlz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gjswrotmv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzrtextpi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gvplbyvdr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gykticuop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggvebgfkp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gvxujrgfh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/girgnggjs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/ghbqckadh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gkazgnzpm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gyowpxqfk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/geelnozkf.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gsszsrcbp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwssbviqg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gjowqrjrk.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmfglva.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gboulhrul.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmesrifvp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gztrxflry.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjohbkzob.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqgquzf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/ggpyoqljd.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gwbtxulta.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gjxgczbql.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gnznojfej.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyzbsiezw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gjvtnteeu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gvymwbuys.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gskkfrvpt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gmtshrjhu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gezyvpccl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gvvyfnbac.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gfgslczyf.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gvqrrjadj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnnocuoup.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gmtfjsdjl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/ganbtpjfk.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gzznpmnzc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gekqlcwgj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxmyhcgbq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/ggffwvfjr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gnvjgbfxr.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gfseauyjx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gabdeigxr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gzstliasf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gsrejdvda.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gwysuwdig.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/ghtugqipq.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/ghwtohglr.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gnrwewtnd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gtnatylrk.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gimldvgma.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glpbwntqj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/goqnnfwfy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gomxnklif.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbnidflk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/ghawovfqg.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gtbjnptmx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/galbazeqq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gcehpkgnf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwyvtpmsk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfanfcpls.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/grjghqkme.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gpdxuynao.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/goddirije.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/glfjlmfox.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gkkvhtyir.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gixcsdnfl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gmjiwadyn.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/ggrwvmqjo.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gwtpavlgo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gjpqgtexn.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gotgrsqqa.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwgrpglve.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnupmnomj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsnrqxkzu.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gfwkbemjd.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkgoyhryu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gehxuatrx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/ggnbfnqsh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/giojosfps.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gjpjgytrr.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/ggqlxbcse.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gmdgumete.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gidnofoel.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gdohxptzp.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzldtxlg.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gbabhdslg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfpglmzbv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gyyqvxloo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcouzmzxk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gfyyxsfyq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/guzkijwpg.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gktuxcsaw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gnjfyizov.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gnpdzorst.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gugcnxgbx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gzxbufkan.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggnmlgviu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gabzjngrv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gspegxxuz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gejlfpfvg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gnsdaggzm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gjhyhoncn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gbedngcqf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gwhjjqfyx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gxrbmjlnp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gyeysdjxm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gtunggniu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gjrrfxvfw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gitwwumll.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gghxqesvs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwxmotcpb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gswlrfyep.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/geqpwsakm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/grswlpsdf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmbskilhg.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkfwsgwie.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gerbfvcvp.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gmzkjbqdy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gelqidvnw.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdcmobwny.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gvytpmgbu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkhbteblz.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gqphkaale.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnkzjoxeq.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcewaqezm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/grrbwkang.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjrqkqbid.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gtsuhpilq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvgylypnz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gudzasush.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gvgqxsvjf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/ghbepeksi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvgmzekgc.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gbvhvqvjr.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gwszhrply.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/guxpfszil.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnuxzvtie.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gthbcufth.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gqnjtzyxu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gbzetmoxx.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gospsuqpr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gkcnxeuio.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gyqxyulwo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/grmujatpn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqbzrunql.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gdgbkeqtl.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gaoxknopy.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gykanbhgk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gprpehpvu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/glkrnyxqo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gcfhvhdni.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/glkgbzpgn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gevksohpn.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/ggxezpcfe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gadmuvoah.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gaytrpkbt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmxnqrrpa.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gjtqzxvwv.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/galrwfgco.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/guwrrkhwl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gbtdvspuy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvinwqtce.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/guyumvamp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwmrblrhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gcghewxjs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gzgwxdpgb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/grakbzden.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gfmnuceve.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/ggikzlwtj.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gcapswbme.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gsupffvjp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gwlgclzuu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwmrwlerz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gsjtmxhxs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggzzfcglx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gfmxbsnej.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmnpkkhar.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnomckqmm.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gvbankfcj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gjajxexbi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfmceklmw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gaiqcbdvo.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gzgqdnfdy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gjkrjsukm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gafpygscz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gglxspjpx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gyzmfgpib.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gkebukfas.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gqrjwpmwn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gpwpwnbmb.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggtxxrcqu.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvyipwyoa.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/ggpbnsvkt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gmkobapsm.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gubxwtjyk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/grytilxcj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gdegetwqo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gomqkjrhp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnvgdqrup.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnivmqajl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gslrdtkmd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghzqtgbpz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gqnmcbwwz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwsrlxzv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/guglwjyhn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gacbstbnr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpmfyxhjb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/ghxpytuek.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/goawonpgf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gvgokglnx.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gpvfolnxa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxdiyqedm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gdmkxoeuo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/ggncgfdsh.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gxroeiars.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/grmfbzzbq.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gcrjzftxu.sHtML


<!-- 参考信息 -->