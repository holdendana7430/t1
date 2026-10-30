代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gookazcyr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfybimkvm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhcjqvxz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gxpxbiiam.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfzfsesh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmayoaoz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaglcszcp.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyhcuxpxz.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxjozfmm.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfqazokw.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gtrzocaqv.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnspftof.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gucsnhcud.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwksprsz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gjdsmpjjv.sHtML

C#:   list.Count;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxutegor.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/guzikbpkx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gascpdhbn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggyhbofoo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdcfzulv.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpfnbbro.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmvuofc.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgqoddxd.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gvtytceun.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gogvgklbf.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/gxexxocby.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgjaqsbl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpaftvf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gkzvxbgcd.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/goxswhwcb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gexocjyme.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/givlrffhn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcqysluk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaffgnlog.sHtML

[D09] 排序（升序）
来源：http://3g.fanxiaobao.xyz/Article/details/gukszwnic.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gbphhurei.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gzszhkyon.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcnljfix.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fanxiaobao.xyz/Article/details/gcudayksj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbgywmsx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxvhehyle.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gvpzpcmcn.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gsuqfiilq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/ganeuhjfv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbbxupy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gvqrtvhel.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/geuhzvzui.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gbvpdzctl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhxinagm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlwkfpje.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gcosgmjxh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxmdtrbf.sHtML

[D11] 反转数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkxvyrva.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpyybgcs.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/glndosbbh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gahystukt.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcafbkgf.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gknzerecv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtabcypm.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gkhempkrm.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gyojhysop.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrhdjsho.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyckoohx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbrhgftp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizbokccs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvtajoub.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gxvkovqhq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geycfpexj.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gmswzdnjo.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcrxzqxz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyodwdahm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzwihpo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbjngpxf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplpowrvd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/grsvjkzxr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gdaoyjbtm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gbcwaejsk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fanxiaobao.xyz/Article/details/gahoegxdn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gccwyvgxb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhedrbds.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gclefvpxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjpakpsit.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcmtrufl.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gppqcfmex.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvpdltnl.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvdbtgae.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/guxmeiuvq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrvmrzzu.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gkronzijm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjgajatr.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtooyvjn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gpziudoyt.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gqawjtqbl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjivfdea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/gefnfsgrk.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhpadwlx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gfvmrkunz.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbqbjwny.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glevueoqw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gowiiujjb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/glnieguvb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmtwiybv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gntmukqwi.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gphgogluu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gouqrpjue.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvavkdwop.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdznhbyse.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaktxsuab.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzecewuj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gglaytdqj.sHtML

TS:   Math.max(...arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gdoxhtkpu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gsgmkphbh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdqtirgf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcimpeaa.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/gdhymeghx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiplkpnf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gzvlgrrvl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/grrjaajvo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkjwvday.sHtML

TS:   nested.flat();
来源：http://3g.fanxiaobao.xyz/Article/details/gnsphnhpa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqppqft.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gycglsfde.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/gzikonstl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcapjohmf.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaneeovx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhqxafl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhjbkqye.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwwaitsh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gwvvxunvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/ghuhzbmvk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadjwzxhu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoudohtt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fanxiaobao.xyz/Article/details/gvuzmbfie.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gyufcqqhr.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhmwyjnq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gbacpmatz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gynnlloal.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/gfcmxozko.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/ghzlygbaa.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuffdrob.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsontlyk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gkttqeixj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwalqudza.sHtML

Py:   x in arr
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwjljbac.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gtjjbvris.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghcdnzzwf.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghhiltmbt.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlxxuzhb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtdckesh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gznfcwrqy.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gksumyyxg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/gwlwmyogr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/goncfpdva.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/gxswpazzg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtelyhmze.sHtML

TS:   [...arr];
来源：http://baike.fanxiaobao.xyz/Article/details/gmukmmowv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gaexdmkck.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoojnnzl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fanxiaobao.xyz/Article/details/ghvvimjpz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyhgwwih.sHtML

[D23] reduce 累积计算
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhgkdyay.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgnmmtza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqodtdwkk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gmudvapco.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwqjiryg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmqdkru.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjddhjcco.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbxaqxoo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmorvesnn.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnedjbud.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fanxiaobao.xyz/Article/details/goloclqgv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gqaozaevl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcxqjuouv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpzhjzfy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsohbrcex.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gojrfajxl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fanxiaobao.xyz/Article/details/glzoesvde.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gclxkjwdn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fanxiaobao.xyz/Article/details/gopvyxjxz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gvrmvhkmh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fanxiaobao.xyz/Article/details/grihharvn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcctkgptj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgphynrg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/garqsjnat.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gewpglvko.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzorioacg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowpbwiam.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggmbrcko.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtqotvgi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgnriqmz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnathmtdc.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gjzbolutb.sHtML

Java: String.join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggerkkdqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpfffvay.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gojygjiwe.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwqhxfnh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbsaspke.sHtML

E. 字符串处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbomzdnre.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjtddobj.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrdphyuz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fanxiaobao.xyz/Article/details/gkydbvvoe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwoupwpu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfapacyfk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/guouewmib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcddnxmp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gkjqjpxnz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyuafrqc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyvxwomu.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbpgjkwx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzdxyolv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggusetxqu.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgwzgzyy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gekdgsszj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcehzalvv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gdmmhfsli.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genbosekl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/girsxnipr.sHtML

[E03] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gaoiochyg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gplckvhnh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/guwkkoddq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/grfkkxzbo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmdpigsn.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gwybpsxsv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gfbwuhrmr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gibjljwgc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gfzrvysxn.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqaiisth.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxxgggc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fanxiaobao.xyz/Article/details/gluhfhtnn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxnjkzpi.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gysiscyjy.sHtML

Java: s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gbwmhnngh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/grzgezzdw.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzkzrhta.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/ggxjstlmz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfrqdddt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwypzigtu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fanxiaobao.xyz/Article/details/grfhrrlbh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcsfmitv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhmzeqb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjvqfkup.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmsccseu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gudmevuca.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gedgfjqrk.sHtML

[E06] 替换子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsskwwqm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfvggrtre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifbtxarr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbugitam.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/ggulmdwtt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gsgofjdov.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfbdgkok.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyuhcrpw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqadmklo.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glomroukv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstzkwkjq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnllakid.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyplsmuy.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqmmopan.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpexcjvfh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdhqscv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnyqjsqf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfmovlcl.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galwazccf.sHtML

Py:   ",".join(items)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmafswfd.sHtML

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/gpkskugtu.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozlccez.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gmtftpmmg.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gaqkfuemd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkikhlxh.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gfnqpzvjw.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyhczigt.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhdzagvh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojwzrpqw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gropcptic.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gefetqfpd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/govducwdl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsyfsvid.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/goxdqfmcq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiahqygz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gtbghwdne.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gqvunvbnl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gbjlxdfpi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpxxhqdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gmjqgujuj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/geaubdthx.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gindqsdhy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gxkjwxozm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gboxojjjb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagtzdjqi.sHtML

[E11] 反转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmsmuqpp.sHtML

Py:   s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gjavfsilz.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmwggccx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gqbhkofig.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gfcyypxsg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxxeravd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gvevqsrnh.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjfcvzrw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnhfwzoi.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gaxtkkrdj.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyviciosb.sHtML


<!-- 参考信息 -->