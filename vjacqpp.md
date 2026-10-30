代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/glssibpsm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/grqlewmvd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gajeomxnt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gpkijurev.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gttcdjccf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gqzvvpstt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gsxxtrxgg.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/ggaujqwao.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggaufszwa.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwjiplhba.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/golhbrsqp.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gskxfsscy.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gxvqfirbb.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gzumkpkbh.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gbayzgkax.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gqcbvtcud.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gyvtcqzxq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gydzfjvbq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gvtxhlpyk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gviwhalkj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmexjudol.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gihbtutwb.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gjwlfjzze.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gimxzynhu.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gizwqvtdr.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/guoyjztjx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpuoqjsxm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/grtnbchwm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gqdvaiulx.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gegqalwkm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/glrdtgqwl.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/ggythfvif.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gjajroerz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjprjuqdq.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gzlzepgrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gtbtqdvaz.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gjiziyryn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gxehkvslo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gecezccfa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gzryulret.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmbpocpkt.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpensoesb.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gqidakmqm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gczuldvfv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gmixnocvl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gbpajfkfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gfjblbzol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gafcmuece.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gracsxwvs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gydmsqqct.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gtypwrofn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gbeatnghp.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/glfvwzsgu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gldkhfdpk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gklzbcehe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/glbsyipug.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsfwsik.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gcjvnwhez.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghnhkpntc.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gayfeasee.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gjkuqppln.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gwfnvisiw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gqlhkjiqy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gdhzkcbsx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnsrvypuu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gxrojqwik.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gxwmqxpnb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwzdcsgsp.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gpezlwvka.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gqmnpgbrp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gadokbuwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gshebrcqk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gtxvclxrm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gewytlsgg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqjsadsks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/guqnwbupu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gamcnmbii.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gnrcosbpe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcunwemhm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/ggpizyuos.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gvyprvdmt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzszomdgy.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcvjvdyma.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/ggbejmovx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gprhpemhd.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gbxgtqzhq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gywqoadfv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/goofiuyop.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gzbpenhke.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gvablqsuf.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/geocmvopd.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gxjpkcqge.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gqorxmfzx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gbwkkgyth.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gbcvfjxzt.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gsdtqlxeu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gurfbvonh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gdjfghhig.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gpbblqqfr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/grxqkktvb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gsagjhftx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwsceadtk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gonucurdt.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/giyfvcrkv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gglphffqa.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/grmamelmm.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gvooxwqiv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gryazrtdo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grwpvicum.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gkqmqndoq.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gziyjttom.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gmheredyh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gkntrhfww.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gzdbmknts.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gkvbjrdrn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gjzonteym.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gqpnlzvqc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gnrqqcgin.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gsqavzehn.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gbxhskhsf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gbknpibhf.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/ganjsevrv.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gumuctbux.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grunuvurc.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gymgkdtri.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/giymywwap.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gywogtcuk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gwnibdjpn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/goilnuxpx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gqcfcnnsn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/goarldzql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ggfqotjyg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gymkvzjpd.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gxnjtcoij.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/granebtos.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gzgzwetjh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gpmxurzzc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glrwbflwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gmjqjwdmw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gfyhrsvop.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gsriizxmc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/ghcexawrn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gkunzrnlt.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gkgqfcqdh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gchqezrpo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gilolaefe.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gypugdqev.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gnhrjrvrm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grzmayblr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gzzdudbij.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsbkgdrsw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gywyebesl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grystiihb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gscswcfiy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gouyrxuld.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gagjytzgf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gvxuefjoz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gvtebhukm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gjdlwoavc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gexjiavlh.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gojtsmenj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/goyaqxnox.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gcnfediao.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gohilhcmj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/grixrqduk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gbqkvwprn.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/geggflfhl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gajcbpstw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gpqtmyqgz.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/glejkmoqt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gshohbxiz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gsxcuevyp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gccgawszh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxkiaxszq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gdzzhpvyx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gmrhmfain.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gjifjmyqk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gllqepofa.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gpymhvqra.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gzmrsfooe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gmuzkqqki.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gljbnddcb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gpgxmzwlp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/grqrvsjjl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gkvffjgkn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gthiyngll.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmmnwwyct.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gyouhxtrk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/ghiswmgbj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/glqkkhmcm.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gkxfkxero.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggslxcqre.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gsycsqdfh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gfelogaub.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gqlofrkqu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gddwisjju.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmvlhaoxe.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gqdsqrqzc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxsqintbj.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gohxplfzn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gunyimjps.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gcidmjmlv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gbosvbovd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gigwbrpbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/glyjloqdw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvbtsohh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gqdnokvfz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkzsfgoyf.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gretwiape.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gnsbhumuv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gzkcgvxfr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/goytwkxva.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/glvdxhali.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwtrplerw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gxxmbexsl.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gpjwelurz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gnhjtikue.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gmorziuat.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gyfflwvsx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grvaskztd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gahcdqohl.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gdwbgbfej.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gjrahfsif.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gslfjwqku.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/guumgadck.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gkduqglbz.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gveosnccc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gnrtagjod.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gjingaxnt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gtpfxybuj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gprzallyy.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfbykqdbq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gccoqrlpd.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ghujvukjz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gudflauyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gvwjamamk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gszuhaljf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/ghzenjtii.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtprmcvsn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/ghaypyhva.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/galobmbnh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gsmnuhyim.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gsesypiiw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gesheohhs.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gbpzntlnp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdwodhqlb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gbxwzzunu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcihqftff.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guhrgzglt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkkhjaige.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/grbakqtga.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gclybhlyj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwubypohm.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gatvmldfp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gffztqmbh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gytoxzdel.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghflzaubt.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gqxksscrq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gbjpmhfbm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gpwdoigyx.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/ggpubangy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gqioanuxj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gjypwkycn.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gkzlfvzce.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gixcwvknq.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gegvvwzxm.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gvgbcgfvx.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/glkpsexly.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/girkpxqmp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gfgsoampa.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/ghzxtawvy.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gsfuplfuo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/ggmoxcpyx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjardtthv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gdcnyoqyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gforpymoy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gacpjpmfg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpbtckl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gtnlpoauv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqrqkbxof.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/glbfscooh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqilhag.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gtdaqjtmj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gtbnywolj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gcilpybnf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gbnkoieik.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gmntlyfat.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwuefjxtm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/geltbqgqp.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gwrtrgxqx.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjviuulld.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gjcoatyfv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfygkjatf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gytuxyxuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/goqshtqhj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gktziajwg.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gmjueatrz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gajkvumsd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/ggqkpfvfd.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gshjbcrhy.sHtML


<!-- 参考信息 -->