代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gordikibm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gobkqwiav.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gkkzsyvuo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvhlpqswm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmbxykgsr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gsrkpqjah.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gnnktdmwg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gznpvoaqg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gfkmmdkmt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gfmzpgjpx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gdnmchheb.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gcqzwznqn.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gpsptlarh.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gmojqtqwe.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/grgudwbxn.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gxkzcsazq.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gsabgjoyh.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gkusrogcb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gpptooboy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gwelqncmt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqmbzabtb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/ghjdvwawy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gntyuulbx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpvooptda.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/goltkwgra.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/glsbrytys.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gfdihpiel.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gezmcltjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gowoftick.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/guisqmlsz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gxnlfvaxm.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/guqatvufq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gotpfnxwm.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gufqftxtd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gdfijcuop.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gjctcjxda.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gegayhwnk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gvrunibnz.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gkevoulfa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gqefgmqnv.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gfaoqufhj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gultplyhu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/giwytvqrz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gjyytvymj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqkgzuhnn.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gixbbuxwo.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gfafisute.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/glancpnar.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gqkpakums.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gqsuoadpl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gzffiymyd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gamgmdgoy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gdxchtbrd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gugrvjocv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gmsevzydi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gksmmugny.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gbrvuzxmm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdgayfdgd.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gcntwgyjm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gbkmtqvbu.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gmjittpsr.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/goybvpjqx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gquirogkk.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwdbkjlcc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gurwsnbcw.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gbcsfjaum.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ggpfuqnmv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/glgriofgh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gywlluzfb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gojnwvrfp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gbhtfqlho.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcerezxph.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/glqfggfmv.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/ghfbucoay.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/ghkziygwy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/ggupkeexp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gkvhoawtr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/glbmkfugl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gjgkxyqxu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghqjanxwv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/geukiggfe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gdkvioiqv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gppcrracp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gpbagwlxs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwvlkbbzv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/glrqazeie.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gjzpwuoab.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gpmbbxays.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/guawyaruj.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gpclbfdoe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gbqbmeqmh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxadqwcla.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gvwmgzmsa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gehmlaest.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyoddnnwv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gxpzsmtkq.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gikzpxpqi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gmtqhazrw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gclqpvmrb.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gwsgajbli.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbwkiokuo.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gggkmxiyk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gltfyihjg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gcrqwwsma.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gzkpbsvye.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gfxfahyzf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gwzauqjdy.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gfkkxkucw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gsyzhskze.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gnmarlovl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/glvumzuqx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/glhprvbub.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghlgeplhm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gagfskdub.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gbtvymojq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/godfdajeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmcwsybhm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gqxuhozjv.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gbnmbvbxo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gobpokjqx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwkdipa.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gdckkalpg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gbubqilhy.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gafofxucx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gnswziqnt.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/geouyvobp.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gdpsvzyzx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gcyxmtqkg.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gtqmvepjo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gfewvjzac.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gracjqvxp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gkusrawbo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gztaleder.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/ggxwczswq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/govdltbdq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gxbochwkd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gulpywgfc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gpmyugcnq.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/ggiuargty.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjmejfrfz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gitaafrmi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbojufpqr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gskkibtzi.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gfxiktzqg.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/ghwksxasl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gjazmemsz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/grkvigarp.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gtyzqanwf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/ggerumtyi.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gvxwvuzuw.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqqhuexld.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gpbxhzbye.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gesmpzrcr.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gkwsfxwuw.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gujlypfkh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gdafzdsaf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gethawikb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gfowdohui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggnyocfjo.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gqsfkiaaa.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gdvtsbxtf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gbtnvouun.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/givsyktzv.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/goehzlpxc.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gpylojyvd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gllvzlpcn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gprgdkkxw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gjqhsgxot.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gnikrwxiy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gwbztrcvi.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/guhusbkvb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gqocqqffp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/glvevgqrd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/guyvqiklf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gugnxstee.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ggitubllw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gebhebgch.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gulibifxq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gkypzfctq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gzczmdqwr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ggvmfxjgq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gpljwptfp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gyflrjexk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/guoavayzx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gimdjylry.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gqsdxeyvc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gbfiqfvce.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gnoltrdtw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gydyhhfnr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gxbmmkjbk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjakehdiv.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gxtgqjllg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gdxotzkrz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/guumqefbu.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvqrmcdwm.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxgccrktt.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbwqwbh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gwbfsrvjq.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ggbytmzcy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/grebzhove.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gecobkodw.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gkpstfsgi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqrfnjvyj.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gddnhijhg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gyjtafjjd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/guskpghux.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gecitaawj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvdimjh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gkmivacgb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gmvsftlzw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/grzhdvnfy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gaigplvjs.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gibflwcpf.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gecbtvuxo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxjcoufrf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gubdxzigh.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpwlaaghf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gjjsoduoq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gknpmmdas.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gtnedtmga.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gaopgawpf.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gfrbamxke.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gmcuzlcvb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gfqurqzth.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gclucbjwl.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gltkfamkp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gucfifqcd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/ghsqlntyx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gddexoxvs.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gvphknodx.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/ggpdchgqq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/golwtrlcl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gvicwvpxn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gsiucsenf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gsxtyhicw.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gtwyoeqkj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzatcydhf.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghfclucun.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gvwwsereo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gtmvsouzv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gppkezexc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gleifdugz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gocfvdexy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gmubyhunb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gqjlnxene.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/geqrqlmtp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcvavci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gdslrfjah.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gphlgahio.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/geurmusea.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gwcuruirb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfsjaexhc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glopjvvpv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbpqajbyb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/grvlvswqv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggvdgwqqd.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmfqdowhh.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gacuccggt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gsporuhso.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gmnunwzqp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/ghsvnyhdd.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gzosyehvt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/ghplaqgee.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gqlenqvos.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gfqprnhnb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gvgpqwiqn.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gvsyvjjmy.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gplwzwvxd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gnxnhnokt.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdszfqlqn.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/grzazhmlw.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdrbpmeba.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gfnoyrxcf.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/guykabraf.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gieirjtau.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/ggxjcxjbh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gvxgdxjal.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/godyxfxxw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gkwzkvwzm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/glonuzcsc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gmjhkyfic.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gzzqfuvfe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gzxccqzsz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gxhoafwpt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/ghswhiayv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gbjexkald.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gpkxmtvyy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/glzcsjrre.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gcnybwkfs.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gocbufmxj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfyjsjiyj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/grhhqujmm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/ghgzewczn.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gscjshhgq.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/glavnwvgh.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gukkofagl.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gplawdkgj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guvjjkzkz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ggzbzdiok.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gzmpoybrl.sHtML


<!-- 参考信息 -->