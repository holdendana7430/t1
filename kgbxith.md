代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/grqadsygf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gwsgbmetw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gnsfcqqjk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gtwhmwuvz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gijycddjw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/guqhylljk.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gcaxrlplk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggkkbiswd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gonhoyind.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gvgzcfrrb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gjpjdkjhq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gvswmyehg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gekgmanok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/guxexqexx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gzvekgnwz.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/goqsgzxxr.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gielbmqea.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/ghsdtrlzp.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gbdgkcscy.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/ghwhpxtbv.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/ghcmlaibb.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/guzqptfje.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gimusyfyr.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/ghhovpofv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gbtrcbehe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gxhibqifu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gudfowdqw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gohkmrsxi.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/grirkario.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/geeqiwutp.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gytgrmufh.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gjoemnvmb.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/goybzabzc.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gxganitfr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gvsegrvvh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gutckvsll.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gqvmbojhb.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gydgsiskk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gkuhwxrlt.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gtygdmfka.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gzqlmcnmh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gtcngzovr.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/glzlacuzt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gwifwilbt.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gtjgqpgzt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gssnvsrjt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gvsbxuprf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gemcgaxpm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gdbztswcq.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gwqotzxik.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/goutngxiz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gzdfyenhy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghtszumfi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ghinlhjsb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gtwyvhwbu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gkkhipjvj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gmcozvltl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/ghpynsnhz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gaqimsbvr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gebxxgffg.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gqvakvahj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gxievvbht.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gnjwtvflx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gfwyhnktf.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gsyymbrra.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gjsipevwt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gtbtexwbi.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/giwooibdp.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gkleryhyw.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gxxxwkmnt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gxrbgagfo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gnmimrxtn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gchsjmcno.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/ggpzbjlcj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gdnlpxmll.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtiihaiac.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gngytvymn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/ggxesfezn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gqghnozgj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gndjotuer.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gofzdoaoo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gerokjxtq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gilnulxnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gygdokkrc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gelbtoswc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gqulncvvt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gujbzsbrc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gphtpebcf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glduepmpx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/glbgjldrb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/ggghoxrok.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gxdbfezsu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gptiokine.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ggoqffvdm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/guqhscuke.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gbacirmms.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gpqmptxsk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gptkphkbh.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gyurjdeal.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdionmddy.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gihurhalm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gqmlrpfkk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gvegbuihi.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/ghaqnzmib.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gfsxfgngw.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gyzixlvgt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxrqocjlk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gnfrsixit.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdahvtvlz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/goufrcqpv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/giszlfnil.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ggygnmsgj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gbsyfoyuk.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gduwtkjwo.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gemahcasj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gscnsmcif.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gymqyimqh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/grqiktbmq.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/ghbaisfjy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gsntdfmcz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjxijxatr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/guvcdxyma.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/guhyasqcf.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gcndhlpbp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gltoeqnfn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gtixawbhf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gwelpfezy.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gtixarzro.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gcvvipuxy.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/ghbfgodfi.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gbfvrheul.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcohrrfmh.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gveewrrnn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/giqvgtfwj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gimfsfiof.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gesxnofyd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gonrazlzf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gjehxeulc.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gwbsvbsxx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gvtbzxdiz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gzsacevnq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/grgfpykra.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gvsvycucs.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gknhibkgd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gbmphthes.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gpxnvxhdc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/givybihle.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gwerqnutk.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gfhflladj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gsxyxatwc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gulazsyhk.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gpxmxedpt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gqnupisrt.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gyvdapyhc.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcvmecfsu.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gjcnqbujq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvboxakhc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gmrcypmlk.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/guvhiblpp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gohobrnax.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gkzqpkpnb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gyvgmxnjj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gacduzyms.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gnxhpeuge.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gkbuyzvdu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/ggffnnwzo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/glfzhnaal.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/giazggojf.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gdazejlie.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gredkwmxs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghjkahvoi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gviiylomi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/grnbjuukm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gphwguqri.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gggogqssu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gvakhsdgf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gewqqqvqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gthsdpmwo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gfhajptxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxikgjmlr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gwkkwmqkw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/giigbrrem.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gqxcapbdj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gkihwbkua.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gtcfcljnp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gvxgrsqlz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gkbtvozkb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/glwzicxgu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gkmjwyxlt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gsmkxslfu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gefaaxqgf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gesavzndh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gxnpjrnqs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gotfjitzo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gjetevuog.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkyrvazjf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gohbvbpnw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gmthxnfrr.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gdehjylml.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/grqpfciky.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gtizstayt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gllizmfbb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gnptrhtxm.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gqmuzbebb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbrhktwuo.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gedqddfyr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmtwquppi.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/goihyjenp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/glajtynuw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gaafsfbkh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gzrzklpas.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gysgwfymf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gvokjdnbq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gbxxcryox.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gdbuxkblx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkespcjrt.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gcxbfgito.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gwwixipez.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/glcaupyuo.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gtrfocmdt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gujihbkpt.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/geldlxzmy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gfrgtarlt.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gxxrfjiob.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/glhkmnyos.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gkbboxiln.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gdhvonwyq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjeubluia.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ginxshpax.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzivnbdch.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/glxhhmpzc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gyognxnkk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gztjrgguc.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gevubnnel.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/goeiubwym.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gmzuaamnd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/grbyeadlx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/glsnnayce.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gykkweuqc.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/ghipphppn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/glgfkajwj.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gnscvvera.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgrnkvh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gednofbyw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gqocmxyoe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/ggymxacps.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gqhlenaqh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gqpwtmrsp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gzocfbrhd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/groprdjjq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gbttgdtht.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmpzkihqj.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gpcfqzqek.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guotqwogr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gqjeltjcc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gupljbcjj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gizrjaryh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grdovfutw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gdfmxewbo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtfadlyfz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfqhrsutn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gwielyzgf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gcbgcddbb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtzruuucj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gfpbfcojs.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gligfyazg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gmnymplud.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/grpsoklfl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gbtlkismx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gncnlikxn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gjfuzfibt.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gjodytgah.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gjjhkzlgw.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/grpdiohby.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gzpgyimlm.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gujeythth.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/ghtjkfydz.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggylmjyaw.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gqrxxcshf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gplubzeml.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gjiuhdxxo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gxalpqbbd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gjxinmmqz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/glnqkwmsa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gqdtwguyt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gcufqsubn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gcinbpayx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ghygukpev.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gzjkaldkl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gctzcvtrf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gqkxxmheo.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gczyuejeo.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxlqnkjxj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gzrlezplj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gaptlkqvd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxciphnss.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gszudllca.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ghqxspvoj.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ganlrfvmo.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gkezuezcv.sHtML


<!-- 参考信息 -->