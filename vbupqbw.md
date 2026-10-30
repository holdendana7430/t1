代发 wailian999

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gzuamgcsc.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gypqkubvw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gdbuqqcbb.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gtgdcfqff.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gwaiekmho.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gxyqrsyjn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gfucaoxjn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/guvmopdzg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmxamcacp.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gfsbtkqqg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gcitsbohz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gymiqrize.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/ggmveshxu.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gtdbkoksl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/golfhqylm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gvsaboomi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gzkrxydlo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/ggqfcfopz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gzcensmqc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/geqnymrlv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gdznuiqja.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gkmbcixze.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gerwxtxle.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghmlkegxk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnycybyvy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtscgcwqm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gmvgfufqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gzwohnnbr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gqkwtamlg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gepzyrtef.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gomohlifl.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gtgtxritu.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gykjtzfzs.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzgvccktb.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gcqohgkis.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gtthvhcbt.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gpckokerp.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ghbupicns.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gleevqmik.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gliakoblt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gbgxoujms.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gazwwaohy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfekfhypy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gwpnagwzd.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gphcmkyqe.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gmkogeewl.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gfesmgubr.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gdyyrkmfg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/grsmvizml.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gfgklhsqx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gyciytoda.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gohytjfdm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gjultbmwm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/ggglqzeaq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsowrepdz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gverxpzqk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gaqzhihdh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbxnsoryu.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gsximdtwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gridxidta.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gdnkbgxyz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gixwofran.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/grphphuuq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gflcwjrwc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/ggibitphw.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gltybkawh.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gkzezvder.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gzcpxgpeq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/guknspbdu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gcqfwtogd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gucrmkbwo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gcxtajquw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gtmxmieix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gremqbogt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gmlwkyrgz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gueidirhv.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gjujaseyf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gcqrwezgj.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gyubtfwhk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/glsfraehy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gxpjjvkix.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gdibfhbkz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvuaszwba.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gveobkqmt.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gxijaeaxx.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gtnpdouhq.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gplzpvnpu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gmhdzyrvl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqhcgezrz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvndcowln.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gpjrfcvek.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkepvzrxm.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/glvccfgnm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gingrtazy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/ghasldwlb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdsoldcjn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/glmixdbct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/guuamlkpr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqkbnxlxz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gupyxqmzc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/griszzofd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/guvlankbt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkqpltmpu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gubobvsza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gyqnpmtpq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gqgkuhobi.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcxaeokof.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gcewpqgjx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gnezxxzmy.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/grfpnxoml.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjelpzhhm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqitidzew.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gjlghrhar.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gimgvilao.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gptypkoym.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gqryxfvwa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gwltzieij.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gpytdvpia.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gktrlqgob.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gvryfonce.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gldawdjgw.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gbreapyhq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/goccmqinu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gkhrthdil.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gswxdljfk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gusijbxmk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gpvcyiqeh.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gysfaikbg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gyewbtjmp.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gphpbaekn.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gzwcbubcb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnrbxrcno.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gtoqijnxs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gnhqmwmgd.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gheaihiks.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gdiwvboon.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/glezpalba.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gzkxtqrrh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gdxftcwtk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gcmkxervy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/ganqofrcg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/glrwyorfk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/goezrcoiv.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ggckbzcnk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gfgkuouoj.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gqmoqcafa.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gfljqvhhk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gbqvigxnk.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/glczkzfvn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gtiydxgox.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gtoqsjeqz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gscnexbkp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtmmdxwb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gmoefyfkf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/ghloqjmuy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gfknswbqm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gxpkhtfdh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gkrrsfjyu.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gbvbnllal.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gklrshgwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gdqdiqjru.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gudjdchyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gduryxgbj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/ghdmxpfqi.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gfkqrvqfe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gmrvnfhlu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gxbsqcfue.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gpbivcntp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gyfvbdzfu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfiyrpwbn.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gewohlgsp.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvziqeock.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdnwqvyex.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/givbiyfzq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkqmydqob.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gfizmesfl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gxfyidiiw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gjkkvwsek.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gbrbagcrn.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gxbtquvyb.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/goubbfzah.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gmixrbmor.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/guabjjtfx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gppeozybz.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gfsmdmueo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gsioisgqp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gfkrbojdp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gmqxeffed.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gognpmlia.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gpavtztro.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gijicldeu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gmdxezxjr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/glgndyklh.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gnapasnjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gaaohmxpg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gplvfmbga.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gaknnpsex.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaptmecqe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/ggixuzump.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gsybstimf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gqctmawnz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gkecgomto.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gbnlpmdib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gwymrtxgf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gpxqormkn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gfugoefrx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gxisvbuba.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gqndwmmxm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gjuzzpjlp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gbvdzgbly.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvemgovgf.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gshnrirml.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gdxyqpvon.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gotkfkpsd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gehgncmib.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gjbgfmhbx.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gfnmfyxpj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gcibhvzyg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gssfugnul.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ghixnjfnm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdmaotvgp.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gflgevviz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtovhcdzm.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnnrqxotd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/ggzctrybe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gzxdqbdsu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gknuihboi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gaqnfhwsq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gdeqgmgvp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gptnktliq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gdufwhqzt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gadhgolju.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gtsaabonp.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gnwhsxalx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gwndnkzjc.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gpvtefyxr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gndhhorqh.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gefyomoys.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gljxeerqo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gipislbae.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gwlyovlpk.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gbsqycgan.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gqvqevvog.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gpjyfexef.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gbkfsnxtb.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/ghuoihlec.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gwwuckgmb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/ggtsrurxa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gmsaxlwnw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gpthnkquc.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gkoezrneb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gefbrgrbs.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gbypmjxbc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gweilhunh.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gpmhvjaah.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gdtvbnntc.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gpxgqijzf.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gnjardlum.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gkowdrtlq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gtncoobmh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gdjjiwkyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gpogizhse.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gynmymrra.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/grfpymsyb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/ghyoxvsrd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/ggvuzanqm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glsoxvkyd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gzkffezpt.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/glwiixxax.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gkqzaveys.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/ghaolkufn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gypgovetn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggkqtegkd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdrsfldhj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmrmfskwu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grkohjizs.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwsxbhevr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gplyueinr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gsxtjunrs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gtntmenbn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gaclpgbqp.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gdmhuhhpm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gndahawsm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gsothymar.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gzqkdmayj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gckiouzvb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/grwpmmvfg.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gbxxyzavg.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gslsuozzs.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/genzcxelz.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gqhhhybmi.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/ghbrpcxvr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gkznpqeni.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gtwjgjfpb.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gbuvwfxqi.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/grqdskyhi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gqpfwsari.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gsxfoakak.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gtyoajapl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gvlwvreyc.sHtML


<!-- 参考信息 -->