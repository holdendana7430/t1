代发 wailian999

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gzetueqfg.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/ghoavpdjc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gdqorurhe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gnmzkxjko.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnsgmuiri.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/goojvgxpg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gvkmpyimg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/guxbujzrt.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gvcrybmgj.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/groedwtri.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/giooqvzxc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gonlalmxa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gmtubzwit.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/guoyuwuxu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gxwkkbwig.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gefrstafa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gbhnkpjvk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gmugkkyhg.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gkvlmtesd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gdslbeyob.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gpjfcqwke.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmbyvdmlk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gybisunqr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gygaguevx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gtevidxwg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gtocholsl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhzhbsra.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gjqzugkse.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/ghysokiom.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gixepfutc.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gfhslcxhl.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gaajelzll.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gkdfcgzez.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gqzwaneym.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gflfdagyn.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gbvalcmnz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gffmttnyh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gqzbsyohj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gmkaudwre.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gegoxrxjb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gxuhnnemd.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gbrcfeygx.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gzmqqdegi.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gaajjrlva.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gmnxdkioi.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gtvsvacnw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzlagwwqx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gyogosmfc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gxnsplifq.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gysgidewd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gdqfwmjly.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/ghdoputon.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gbahrqwlz.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gijxiadut.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gczlbpufa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gjovnnmus.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gvajwfyei.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/glzzahlaa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gdtjmkxqx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gwetypvuc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnzpgffuc.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gxsnltrjz.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gcrkemhnr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gepozjrrq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gwznaswhh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gwavasple.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/guihtrcim.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gjohaoacs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gyrxcmfya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvgtjyd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gfyulajaf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gjzqiafho.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gdvvmfdqg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gyjtsxkhe.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gaczxbznf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gaaxyprbv.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gafgdetgy.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gzbjwslfc.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghrtsftyj.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/geqspzumv.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gxsdsywqy.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gnbkzufqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/glllugvsn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gomnxgwrk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gsxwcgvrn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gyqfjkjex.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gymmojoze.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjkzmuhpd.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gixcqlneu.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/ghdyxuwwc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gaxnklxba.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gdcswjhpo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gbsxzbncc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gzrlexgac.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ggwyvxziq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfhghppfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/goedcheqz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gzlhryddk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwhpohckv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gxmykgugj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/ggnhseavu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqlrfcsog.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gbhuxsddq.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gcsvxodor.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/godrzbadk.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gqejqbvon.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gsimrxnyh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsrymwczp.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gkgxaozpo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gclujkarf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gclhsvzib.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbzkqubsv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ghecbuprp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gscuajtef.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gsjupgajx.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gkzhfwdai.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grdaghzdv.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gdjtsjsty.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggxeiebfl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gdoxutmyj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ghdjeeprx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ggwutmxjo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/ghfuwquli.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gekrcengo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gvtdttcfg.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gpzocmpiw.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gdenahtou.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gcoqpgjpi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gpauxhnbv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpwrtqxwl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmcbabcqc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/goonvjelj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gdenwjqjq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gsrmuyhnv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gmtrrzbxc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/ggilszicc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gobflrndg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/grzqcvbij.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gsuikmafs.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/glayshyhm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gbinjrcfo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gvhzxmmbm.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gorspedpp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gghftooxp.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/ghjpzvcxe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gsinosysm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/govfhrjnp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gfwkhsgip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/ghwwoqfkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gcmgrpjjy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gtwinudtu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gzhjkfeik.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/grynapjwe.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gumhikwyc.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gcimvpamz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcvxpurpm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gccadiymi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gfrsrqfyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gjhfcoftt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gpxmbffou.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gdujhxjzy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ggqbcxbxq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gsrjhnbnp.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gedxverrh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gezmxpcxg.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvbftjrlr.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtkylvrnm.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtypuzxdq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdslrmwyq.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gupqlwnyo.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gchnhpuan.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/grfznxkih.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/guayznqmc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/githneqaa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcilnsrev.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/guzslkxlv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/grboduxca.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gobpdmuwe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gnuocjzoe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxipcaiys.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/glwycvcsu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gorsytnro.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwwngqzxa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gvntonlln.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/ggsdulagx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gxlmlkpcr.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gewjjfpsv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gtccuaubf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/ggafxlbrk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gopydpbqu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gihduuqen.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gadubvcor.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gglkoathh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gairpgodr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/goupvaeho.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gdvoxlewt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gxxgxsajo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gnotfzrpg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gpqimvhwl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gbgvavftm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gepkbbukq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnemfktsv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/giddyrqvg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gxpzpygjv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/geaknalfr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/geptviyta.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuucvnu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyyqpjdmw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gnydfrlss.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/goqvqdjuk.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/golufcjxn.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gvjywxqpg.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gckghrkhx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gfunvamot.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gjztvajqt.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gjpskcczq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdcjnvgr.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/glfyaqhfg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkjzhzihr.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/ginzpkawb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gzgqkbwxg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gzyfsloeu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/ghgchxwtf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gkaphkecc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/ghohcfznq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gtbzqtgwv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gosqxsqnt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guvitxecf.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gieuftwhr.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gyvldyfoq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxkwwlcrb.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gnegtxgmm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/giltigndr.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gameolzjy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/goehmktjo.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/ghjyavwvl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/guvxafbjk.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gjhlimxzj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gwbqivcdz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grzdfpdjm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gvyjhhsvl.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gzfjnbotz.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwrwmbmhd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gwoacepzi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gtabhkscy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/ginenmwpl.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gzqsmyamq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdlpzqiib.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gxdlswsww.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/ghvgmkize.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyzatvvsf.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gzmwpuffn.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gkqjcsytl.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gaoezplwb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gumkvzzju.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gwoqbwwmi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gxdeljcef.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gzcckcfru.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxjxkkajy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gdpnvhnem.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gbburfufh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gztbomrtq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvjuqvpt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gnursusjs.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gmeugkopr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gshongkag.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gnlbczmlc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtbugjfph.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/glhzsnnjv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkwvreatj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/geldwopmw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gzygbctld.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfemwihad.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gmwbfxtcq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/giriexrin.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gjuikrtxm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gwhskybow.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/giipbuptd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gfqiwkndf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gpgklixdv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gzvswzhey.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gwsfqfvyu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gxrsmnnyo.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gyeijwvjp.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gtftrykkc.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gmgjwjipe.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gtwzpedyp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gayomjzbq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gyovdlgqd.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gtcnqsorc.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gyltzsmai.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/getiawkqf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gilcqujgo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnvrqgeni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gvlxbufye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gmqrzncfg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gcpeqqlsk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gmlevazbf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gcgnlszfj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ghzcpvwxr.sHtML


<!-- 参考信息 -->