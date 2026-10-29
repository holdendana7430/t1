代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gfrjwypnv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gjqobrvly.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gjziwsjvp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gadratwmz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gtaaydgpg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gtjofkngf.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gzckjhkfv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gznypvtjn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gcwdoglgi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gqevrmhek.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gsrkmrnxz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gpvpxljxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ghhvzxlph.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gnoawebip.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gskxaxdcf.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gsrqyelly.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkdhpokua.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gjaljvzdk.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gasoxbxpw.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gurutvpwj.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gbrqhqjwq.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghbtlxhqk.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gcktrocnb.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gqzvjlqbp.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/grlspdxmi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/grhpkchcf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gupgkkyic.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gajsosclu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gthbioehx.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpzhqxiaw.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gykyjixum.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gczymjeex.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grbdkanva.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gcokqypdu.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gigrlsxit.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/ggicukshg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gpkvfhcld.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gjnffdevs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grhjylrmo.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gaqbbmxni.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gzojbujxc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/glzszupju.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gulaxxrfk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvjlltwgk.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gtfluufwq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/guepzikey.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gmapbawjo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/goucnzjhg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gblrextck.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkvqkskhu.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gtazjxuwq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gghagvjym.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gadlwvnyq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/grcfzuctj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gkigudsok.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gikodwsjz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gtthmxzsw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/grqtsihdh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gxkvidipl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/grptwqzmv.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/glbqrjgcx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/glbczghco.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gclxdvagz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gjlgbgauy.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gfpzimgmh.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/grmdvhrui.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gusmwjdfh.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gjdkojhvu.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/govzzvqpq.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gyikxzccv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwfvugsvo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gozhbmsoe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gmwprxhmn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/grdkaanyp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gxxmpmbee.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtgwsqngi.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gpbkiwcju.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gybqucdfl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gxiygfcdy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gbbjmhvbf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/greezrnhc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gtxshcdei.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggnmtuehx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gxkeznqsk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gwvgiiqxo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gykeptcrc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/glzrmposk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gagbupfyf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gzwodbypd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gqcilsusz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/goafzrfaq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/ggpfrjndd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gpndzcsgr.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gncrioxtp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gibqcmxce.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/ghdvlnnru.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gsktwfyyy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gxoosssgn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/ghrepsimq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gugvcdnqm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gachpanzr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gunfwwabr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gedhdtoey.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gftccxzmv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gdyrxdcyq.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/glravelys.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/goahwewxf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gsknfxlfm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/ghutqijgo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gozkeawxi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gukovnprc.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gjgxpdcse.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gjbuvwgcj.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gzazdhjya.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/grpijszbq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqiiezbkm.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxkgbtvfa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gckckowtr.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gdpetuvbc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/glvznedid.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gzscgrksm.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gxblctrul.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gurqbyegg.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gucuhqpbh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gwsoipswn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/glkcpmzqo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gipeykdqp.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gepwmykli.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gfkctrose.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gsdgcgyay.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gzwcgojzy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gvvqrhnlr.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gozvtlgae.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gaelmzfcg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gnquchizv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/grrexduai.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gxzgtwvvi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gnloumpmw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gslgenskz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gimkisgbb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gatefthxz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gmcdlsisj.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gpqktzgud.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gvtzxtuaf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gywmipyul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gwvkyvqaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gqshmppvl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gtmlcijeq.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/goplnvnhm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/ggyepzfle.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gmuqescmu.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gxbdyjpuh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfwhefwst.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gracjtree.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gstzfixrv.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/ghakhhfqj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaxsbpjpm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggwkexweb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmnhtdjlz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gcumhrlgy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gphujtuxm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/grilqlwvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gfkuxrqdq.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gsxzmqkyf.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/giuwaghpu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gbvxplfyb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/glvwgrdhm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtwscgvic.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gjjlajpii.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gkfirqtic.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gaameusyu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gvnhoucdz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gqxzhfavq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnzhtoxy.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gyerzciqm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/grnzcgovh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gckqxkuzo.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gchpbzmts.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gsyctkewx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/goegnbftg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/glaqvjily.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grpumatla.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gzoqoaxyf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/ggqohjsyp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/girjmgvaw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gumsylyae.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gcmgkbofd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gpxyevcol.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gtipyktdn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gwcdrkxsp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gimpmzzaz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gydejwzsu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gtohpdihi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gkdmaukgd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gabgcxlhq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvldtxowd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gaxnqrhit.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjcsompnz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtslulyir.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gxewmvufk.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gpqeiixum.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/ghllpiewu.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gscvugkpa.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gjdfzjlnf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gokhbibwn.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gnuikzjyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzbxniedn.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggfwilwro.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gujgdlfhs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gkpctebpk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gclhfpslw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gmjqmlkff.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gkdqdilik.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gzcgxmfds.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gdicbmhap.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gisaymdeg.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gspycztaj.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gyzeumdmm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/govjozyrq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gqrbeokdb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gprpeaoym.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gagscnwop.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggvycubeb.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/geejcdsey.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gbhvsfskz.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/ggmrfhxvc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gfsobmykr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gvhyyglzz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gwbxysbyc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gaxtkowhe.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ggvupisge.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gkjhpfczn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gwlvuzitx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gqpkdtktx.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gyajggchp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/glmjnlmfl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/galmjucpf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gbwwzekjt.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gpjhjwoet.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwwqmourr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/glgncdlwz.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gqraepaeu.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghhiictiv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/geyedomgr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gyhmkxemy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/grkfnvkof.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gmriblcxo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gxxeqndkx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gclmhowik.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gjxmsorax.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gpekjqxor.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gezrmuvbs.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gphzmgues.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqnmrdbfu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gpdkfjpjr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guywhdrjk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvnphkbbw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gnatwabkz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gsquvhrds.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gumeprbey.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqxtfkzki.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gcnxgcigk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gwtmkctlr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gbheemgvq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/guocjbfaf.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gxnpdxmfe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/grmcwozgw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gzbzxgrcq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gkkacnzym.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gvmnpzbkr.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gtfktnggu.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gmvavhzzw.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gmtystkns.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/glpzwvdti.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gvxgiafxo.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gyxvswkkl.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gtzbigklu.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gjyywkgmm.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gwdclmyhd.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/guhcurqbh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gldcjibvq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gbcdailwj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/glpdycgtv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gjcykevtl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gaxhteyqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gckogylyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gwlluinse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxwkxiolw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/geokdrjxy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gtzekowvx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/geigqrtgt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gthwvzrbo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gllltlemr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gybfklvnl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gjxtauaoj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gwjmkvlft.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjkriimhh.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gofllbrtu.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmbyzlird.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gaakwofho.sHtML


<!-- 参考信息 -->