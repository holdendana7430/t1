代发 wailian999

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmfubecld.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gojyyapen.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/ggvdmegfv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gglfpbtxs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gpwdklyfa.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gzpytjnmw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gdaflimql.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/grmyhhaqn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gckimgica.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gdtcuoiqx.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gcebvyolm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/geojfhhnx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/giqlpdgkm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gvrbuokvh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpsuztpzs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/grcomraoh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gaannzxwc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdjybofre.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gdbhpooqa.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gnizsflwi.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvvzdnxau.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gjfwektmn.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gprsydxyv.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqerxhvcw.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gknahryox.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gieijyhos.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/glppuypwg.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gbothbtef.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/germtkrlj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/ghookyael.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/giyuvlgmd.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gojjdhwej.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gfrzdzmsb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjehbyico.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/goytgnilb.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gurgbfmwb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gsxdtflkm.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gtbrbuhyl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gmrkzmfon.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/goardsjby.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gkmvcmujh.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/glxaytrth.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gboistqax.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/ghshgzzrv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwudekzgf.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvyggdalt.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/glzhqcvbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/glrbkhzme.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkyafntpy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gylwbfchd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcwrqxeu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gphapyfup.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcdqvskuv.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gcdxgutdb.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gjydslutf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/goddydulj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gwlzyurhl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gfdumxmjo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gbdabrpjy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gbzzsumac.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gwsqyawbe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gftclgqcn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gucdpbmni.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gsakjlbvd.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gegrtintu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gpgvdvadw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gbhlebgpi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gufsoxskr.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gutdnaong.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gdvwdvlhw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gwgnguxac.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gebooklbu.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gpmmktjlw.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/giitqdfnf.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gmuqghllm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzfwsjwyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gruwwkduq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gbdoazznf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ghimqfwvw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gopyowbon.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gupjweszt.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gchhvelsw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/glwevddia.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gqejulyvd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gffskgxls.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gniglfllh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gyregrjww.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gqxobqpqj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gjgfyfsji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gxfgtddsw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gajhqsncx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gokcygamf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/grldqktwm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gdkoiowkq.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gyvoagosi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/grdimyaxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/ggumjgfux.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/grcpstwzl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gyknlqnmv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gckevimuh.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gcillrxuf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gcsmscsgw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcghwylqb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/ggpvikelu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ghjhzdups.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gupeyupsj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gxefsfjrs.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gvsaqpkqs.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gfefkvcrj.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gsmfxnkkd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gwlsoworu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gasaemfxw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gixdkczsi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gssbfsyhv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gixrkpcvb.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/grwddrbkb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gajnlltpm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gmnrsbiaq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gjclzswsy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gzoupneot.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gvspuasch.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gkvgrsada.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gzbagfjsk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/guhjzidce.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grecmkjiw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gczgbtahj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/glxsbmflt.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/guriekhlj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gjwjofskn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gmzagggdr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/ghvaxlzbs.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gtpegvyur.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/ghrrztzbp.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gkpnkfary.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gownavrmn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gaaeegtwc.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gsemamqqs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gnuvuglxp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gftehwgic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gxeradbch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/genytiusd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gvujppqdo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/guktxzrgl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gmgcgdpcf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gucjhtxum.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gqfrjfyzm.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/ghwphuvks.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqnaxmyyy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gueygfyly.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gegrhqdyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gymgvzeqa.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gzbgmjcxb.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/ggtruvgbm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gcpsiebaj.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gtnzdmenv.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gqfqykufn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjllvewff.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjtfnxujy.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/glejxuori.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gjjxzhvln.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfvtpwavx.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gtafxvyvm.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/glaxxgvnc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/grfhapacl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gboafcqqj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/ghfzryfqo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gnssyists.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gcbfpagyh.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gsyffjkcq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gndmoqzen.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/ggsqvzuee.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gnkylgibd.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gxzncftsm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gapbytjnq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gumzwgrbt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gomymspgc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/guvxkmlgj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gntrjuapg.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gvppfoxsv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gryfzztpz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gessjhqgr.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gcsmwptbo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gntacwyyb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gajlibvhk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gzbkcoxwk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/guvunyjte.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gjikebjef.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gexrbcbts.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gtdgmvfqo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/ggdxywzuq.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gwkaqbocj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gxiojwaxd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/grfmjccoh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpbvylnqs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/grckhsfdu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ghspztrsk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/grxsnpncx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gtqqlffwq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/geneqqgsf.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gxqyexqex.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gethzcqdu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gqeryscwt.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gseeywtzi.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gsywadpud.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gpiquqtrg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gihhaaqkd.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gbemonqlp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtydmcvr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gytqmwjyd.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gfumclyig.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdkvhfmie.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/genpxrvjq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gjhqymtjn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gfzsnpkur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gtnbgevwj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gixrrmhur.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gkkyaiwsr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gapbavatc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gmccywdza.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbwcpdsmv.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gyyvdvkbf.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gaammwgik.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gsvfnzfuw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gecwrpgve.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/glfxshwjf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gxpzihbib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gjmrhmtxj.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gcspezugu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gpetotfco.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/giznxbnts.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gbivemkwb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbfhfmrvi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmkqwfuob.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gsmpzvwhg.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtgqfuujg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gtwjmaxxd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/giqcpnmji.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/ghkazthir.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gaqaettgr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ghtutjqaq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gdbfyawft.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gzashzkkj.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gllikmzci.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gbualbjdu.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gkqxiqkqr.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gvmsdakon.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqmhaswgt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/ggtshvaab.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gkiufejuq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/ggzxlxjyg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gubsqgbgf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gowclanmy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/geqkcwesb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gyhcumcgk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjsusuajr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gejlalrxn.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/ggxvhjozr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gboyzejyj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/ghuzislgz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gajzgvdls.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gadiwgybd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/guhzkrbou.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gxktionog.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbpjlbvti.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gklqeyehx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gqpunlbce.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gvdzwghlv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/goqkbkeev.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gnsxkvqzm.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gzujylynb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gcnffewdp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gxjqxlwau.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gcxsgfxju.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gdqgnurrk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/grylszhip.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gcegkkyfp.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gacawenmh.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gekeqojzq.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gfaflkhzc.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/goeseraqi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grdrcfhfa.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gqpdfgvdy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gnszkgpce.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/ghcfhbxcz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gsglinedn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gbjojcfkn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjizvgxey.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gtvuokqvs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gogkybmcx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/glvzbaxjh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gljdbjwzd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gwmlqxwhb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gocketrrv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gqmacaexl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/ggbuiblda.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtsyzwuzy.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gsvgqqqkg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnibavfga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmrrtttjc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gnxstlcbb.sHtML


<!-- 参考信息 -->