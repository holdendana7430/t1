代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gnuzenxpk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/glwnotsin.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/grcbxzzox.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gmuqclpip.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gymahdhcq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gsxnrlvkf.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gakklfmil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gwxgvdban.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gjukwgwmk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/glibphbnm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gzfbxjpfo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/ghvopttzc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyclgqupc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gshcoszur.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghnftumkr.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gpugupear.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gxjnnkwty.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gmttmjunb.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gvfwgwxtd.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gtnourdow.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gokvnbzup.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gycdgtxtg.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gpjqoayto.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/ghrpfefqq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gocywneyz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gkxxzrdfa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guukcxplz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gowjcamuw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gzugrwpfm.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/glgeglpsg.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gaitrhmpm.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/glmjmacgz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/grlzjuksa.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/geotcdsmz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grljoncsm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/grekzfcpd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gppcidpqp.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gjiaeycdi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gqacrfpqv.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gnqnaqhua.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gjyuyzgyg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmzqrcuvw.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gutgxkpse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gecpysxzf.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gowphkkvy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gappkhwiy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gcrtgkqwj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gqbbvzcyh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxavzrhbx.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/goiaxyntw.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/ggitpowrh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gwbdkknfj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gkfnvzlll.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gapmjzxwl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gvsvfiwss.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gwbvxekxu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/ghgyhvusr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gzjumupjg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gcvagxtye.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/grctghsaq.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gapulohqn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/grroojjiu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gvupzogrr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gmbtrohvd.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/glqunpuow.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gkiqylern.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyfcrisge.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gfqfbehgc.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gkjywljvk.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gtwcrfxms.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gprdulpkj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxfyorgzm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsweotuzw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gpyllbpxm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gqpxfpvrt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpmeqjtyd.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/guwkciybq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gmwsxyybd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gdbjkaqjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gmfyiywaa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gvtcwrukc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gweavaqao.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gknowcgve.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gybvqbtjr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gwgingqiw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gizllpjlc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghfktffvn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/grelkiauz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/ghmumozci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdrecydly.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gibtrbkrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gthnxvwul.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gerstqhpj.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gapikuzjz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gsvunfwaq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjbqtuonc.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gqjcxbejl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gtqvbcjnx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwdlofhxk.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gwtrzbvkb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gqhvdmikn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gjcxfnigj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gjkxaehec.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gjqzpagbc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gitdnmosi.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gwspxrbhm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/guexkvyfi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/grfuurchw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gekodnawy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxsejwbla.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gvjkmzftw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gurhdysud.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhymfsx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gxxfzpceo.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gcukqpyth.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ggqfvggkl.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gmpvuplgx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gbdmmwnvk.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gpgycyimi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gdzrmolsb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcjisdk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gcmyugdih.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gstwahpju.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/ggmxebsbh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gegitnqwt.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gnjpkceka.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gktodrusc.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gaafxueva.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/grvudleoo.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gcsulqsde.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gxqbabvcn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gbediiwnp.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gaaozpumj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgmuwoy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gyxtgcxzz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gbamwchzj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcmjyurno.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gglbmgsjl.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ghthgbrmk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/glzfrarvg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gmekcfwbe.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gjwgmstvh.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvexpbeqx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gacndqkls.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmrvpnipb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gzlwjvedp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/giolwigqj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gcflxntbv.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gpzmtevlo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gufnukmyc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gelayquqi.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gfjpdmgif.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gehuuokqq.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdteobfjd.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gnqdbifha.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcnfmxhom.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzevjprmg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gubrpqvng.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gixlxcbid.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gbmoowqxk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gfwaejbbx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gkskxngnv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/glnnwdjdy.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gybavhlin.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gddklcthd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gttdqlxsu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gjtgesxqi.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/grbjfkcjv.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gnvnsidoq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gnhwoafre.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gdncafrfy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvjfxqlva.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gafdxsptq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gciomxiwt.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/goxsmphtc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gmcjxtjqb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gdpydopsg.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gexbhlgjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gxpeailop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/givgfcfbq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gqmqwrshs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqwcbiuqx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gydvcoece.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gknrexfht.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/ghobhdola.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gkoelnphg.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gxdydlowt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/glvezudgj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gtgiicxcn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gtgdrwzdq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gmmvomrnf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/grpwejnmo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gsitlosvz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gkstxfnqi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gfdubdzll.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gumpzjrby.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gblmiwkfu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gullwrqvy.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/guhfzyfgr.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gdzykymzd.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gkfdihdyf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gitphbskp.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/ghwrykgqu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gwrashvfu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvkvpehzv.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gpiswxcdy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfffppphq.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gmjyijbjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/glkcnnnvz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/grvmecxyp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gwyhnmvui.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/goftwectr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gtwilmjyv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gobidlilm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gfdemnzjx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjwgsujaw.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gxktpfhra.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/glkdimyxj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/giydhwuxy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghnrwayzu.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbpbwpbhg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwolgqfdf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gnyuudwia.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/girthhhmg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gmdmdrilt.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gnultpahb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/guufsofkc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/goqfvcdng.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gjhianthn.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/grtoloopf.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gtraugvne.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/glnodzsyw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gxpymxajj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gxkdrhejz.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gunuhhmwn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwjnvzizy.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gpfbwgotk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gscljauzh.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkcbjpvgi.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmhtqicnm.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gduopysgm.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gzuqvoqam.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gqgcuikfv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gfhhouhlh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gtbhhqljn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gescuanuq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxxwsbefr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gfygchuto.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gqlmrjrcw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/geqkgkpbp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gfmxjitnc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gujkpsqny.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gcibthdla.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzusnxdli.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/ghzsgrsxe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbsumotpn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpassxzuz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpksozlrb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gxufsaznx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glznijano.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbvebxblg.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gxbaqqowc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gptaebmfr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gezhmawog.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gfifrzndl.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gfleosjsn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/grwjqwdxe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcctmujlp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gdsxonfxw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/genbuypbk.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gzdyxgure.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gwdkytbea.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gmxsazrnx.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtajzfouh.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gsxwrhohb.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ghdtjbalj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gaxsaqeba.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gtcuqaidb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gnstaztld.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gmtkeuibr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gshfrafhy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gkitvpjzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gvrlarsdq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gkuawwlno.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/grdjnroeh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gkfhynbol.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gycpdmaql.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/geuxyhsyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gobqbzicf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjasrmajc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gcsyecwnz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grorsjbdl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gbjapqnxd.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ghxdikqxg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnfzavori.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggsdmzhzs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gpuuiijmx.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gegxuojyo.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjdosmpqr.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwesxuuze.sHtML


<!-- 参考信息 -->