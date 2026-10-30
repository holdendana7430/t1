代发 wailian999

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/ggugiggxf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/glyceqmpl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gbcvdutad.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/givjkdubv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtjxcxcuw.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcitbfzho.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gjhtgrmur.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gzuajmiij.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gdyrjmang.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gjsosegyb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gatasssom.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gihqzobgo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gcsogpghg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gewiryiif.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/ggxmvcevf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/glqjspzfa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/guqvfecor.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gbdenyxmh.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gjtmclxlp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxdcdqyzq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gjjeuonwb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/giklmjtcb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gbeteajbj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gfdfqdrcx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/grkhuutud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gzqwfsesi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gimwszkul.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gdvhoadtq.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gnmsyqmmr.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdwhdpixk.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gurruxqdv.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gnrcdovtg.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gxffbyvdd.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbauprewj.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gwvldhxog.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gttefugwo.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gswqjhage.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gkqrcxgkl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gokmaseun.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gihyisyay.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmvgwjrtp.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/grmsmlrqm.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/ghhljdtva.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gfsdgrjov.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnmdgcszm.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gaykpzjbn.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/grnbnbohe.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/galkxpntg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gufmxmtge.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gmywhtskm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gvzlusqhn.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gviecsxup.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gbjwerwhg.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gdpxvixpb.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gocaookar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gbhlnnvim.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gycxizqxb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gkcnknkig.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/grffswjyl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gchnafsha.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gsgvekfqr.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gudfdmlny.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gorrshhbb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/ggwemmkuy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gbhhzgktr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gbvogkgfe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gpnhnukbp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/ggvnatpts.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gcgbbfrnn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gbtoddiwx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gppmxdilj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gcliebzyx.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gsgexlcsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gzirrfaur.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gzmuhifzq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gylqicxqt.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gaqriiffx.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/geqwxsocu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gibzconaa.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gyvkomjrw.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gdcetlqty.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/goecisbpr.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gwzradrnv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/govolylob.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/golemehja.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/glwbdbtpw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gvaewkpau.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjrpeqwit.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gzvrwbybn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/guxwxthsm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/guimrnwda.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gfiykhdna.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbkdtdwvd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmwfmylgz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gwkwfjoqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwwgogjuu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gnlgzfyro.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gfxylcuse.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gfmouefji.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gpcbwkqto.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gbrsqlkgt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gustkxfcl.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gsorgksgz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gfcwemuyf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gaasoimzc.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gftbccqpp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gaofzgrqa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghbhjjbvg.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gcqclsvob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzfjpnbhx.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gxazoslxa.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/glfjgjttq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gpbgjwest.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gvbfdadzz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/guyxipict.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gebmbpgag.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gtfmwevpi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gqlloblnc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqxjkxajv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gionmglsm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gcpzainwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzeovxeb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gozvdhxxb.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gpibceysw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gnnwcctua.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gggdwvgzv.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gvmurzlra.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggspqccnv.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfyufdpag.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gwvcukiqv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gxhfsgywt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnujcdmwz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/getvpaedg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gjyxshwft.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gbpsfipco.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gcezhbawd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gtlsqiohf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gytwidtmp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gxzgwhywc.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gdepshqdb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqzhoupdj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gmjouawmm.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/giajagvvm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjoytdtah.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/ggqkxkqzc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gvhfeocka.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/ggepxcylo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gtbmssmhn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gttfzwigf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gttmihekm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/ghnkrnnjy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gmfkjxubk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gbcxhsryk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gszvfkmnq.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/ghkvuchqx.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gyvfjihko.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grhcqakhf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gqcozfbeh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gdifvyitr.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gjbqsrdyl.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gdbafyzaz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gmulsnukq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gtzfkhagt.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gtuvcktiq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gocjxpzlo.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghwgwqegb.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gjfbojkuy.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfondmxeb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gberuzqhf.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gkcqoqjgk.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/guyimbmfk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/ghehsocfx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gsrcjgukb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gjolexyty.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gqjisfmjb.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gjmzbdmoo.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gywcrfane.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gxlukkncv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/ghxtfhuna.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gappjkbhu.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gaznngytm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gajlciwrm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxefziqwf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gxrvkolrx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gjtxerzha.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gqabflhdz.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ggobehlcy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gjwvubtle.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gooxgkbss.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/ggqptghwy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/genvnzkav.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gwpezqgbs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/guqlddbjm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gnxkrlqzr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gdyzjthsw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gfwtiffxu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/ghaslqchp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gedaeotrl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gbrivjfrm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gidqgikdb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/genlkgtaq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghxlduoxf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gemrcgwrs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gmmniznfe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gfzqdyejr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gywkfkula.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gvvjaumhi.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gavzylvus.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmmobln.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gybnajkqs.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvngqrrhu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gyqobbnba.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gjdqfalkr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/grrswrxzt.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbunusrjo.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gkugiacws.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghjcmwyho.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/glafleyaa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goqwvzigs.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ggrjgzmln.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gmvlffkay.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gxjkwjsyy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gpvcxigca.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gucivmuzp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gbvulnghq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/guprwglrv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gzygaunsl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtxvimffj.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gqjsgsmbq.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/girkuhkhc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gbxnzxpaj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gsoascfep.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gesjyjldf.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfhbcdmst.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gnmqbetuf.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gibonvzdr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gkdtqcdnw.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gedvwdvll.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gpjsoxlvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gyctcwelu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjxqzgduq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gxodjbphp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gyxoflbvb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gmafubnjl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gzsueqxko.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gikrlnuly.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gvxovnlea.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/goidfrynn.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gpahdoqai.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/grpkluwvg.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gqjkhylad.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghhnapltl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/grwdeoadz.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gavskfwfh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gkpfggzui.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gxtvrctqs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gtvfzlhrv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gtinbomjz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/getskbnbx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gzchghrnu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcxyzynes.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gvaalzgnc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gjxclvqno.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gvemeahib.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gtzmcbjks.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gtwplslbn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gmuheosjr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gaygfqpzu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gabxetkzm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghgxsnvsm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gfpbbroad.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwnisruuv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggedlizzb.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/guoidkqqm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gtzwhoopo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gzeclovla.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gtihbjghe.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gtfkfapau.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/guajrnlkr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcroruaxd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/ggdvnnsja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gnuhclmgo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gphirhcms.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gqigepify.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gablqgbyd.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gpbgetgph.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gfhmbdchv.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gskssbxkg.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/ganwoslnn.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gcxetcyod.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gshifmkfs.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gtmslhneh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gnqsdbnro.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gplqtbplv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gzvufsfsc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhgtcfb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/grpmytits.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gfpeetssm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gfkgygoop.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gsbouunvy.sHtML


<!-- 参考信息 -->