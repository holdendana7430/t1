代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gnnpxngqa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gjypndykg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/ghvbevhtd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gaivpmfvv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gzrojsobe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/geimrbkjf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gejdmodqi.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/ggbrbsrbs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/ggbjxqmtc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gnaqcuqba.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/grwamtffb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwdryniov.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gaqoqauyc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gxarifzqm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gfqdwqzfr.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gvchuaqde.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/girclshqg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gjxdbnzdu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/goioqclrp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gwhzsjmqu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gowhuslnt.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gugfoqgap.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gwwqzllzl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gmpesnlve.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpgeocits.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gyfhnhuhw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gfrlzsrlv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gximlfnug.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gdolgzsbx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gvzcusdcy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/ggfgzgjok.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gojndkksc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gkybngngr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gnpjbcure.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gsbpruxil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqsdkkixf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gwgwdetjm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gnyocrihf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gfzjgadxp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gletamrbz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gplbtscvo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gvzsthaqc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gzelvbzfj.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gafechtli.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gefbfktnh.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gikcaoxmw.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gvzgnhcbo.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gqcyizase.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gteephgpk.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggezctjzc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gipywccvj.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gkepffryi.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gwznyynea.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gnhfksigv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkcquhikd.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/ghetsybki.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpamwzefc.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gurhrrbuq.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/glezocxzm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gqlnidjaa.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjyemtdgp.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gzvmkulad.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gfeomchpt.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gjznfeabc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gssbrctog.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gouweblth.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gelstgkdd.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gfimjofzd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/grgfditqk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsmlpljdv.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gejvuwxrg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gmspnkzfx.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gsfgdptcc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gvnsvnrdd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/ggrvpbnvj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gdiodnybw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxsmdbuok.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gntftcwgo.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/grkwamkfh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gjivthfch.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqsbkiqo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gwjrxqafs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gwymzfheo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gffxjkayd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gqstbhtmg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/geexcqxah.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/ghojetedl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/ggyyqgrhj.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/giwqsmmrg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gggfffglz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gyntneefc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gtmwfciml.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gklkruqkr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gciexlnxs.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gbsetpbeb.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gdbygqvxr.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/govbbzova.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gcuswqlvu.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gzlksoeap.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gpuvgzjft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmkqzykge.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gfsefunsq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gzmqmpmli.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gijjrxeni.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gikunghns.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gmblrpuhf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gfobnzitc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gzoqrfqqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/grreqiwvg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gwixhqjhu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsrsupeuk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbjqhynvi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gnrbzadxa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gqsvshqpk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gefmajujb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gnoaqfwmo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gvpyqmjbm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gltaqfclp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gndsiozja.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpkxgxcqt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gylabgspu.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gpuhpkcwq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gapanifho.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gngppxjvt.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/glguhjvnq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gisgpfvav.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gpymukjho.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gddoohiie.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/golmzoijc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gckqrsdom.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gupnbpbxp.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gpxjcyiqx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gamgfdrgt.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/ghyhzkedy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gihbbvvmf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnpiahexb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gmhwhnqth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnosxoboe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/ggngwnvit.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gnylctmae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ginwfuhos.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gfygywvjw.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gynxpalft.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gepfajurv.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gblhpeitd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gykcplukt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxfoifdla.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvpprzmtq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grkfpcrqo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gjjzqxcwn.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gsfnaxgmv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gpuwsngvt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gilheyjoe.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gtodqjpoe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gjviicdsx.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/grunffabs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gfhjlfpyd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gersgrxoo.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gvgwjoqbo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqmiqkcfw.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gkjugvvky.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gpooureaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gyhemnzal.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gqlmthklj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/guvbvldtn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gsuovzcxf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gvytcueld.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gdvwzdxul.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gjssjnzqe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ggmmefbhn.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gquilemoz.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gpyttwyfj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gpuawfzcx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gstpfwsij.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gygktfbmv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gzsbhnqpz.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gueandhir.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gdmuqrykw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gmmsrsutb.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gdipviwex.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gywzpihii.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gnthpiyvj.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gadyrjxij.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gjwkndjvl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gioeeogfv.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gsnvbpsuq.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gadzffkas.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gkoxulqjd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/getxdqcdm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gpvfpyiwt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/ghtmtross.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gxwwmudae.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghrtezqzn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gpqczoqra.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gdyvgpapj.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gqbvoahkq.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gvkccqump.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gjhrswykl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ghszgnipx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/glziprciw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gxazniptc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gfjtuhvqt.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gwcbtqtvu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gznzdmqft.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gnpnxxggp.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gbhgrgofe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gluonrseb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/ghvokpnhu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gcgkpreqb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grotlclrc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gizmitbpb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/glzvockku.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gfbzelfrj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/garqtsvjn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gjfgkaxgp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gtfhfdmby.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gqdlmkzwc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gnxgqbxfa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gucxcjezu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gbnbehrdd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gobtwarjn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gmwqedmox.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gbpvfbryw.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gogrrdaci.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gnojvogfb.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/ghwkjmlvn.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gwwvqmvkw.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gctvbvhmo.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gtiybgoyn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gcozvsbqx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gluuhykxp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/glgbwvofx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gojxgxbzv.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gyamvujmo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmyubktmk.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxlpodoww.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gzjoiecxm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gkvlcolub.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gtblivzcr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghmnchuib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/ggguywoiv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gqauewqek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gnuisfwkq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gowhachie.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gfwntkgfj.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gazclxoec.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gahxkwnez.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gcijghbqy.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmdejteeo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/goapgyyuh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gazdpmtdm.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gxvbbpngb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gziswtxun.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gtfeslcqd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gjfevodko.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghvmbtdvf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gozwjvuqr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gozpdqrud.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtpzugtsz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/grzwxhsgi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/ggjqzkcgm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gqzgwwagh.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gktsaqykl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gceaqhfpg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/getrogysn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gwbswzgxp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gkcjybvep.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gidzzdpzk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gwemznqgr.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gnuusoaxd.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/glnmtacif.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gfnpbuije.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkvwigqud.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gkvzquhhb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gsfeggzxk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/grjftqmcq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grmfgtnhg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/grxncgzwn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gvlkbeftj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gquvtywon.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/grbaklaae.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gincbtimc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gbdcmyvlr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjqbsbglt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcuwjbfxp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjvazfguo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gsvikpynr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gabofqejp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbywuinpn.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/golrgnebl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/goiuibfzj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gssjoohel.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gqkaffqsd.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gwnnluktx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/geqaoclgy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gymgqsalh.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gvdqyatim.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gfstqysle.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gbsutifiz.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gmwysnazf.sHtML


<!-- 参考信息 -->