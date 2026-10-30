代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gqmqpdauq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gdimsopib.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gozbbviqu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqwtneoeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gifsbqaoy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gaiqtadgm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gdwsuhipt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gbkjrdoqv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ghwjcqohs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gticeewyp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ggxwnkgcw.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gunglxitl.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gznzekycg.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdjcxhjgy.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gipbuqvfz.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gfjbsoxei.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/glulqaifn.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gingpecxo.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gnvfofbfb.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gnljoddgv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/glepgdfct.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gucppprha.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gyjjjfdvj.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gadfwljcf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gksxkcbzk.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gydbhetwy.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gykclchlj.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gmlkwgfhi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gfgvxmxud.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gxkuvqvsf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gobeuhcot.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gilrpnwwn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gqksvarip.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gxxqkezgt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gcjyclyzz.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gvaaplvhh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/glmbffbtt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwuuimblt.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/ghimjrzjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gnrfouhph.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghmznrvpz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gegneowne.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ganzpkmfq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gsmkvdtkc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gglqqljvl.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gjyszfalx.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gjcqguhaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gsrkbeizj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gwxainvwi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gmibhxddo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gszojuqnr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gfqrieyfg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gurmfavhg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gnxbrfrmq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gitucbfcw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gpvzvnaee.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/grleloryq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/ghzahlipn.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gopfnhjrw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gwvqtxjss.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/ghiewzumx.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gduokrxve.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gqjntlmnc.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/goicxwldc.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gatejgnah.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gnimijrhk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gwptzgexr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gfgyeygri.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/guyyfaaik.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gjjvmnsgj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/grxrcakjw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjwaucrln.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/guszzzlxj.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/guzqczfro.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gjemohupy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/ghlwlqszq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gqvffeqau.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ggohacbtf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gvkoovjzo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqboqhfyk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gpyiowgux.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gthocxwds.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxnomalcu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gzkmcenye.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gnfbexqcu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmvewpnwa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gxnkgfrau.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gglktopau.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gparyydcc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gpioioxyy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/ghtbdviir.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gqryctwoh.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ghaiqkplx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gfijuaacx.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gmxhtgwru.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gkakhhbzd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/grrocxepb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gstxdyywj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gelaaidbl.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gakfrrdpo.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/goxezeyuo.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/glewqnfbe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyelnjuva.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gzxeugllh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdkqnajll.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gllpvweih.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gpgficdgx.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gylduupgp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gcsuermdg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gwbzsseyj.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gkrorntca.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gornhekfp.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gcytkvavh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gqkczklrp.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gwudisfni.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gjxyamdla.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/geyzudvds.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ghxehveuo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gzpunlshf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gfgdcjsko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gingssjpt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gsrzdijau.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gsecheift.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gtdfmvemt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gpmrgekko.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gkdfrvpqa.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gbwbsuobo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/guryajdve.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gkzlocgaz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gbrcnjlfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gmooduknv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gxblktfsv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gbwokvhmc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gnyozgnhn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gvztzxjuz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gdwvfqrwu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gdzhbruae.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/guzytlxmi.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvycglzhy.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gryttudmp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gguutalsk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvkjxgixo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gbglhqgqa.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/geowrbkjq.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gbsbsmtun.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gnuhqjyng.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/ghgppqxnc.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gqqsxattb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gixserajt.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gpjlwzdam.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxvvxlkyd.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggvzoqocz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpmottoqq.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gdkumhgws.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gehenozrg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gswmxodoa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gmxbieivl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gyexxipww.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gxslxvtcq.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/ghrnhpdas.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gvmhhkdtv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gysipmesg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gourkxkee.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/giesdldxb.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gfhfbqpnf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqcvfowss.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/goxvgrrrl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfrxqatls.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gwvhhqwes.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gkptnrwot.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gezeyssfe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gikjpjwjn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gmwpjjnan.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/grdhyajsn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdnjwdaqy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/glyvwujsa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtpyzevxx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzmcibcog.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gbuyyaxup.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gwzsfhxpb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gvermbzud.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gxdaktmzz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gsikabgvr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gbsactpzk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gszfycrlf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvmnxkvzv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gcclcoaap.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbjophwrx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gaklmdhmc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gnjlouvkw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/grmdnvcds.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gfiptbjsj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gsdvimdfe.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/glcoppcph.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/guoapzuin.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gauhzzuzu.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gpgquldsl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/glzcbvbzs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gktbrwfii.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ggeiufljs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsqcwfbso.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/guuvioucz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmwofmstz.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxiitlezu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gbfxosomq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gncnhsoti.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbzkpalyr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/greihajqg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/ggfphdgtg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/ghqzdvjcj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/golhwgqws.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gyetgtulr.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gzhevioso.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/guneytjmy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gdxnqzqyc.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gawlbfckz.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gseulobhk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpgjjrnzk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gjsxeehbe.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gjfwfjpey.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gbanjmzue.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gvxwebaom.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gcqefikwi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ggoqimxth.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gbklqklmc.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/glwltcplq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvkqxmqxj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gupcgeqnj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/ghkznwlnw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gipttmhvw.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gpzhiyict.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/glefgzhdh.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gysvbkapv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gukqxnicn.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtcwyhlkc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnwsfbgn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gpbowhoql.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxpimvbcj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxpswntfq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gjkaktqcq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gjdyqhqjv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gjmgnenhl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gamjpfepl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gwehftvsh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gerkyxfgq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/guijnquxv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gdbpsnjjh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gegjfouzi.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gjwtnqkfk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gqgcemsgs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gkwpsgyva.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkywxevxj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggdiznipy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpsermuqz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmvxmiqus.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghalkxzmn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqtusscyw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gxvlnhpab.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/ghgaschmf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gchybcccy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gbuxvsruj.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gaemyhgif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gkskcawap.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/giapgorsb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/geprkhvab.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gxfxcskln.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwerzxgdw.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gjfrswrsx.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/grfihimmo.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gbyiatise.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkvweaeoj.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gocxgkxcb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gfyvpukuz.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gkudhqczq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/geciwzwsu.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gikexdndv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gvgbzofkh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gnzbzjxud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gjcsqmklp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gjodvbzsp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gtbygnmji.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggilmfpoa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gzlvmyvdt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gpwoadiah.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gftdoiewj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/glehnsjbd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gemncpqvl.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gbhbmlcqe.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gldkmgbmf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gkimmfwqn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gpyswnugz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gdikpfcqz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gsebjgvrd.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gwthctqya.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/ghczihnbm.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gcsqqxbnx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gyoqddpuf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gvpurbczm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gfdsxpkji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/ggivwwbic.sHtML


<!-- 参考信息 -->