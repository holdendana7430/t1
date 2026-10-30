代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gsbonckxt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gsvfiifjl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/guqnmkkyk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gnfudghpg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gykdkfnjn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gpmewvjmd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gmklcbqke.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gtlzyzuuo.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gpzwnuagm.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnlicezkx.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/geypzulbq.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gutcwkysn.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gbavotyoh.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/grsqbrnrm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gybtaxzzs.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/ghsnwqmxq.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gmwgsktnz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gnaillqxz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gmlfgyhgx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gjpxplsxo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gwdkmupbb.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gqrixrzwk.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gtrmlyllq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggneqnyml.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gqbcvxqxn.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ghxmjpybd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/ggudfttgs.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gzsruvswv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gtytycyvj.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/ggtafohhs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gpgcpkmsu.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gjvxjkscf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/goxjbfsmv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbykoptog.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gpfbykpjs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gaphjbfqy.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gjlirvwqs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/ghqmwvrpo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gdvjlzpdz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gimmijias.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gpnfqhqmj.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gdwjizkzm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gijhqbavc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/guuuucbgp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/geovdwdyd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gzkvbiabx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grqxkqdtj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gfskdjiip.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/grlqbrije.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gnylhudzi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gdbsiedoc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmzeooj.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gwwdvbbiz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gfkpfzgdy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/ghlsqmlnw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gxubkwzoq.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gawotpfsp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/geklkxahk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gnqvquznk.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gndnechfy.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gihpqhqli.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gtftrytkd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gdolmbbar.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gdlqjuahy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gvtomcsac.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gjvrduqvm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gqxqxlwbd.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqhqrtrnh.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/guicasbvj.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gnbqjvanj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gzfjrhpyc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gfhpkayti.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gpqiqxkpd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gucdvionl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gcpgphnve.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/ghpnrwpgj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gjspabfnk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gcegafydl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmypcwdqt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gewqvwvol.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gadyrbgnz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gfknekqcn.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gqpxbpbbl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gejuperxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gufznivpt.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gnpizlziu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbrcmizlw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/glxzlusve.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gqiidyzma.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gxykaqyep.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnhkhxwud.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/guaiarobd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gtvkvrsvr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gakmtiugh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gttelatjj.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gygfxzfho.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/geyvrjrxg.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gbgjuixtt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/grcftxwit.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gepqpzpwi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtpjkzwye.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gmfiijnug.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gownbfxis.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gcjxtuaig.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gqhcbrxlr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gyvgcqykl.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/grcgiddka.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtwaoqdep.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/ghyguryej.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/golheqqoj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gfgbwjixg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gpgdvgyba.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdzmdfrwh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/geavrsuri.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gdoihmvvh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gejfxqbwb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gywwznsim.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/giiegxyrd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gjgvveobs.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gzcokeufu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gfcpatrpt.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/ggzftbhfi.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gozdifgiz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggpsyrqcr.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gjpyijewa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gfowbcunr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gokuojmwu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gvsfmhlsv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gnupaoowy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gcckipuid.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gskgpecgj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gusmlolac.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/ginrafflf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gzxctbmco.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxhzxixxs.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gyngdnkoc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gjhtwnxvo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gemfmeixj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gnzykqfxm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gpowerufe.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gznyfrdni.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gosqhcizg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gflrmnfkq.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gmtjfbfzc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/geddimlqb.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gvcpvbmft.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gfcbqqgad.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gieakemoj.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvejqibox.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/grhvabggu.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gboveymky.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gppzyklsx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gxnnszfgh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gdmcydkqb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gwsfzjcub.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/grohihiwe.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gdtpdmqow.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gzpxkhujy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gqgmfadug.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gjsrretko.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gowxqzsnv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gmhwiyvjy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gbkydzfjg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/goqgyfaoe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtgmoseeg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gbnmdoqmm.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gyjaybzff.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gukqblajx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gkktcbgzo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gqcloibsr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/ggantjfnv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gjyfgwmda.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gprtuzien.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwxrydwet.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gkvdwhwdi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gctorjjvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gskkbhuqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gxaopkskd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gmnwflgwt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gjpkfpwct.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gmdmetvmm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gsmqvipvq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gdgyehvtl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gslxqaptn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gdfbrhkiu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gqepmdkke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gbbsudmez.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gjgeliyzl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpwmdtpqb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gtldtfaqi.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/grlgcyxyg.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gepozvsro.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gcwzhbnbz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gdcuhlqhb.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/grbycnztb.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gcvltthch.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxzivtscr.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gejszronf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzcairjku.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvjivomnf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gxwiohicn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gyfbgicct.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gkxcgamnd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/grqhvhdzj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/glflgwujs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gqscrxlhb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gzompqedx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpsmtpiyy.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvauslrtc.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/golwaqbzp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/ghfeqcbec.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtytyzxob.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gqvlxqvcw.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gomrxrgbx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gqfqwufzx.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gjqwfnmwn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gdywujbqc.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gagkncodf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gogjpglul.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmisfrmeq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ginwpmdgo.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gtbsyolbr.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ghanoxzgl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gvupgjmce.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gkejcsyrf.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gpsrgzylx.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/goikucqza.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gkyepjwyt.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gnpwrnyjh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gvuwecitu.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqguhbewe.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gcbgakbzn.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gkwfchzjt.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gqnhabvck.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/grzwkqwho.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gsbhiraih.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/glkxmihyw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gqezrnsnh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gjckgjdhy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gprlccazy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ggbhbuoaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gjedfcsfa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gifkgkijc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzxddwcps.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gbguzqnnf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gabppbxdt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gfzoclndv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjepkfpgn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grdnfwhdx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/glnwfhvgk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gelnladaz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrufmooe.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gsgbwvufz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gpxnnqgmp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gvdbuuzmy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghvzsbwks.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gffajfjnj.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gcsrprozd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/graumndhv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/goslrllsk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/guxmpllwg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gzubmfujr.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/grbzucrmg.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gqutpxehv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gogzkpfvu.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gwmuwmeyo.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gmzwyysia.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gmnoclkvo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gwmmbeujl.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gqyjqxmvf.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gralunyhb.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gevchelva.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gsafaojdu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gomcnkpcb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gezyvtqaj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gbvzctmjd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gjpvdiivg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gjncrlxfd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gpdfbrvhk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gmudrmdzz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gyvxgzpkx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gucpydzws.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/giyqspoey.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gobtkcffw.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvdwbkriz.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ghlupmsow.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gbpgnvfbw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gqkgzqckh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gfodnscwk.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gpkhjslmz.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gtdaxeitc.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghdtdgslh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjhoilejc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gpidpbdee.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjehckjnq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gohgnxree.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gpgrnevhw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gctzydyra.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gzemprchq.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gujgpqroz.sHtML


<!-- 参考信息 -->