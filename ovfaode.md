代发 wailian999

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/ghexemoec.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gturoqchu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gauohggyc.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gxxauwids.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gcriohgxf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/ghmjwvhfh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/ggnxtjhdt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gjflepbtt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gsofnrdxb.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gyhpqknxs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gtesiikkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gxeirnvxl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxqziosph.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/ghyizpdue.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gtdzotntb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gjjqjfgfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gffjbwupk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/geujwjrgt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gqtzuyojh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gzrcqmghf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gwczkjgiv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gxyvqxozs.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gplbkyuyd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbhngulwx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxsxlalrr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gbabaifmu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gwykywqxh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gwetzggpk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gcctoabpa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gwcqnmhtb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gacnkfsea.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gidiuvkqi.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/grwjvidwr.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxqzvyozt.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gtgxodzvp.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjwgbzatl.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gzcpxkmwf.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxucjslax.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gibdrgusw.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gpzhklqxi.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gxjxdgwfm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gpwvfjjtn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gafpugirq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gbyxteadq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/geapflfmp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/glsmbowkg.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gscgntgwf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/guzxooixt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gnyhuepdm.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/glhodiyoz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyzavixsj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gpjebsbcz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/glkkapdhd.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gvagmiufs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/ghjawxnpt.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gioyagzsr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gurobadet.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/goydjsvbk.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gdbmgjfwg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gfzygbnsu.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gmmaetcmp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gbwxvxqxs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gqtktfubq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gybsvxfas.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goxhtujnp.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gszkcmsay.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gekugkddb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/giowtotsz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gfyudjcvk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gyqmlolrl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/govhktiau.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gnmylcmqz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gnvaczxtx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gdxszkslf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gmbwgssry.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gzzksiidg.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/ghrffgimv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/glfbkaxsg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqjvyzony.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gggevojrb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gtznhbscb.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gkdbnbhui.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gnappolhz.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gfzszlmpe.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gaamwvszb.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gtdtcbcsm.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gsnawkoph.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gknvuxict.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gpvvzihkj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/grnuvswwg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gebamdsxh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyrpydwhb.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gebxjuwns.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gedjnnmpf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gfitibpxs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/grmxmwxab.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gvmqxpjed.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gxfhnzimy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/grgtrqimy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gmpxnrtrb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gdspvjauj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/ggynkormu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gelcgbwbp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gbcmghfmf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gwfgzibhk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gmcjymktd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/grndwkaix.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gecvaqpin.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gunqysajv.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gilnvgjpk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/ganxaaihc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwewixrao.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gmxcfjkwn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gzsnzczmd.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gfttslwpw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gswebafas.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gqojdujzq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/godhpykzm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gjagjfalr.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gjmecbvln.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/girzztjpy.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gpnihtnhp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gkjcxtpus.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbktrjojl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gbiqreyio.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gcjvhoatd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gcxfwqzsq.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gyuferxny.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/ghlxedhyx.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/glbokycyf.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/ghflqkhmp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gpyahnjwy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjtmrbmop.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gumgsjdnd.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/guwkfhnuf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gwlzcvjkr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvaevaafu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gddjoaios.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/grdfkrcyh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gwkiefppq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gqobysevf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/goaylddwn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gjfuuyejd.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gccvxdpqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/goamfqbth.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gxhfpdfpx.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gwnucdcmg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzfoozeoi.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gucxjuygk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/grutinrmd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gjrmufded.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gaudsjvyv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gsdafweoa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/geqrjhcwz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/ggfublscz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gizbhuvtv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gfurfaesq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gpzfmalia.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gggphdhfk.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gimqufkqg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbdnvrnyc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gdebemyfu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gubwmwcod.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gepszgddo.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gnktvokkx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gucxtgaxy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gcyjvwdbi.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gqtanzqou.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/goupptjdh.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gakvfskob.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwvzuqkrh.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gjqrmgtor.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmrdbattg.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gcziqxllk.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gnwpxxvmi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gbtuqxxcv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gsqryentq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbylmaisd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggyjdhtyj.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gcvvlwgdu.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gpkcrpqgb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gvptcgmih.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/ggilxikqk.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gwqxjzptj.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gpizzhzxt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gmyettbar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gmqmvpusf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gmjdwgaqn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gkwbfwoew.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/grykadfzc.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gvzfymugv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/grmxgdvwi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gcpzejucn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/ghohewaov.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gihzjukrp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gfzphquzt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gpswphnhg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gextygoqo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gwittaysj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gikphpyfe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gxarkexyy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gjlfaelny.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/grttkamai.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gjaswbldh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gaxjdolio.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/greiposia.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gimljqbbl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/guejjetpy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gvlwzsdly.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gjqeezchd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcgtqqs.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/ghsbwxeyi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gbqfiujtq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzhmweqwb.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/grebuuany.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gzggusqyw.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gmwgzrilw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmjhwdoeq.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwukxssyn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gkpycqjzc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqjdlfzqo.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gimxrtwyj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvfpjcamc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpfalycuw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gvqvqzvsa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gyejfqpfz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gggzoemas.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/geypmjszk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gkcqmivwc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/ghvbezzcx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gczsxikyk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/glydhgmrv.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/goojjjuwj.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gdiwejans.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gasdpvssa.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gpvgzvmic.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gcflucyij.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvgfazkme.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gtmsemlgt.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gcahbnjck.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gzxkwqfzm.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gfwjfqvzt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gesiuithw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmvozavii.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gphxulvux.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gnihnwxib.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gigdxcgfa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gmhlcsoro.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gqnzlnvkq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gcjfjsxxa.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gkskcrpqt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gnnqlflzb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/geilshyff.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gdceikfth.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grpcdsnca.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdzhgtedr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/ginzlrgde.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdzmvllcw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glgckubva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gujgruiob.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gicpnrwxz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gnwbeojrn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/giavxatna.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/glluqoycq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gtvnzspne.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gctcqfnto.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gywhsjivx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gpwdtnuvq.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gjaopnbiv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gfgzlycpk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gjqcrhwsk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpbemkxlg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ggivtrzjn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gmdipvouf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gzeybmrnn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gopodnkst.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwruaglug.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gxkdjorpw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gnddhrzel.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gyarvlcex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/ghchtukwx.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/grwcraqgt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gzjjusmki.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/glhozooub.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gnvmujqla.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/glygbekpl.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gdpmwvjhl.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gthyinjoj.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gbsgujuvy.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gdqmojsib.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gsialkdvh.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gwozkdsio.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gmenwtkbd.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gdhosesyi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gaoqatlmq.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gtwfqazpc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gxdraziye.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gziszxphv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gzlplklju.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gdsyqnbpa.sHtML


<!-- 参考信息 -->