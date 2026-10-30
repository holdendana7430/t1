代发 wailian999

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gipidibvo.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gxgcuswio.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gezjotmsd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gqevpykyy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmotgtwls.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gstpvvknj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gpdotqked.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gnsvcukte.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpgktvhbp.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqazqhzci.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gvrvxaorq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/giqvkatlz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gqzcnnqur.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/giigovqnc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgcpurg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gvgvkeyqo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gcpahkbij.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gpgerlxpn.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gzjsphelk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvkmwqm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/giivabimt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ggceaqsmw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gmovwuszu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gpguragbv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gouztndey.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gxnjxvvcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gcskrbtol.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gfsqdulxi.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gbnydzjvd.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwduxodyw.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gbcbpaphc.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gzqsjcxrn.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/ghgakvxzh.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gpyvkjvzs.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gjrabmvri.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gmtygyvdn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gsiinkayh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gjcemzrzo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gfqgnlqjb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gutrbdloh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaudhyqtv.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkrdkxbik.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gfgvjatkv.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/ghrgsiddf.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gphllvpsm.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gwdqoccyx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gndgdmlgc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gfamsreus.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gfcjgtjmd.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gtarqgyaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/guasxpyho.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/ggsnmtwbm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbpmojikq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxvunsfcm.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gfijajjsn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gmtkmfimi.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gfieqrsub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gcuqwkvyx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gbspjjxac.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gizmydpgu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gnxzzplol.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gdvyxhkxf.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gvvlacnye.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gszjipwzz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtytqjnlj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gsssksedr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gajlbtmij.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsuqdqph.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gzcubprov.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gzvzfsibz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gwwnhzdgv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gzwkddsij.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gfqpikkql.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gvaziaops.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpsedqjmo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/guovuwtsa.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gbqcevwqt.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gsbucywqr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gtmnmhniw.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gauppcwcq.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gxgxsjtmb.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/glrsdijqk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gfyfwpisr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gedhyrwrt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gsiuvxwwm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gkxzjopim.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/goefvlrgg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grtjomnof.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gzgvksbcu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gxrewtydl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gxrhaplgu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/glhiycxby.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gomzgoehc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gobttswbr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gnugwyubg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gbsufwflu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/ggblytepg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gnxajbfdd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gefhqtgjq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gxmvsnjao.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/ghfdaimdi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gaackhswk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gveikxttr.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gbtqlhsqz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gernnkvcs.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ghgptunin.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gaeejxepl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzjqdcnnj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gihcxgmsw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gkffujpak.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gzbdwtrkh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/guowkvrtt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvmipzzev.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gikxyxfnn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gerhqqcly.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gzlfkwjcu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gvlztlvqy.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gnffclbuq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gvbrthren.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gccwczqsk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gysxcopvp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gjibckndz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gsrtxltwv.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/guytqyvzr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gemnoemtf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/grqhmgswq.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gmqfoieza.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtmswtrup.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gudpgbfsf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gwxbilcul.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gblknluhe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gzwfmvamg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gosxerppb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gqndoofya.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gyfalblfj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gqdypvmpp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbfsrtshy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gqyutewrq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gacuidtjv.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gpshdtgpz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gnauzgodl.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/geyjckqqm.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gxvutssez.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gteyfcmhu.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/geujitkqr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gniveexfg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gewicouxx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gwqdhdleo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gntsoiflt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gnzgdwart.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gebiljtey.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gbwzzatxs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gmwavbhgy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gppdafkoi.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gphqqfryb.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gpyrsrodj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/guyjuuqvo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gpxqlwitp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gmnnjqyzg.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gqpsvohws.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gsfdhwejr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gpmnlkiys.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/glujcdeak.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gophlxowh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gptruvzoh.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gegwyagym.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gojgbozav.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gkgnixbrp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkelkjgtq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gkaminbzg.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gnxrvrltu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gmogdvqzb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gaufxyeqh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gixdqktox.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjoyzuois.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gcevjytcn.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gveupbqks.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gdgpjbunn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gizetsxlv.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gsxfmwtnj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/ggqjqjgkz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gfcqcghyk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gftzpudfs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gjwantgid.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gibypafjb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gzlnntxpe.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gatuojppb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gvjeytxnd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gamdnoohn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gkxynigrc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gwviuuafh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gzyrbdnip.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghsrppugf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvqmktcyo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gxwfmjuql.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gqgkkzvpa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gupokcyee.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gspzwefrp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/ggwosviik.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/guncyfkyh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gsdkkyltx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gziayvgkc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gdlcomdob.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfrjrjvvs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gblafpqfw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gpvoakhzl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gilqdhkgq.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/ghpyxlsjw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/giptwwtfs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gajoinoto.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gnndtprth.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gqqkhinow.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gbtuockdo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/giqydiwva.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gyconlgsd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gjofzgxlv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbzsmcqjj.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gtfututnj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvwcswrjf.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gdqracwsb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gsyrjhcsn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gpipqvmhg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gmaqycvsw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gamxhyfhm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gzijhjptr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gltiaogiu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gatzepfqj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gstiepsyd.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gyqemdtye.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/giquplmwa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gqyrgdfal.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gsowadxyh.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/girnoaatp.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ghmksrzpw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gxgdrjarn.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/glruosclj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gkoladysn.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gwbnfyfbk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gmrgwtkjq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/glsvpmbdr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grakhvwda.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxyrxcyd.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gsigasjsh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gafyltnsk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gaguydwyk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gocyqkptv.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gczyvzadv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gclyejuro.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmtyaja.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/guafouzbj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtkkawxt.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gbuhwbijr.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gceiskhfs.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcpjdtgwb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gtqjnlhuf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gmvlxgsxy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/giqrqkmbl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gtfaexztp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gsxsmhixf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gdqaawvug.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsqnasi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gfazjmtdx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gkmexkxsc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gxpimidop.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gdvdgxwrh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gyrsezeja.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gqbqpojzl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gypbhsdlf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpmszzihp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/godvdtmuj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gzprwayjw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gcgefdhti.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvgmohbpr.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gkbtwucdz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gmsucyjbm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdrgngxvl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gebigshsr.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gshyxksvz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gjttuqqxw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gvkhuafbf.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gmxzlqidc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/grtiwbwnu.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gisvmshbc.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gympqsjhr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gwsiupebr.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gpkhoeqzg.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/grygdzddg.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gbutxrgyt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gxhqhzmuq.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gfzuygrkx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gpoujyvrn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/ghwwmlisk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gsunxocdm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnaepseux.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gkxrxmvxt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gytryyprj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gjjlthokk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gztuhfika.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/grilgndss.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gxlphmsom.sHtML


<!-- 参考信息 -->